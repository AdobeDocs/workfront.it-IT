---
content-type: api
navigation-topic: api-navigation-topic
title: Certificati di abbonamento agli eventi
description: Certificati di abbonamento agli eventi
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 2c5a4ff65088652b67099d187e6ee4c11d80a3b3
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Configurare Client TLS per la sottoscrizione di eventi

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

Client TLS consente di verificare che il messaggio di abbonamento all’evento ricevuto provenga effettivamente da Adobe Workfront. Per abilitare questa funzionalità, il server deve essere configurato per richiedere e convalidare il certificato x509 di Workfront.


>[!NOTE]
>
>Le sottoscrizioni di eventi utilizzano TLS versione 1.3 se il server a cui la sottoscrizione di eventi invia eventi supporta la versione 1.3. Se il server di connessione non supporta la versione 1.3, la sottoscrizione dell’evento utilizza la versione 1.2 di TLS.



## Verifica certificato client di Workfront

Questa procedura presuppone che il server sia configurato per accettare connessioni TLS. Workfront non supporta i certificati autofirmati.

In generale, questi sono i passaggi necessari per attivare l’autenticazione client per il server:

1. Scarica la versione PEM del certificato CA radice globale di DigiCert.
1. Attiva la verifica del certificato client.

   Specificare il certificato CA del passaggio 1 come attendibile.

1. Imposta l’annidamento della verifica su 2 poiché il nostro certificato è effettivamente firmato dalla CA del server protetto DigiCert SHA2 che è una CA intermedia nella CA radice globale di DigiCert.
1. Verificare che il certificato client provenga effettivamente da Workfront esaminandone il nome di dominio soggetto.

## Esempi di configurazione del server

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

Per ulteriori informazioni, consulta la documentazione di [NGiNX per ngx_http_ssl_module](https://nginx.org/en/docs/http/ngx_http_ssl_module.html).

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

Per ulteriori informazioni, consulta

* [Autenticazione client e controllo degli accessi](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Modulo Apache mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Mappatura certificato-ambiente

| Ambiente WF | Nome comune certificato | Oggetto certificato (DN) |
| -- | -- | -- |
| Production | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| Anteprima | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Scarica certificati

Fai clic sui seguenti collegamenti per scaricare i certificati client.

* [Certificato client - Ambiente di produzione](assets/prod-environment-nov-2024.crt)
* [Certificato client - Ambiente di anteprima](assets/preview-environment-nov-2024.crt)
* [Certificato client - Ambiente sandbox](assets/sandbox-environment-nov-2024.crt)

>[!NOTE]
>
>Puoi utilizzare lo stesso certificato client per entrambi gli ambienti Sandbox.
