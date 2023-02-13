---
content-type: api
navigation-topic: api-navigation-topic
title: Certificati di sottoscrizione eventi
description: Certificati di sottoscrizione eventi
author: Becky
feature: Workfront API
source-git-commit: 53ef8f4fda22c912c274841d07ad865aa04141c8
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Configurare TLS client per l’abbonamento agli eventi

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

Client TLS ti consente di verificare che il messaggio di abbonamento all’evento ricevuto provenga effettivamente da Adobe Workfront. Per abilitare questa funzionalità, il server deve essere configurato per richiedere e convalidare il certificato Workfront x509.


## Verifica del certificato client Workfront

Questa procedura presuppone che il server sia configurato per accettare connessioni TLS. Workfront non supporta i certificati autofirmati.

In generale, questi sono i passaggi necessari per attivare l’autenticazione client per il server:

1. Scarica la versione PEM del certificato DigiCert Global Root CA.
1. Attiva la verifica del certificato client.

   Specificare il certificato CA dal passaggio 1 come attendibile.

1. Imposta la profondità di verifica su 2 poiché il nostro certificato è effettivamente firmato dal DigiCert SHA2 Secure Server CA che è una CA intermedia sotto DigiCert Global Root CA.
1. Verifica che il certificato client provenga effettivamente da Workfront controllando il relativo nome di dominio oggetto.

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

Per ulteriori informazioni, consulta la sezione [Documentazione NGiNX per ngx_http_ssl_module](http://nginx.org/en/docs/http/ngx_http_ssl_module.html).

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

* [Controllo accesso e autenticazione client](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Modulo Apache mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Mappatura del certificato in ambiente

| Ambiente WF | Nome comune del certificato | Oggetto del certificato (DN) | | — | — | — | | Produzione | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com| | Anteprima | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com | | Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com | | Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Scaricare i certificati

Fare clic sui seguenti collegamenti per scaricare i certificati client.

* [Certificato client - Ambiente di produzione](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [Certificato client - Ambiente di anteprima](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [Certificato client - Ambiente sandbox](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>Puoi utilizzare lo stesso certificato client per entrambi gli ambienti Sandbox.

