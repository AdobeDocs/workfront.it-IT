---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Aggiornare i metadati SAML 2.0 nel provider di identità
description: Puoi aggiornare i metadati SAML 2.0 nel provider di identità.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 96f1d50024605328713ca2019f3b726e27dc569c
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# Aggiornare i metadati SAML 2.0 nel provider di identità

{{important-admin-console-onboard}}

Nelle sezioni seguenti viene descritto come aggiornare i metadati SAML (Security Assertion Markup Language) 2.0 quando si utilizza ADFS (Active Directory Federation Services) come provider di identità.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Utilizza ADFS come provider di identità

È possibile aggiornare i metadati ADFS prima che Adobe Workfront aggiorni il certificato SAML 2.0 o successivo. Se scegli di aggiornare i metadati ADFS prima che Workfront aggiorni il certificato SAML 2.0, sono necessari ulteriori passaggi.

* [Aggiornare i metadati ADFS](#update-your-adfs-metadata)
* [Forza l&#39;aggiornamento dei metadati ADFS](#force-your-adfs-metadata-to-update)

### Aggiornare i metadati ADFS {#update-your-adfs-metadata}

Per impostare i metadati ADFS da aggiornare automaticamente, completa i passaggi descritti in questa sezione.

Per impostazione predefinita, ADFS è configurato per verificare automaticamente la presenza di aggiornamenti a tutti i metadati dell&#39;attendibilità del componente; tuttavia, l’impostazione predefinita prevede il polling solo ogni 24 ore. È possibile modificare questo valore con i comandi powershell.

1. Accedi al server ADFS e apri la console di gestione ADFS.
1. Nel pannello a sinistra, espandi **ADFS 2.0,** quindi espandi **Relazioni di trust.**

1. Fai clic sul pulsante **Fiducia nel partito** cartella.
1. Seleziona l’attendibilità del componente configurato in precedenza per l’utilizzo con Workfront, quindi fai clic su nel pannello di destra **Aggiornamento da metadati federativi**.
1. (Condizionale) Se questa opzione è oscurata (il che significa che l’attendibilità del componente è stata configurata in precedenza utilizzando un file di metadati), completa quanto segue.

   1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

   1. Fai clic su **Sistema** > **Single Sign On (SSO)**.

   1. Fai clic su **Modifica impostazioni.**
   1. Fai clic su **Modifica configurazione**, quindi seleziona **SAML 2.0** in **Tipo** elenco a discesa.

   1. Copia il **URL metadati**, che dovrebbe essere simile al seguente:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Nel server ADFS, fare clic con il pulsante destro del mouse sull&#39;attendibilità del componente configurata in precedenza, quindi fare clic su **Proprietà.**
   1. Fai clic sul pulsante **Monitoraggio** , quindi incolla l’URL copiato da Workfront nel **URL metadati federazione del componente** campo .

   1. Seleziona le opzioni per **Monitorare il gruppo di fiducia** e **Aggiorna automaticamente il componente**.

   1. Fai clic su **OK.**
   1. Selezionare l&#39;attendibilità del componente configurato in precedenza per l&#39;utilizzo con Workfront; quindi, nel pannello di destra, fai clic su **Aggiornamento da metadati federativi.**

1. Fai clic su **OK** ignorare il messaggio relativo ad alcuni contenuti dei metadati federativi non supportati da ADFS 2.0.
1. Apri **Moduli Windows Powershell.**
1. Dopo aver caricato tutti i moduli, esegui il seguente comando in powershell:

   `Get-ADFSProperties`

1. Cerca il valore accanto a **Intervallo di monitoraggio.**

   Sarà un numero che rappresenta il numero di minuti tra i sondaggi. Il valore predefinito deve essere 1440 (1440 minuti = 24 ore).

1. Imposta un nuovo valore eseguendo il seguente comando in powershell:

   `Set-ADFSProperties -MonitoringInterval 1`

   Questo cambia l&#39;intervallo di monitoraggio da ogni 24 ore a ogni minuto. Se desideri che il polling sia meno frequente, puoi cambiare il valore 1 in un altro valore più grande.

1. Per verificare che funzioni correttamente, utilizza la funzione **Visualizzatore eventi** per cercare le seguenti informazioni nei registri ADFS2.0:

   **ID evento 156 e 157**

### Forza l&#39;aggiornamento dei metadati ADFS {#force-your-adfs-metadata-to-update}

Per aggiornare i metadati ADFS completa i passaggi descritti nella sezione seguente.

Per forzare lo scambio dei metadati tra Workfront e il provider SAML 2.0 quando si utilizza ADFS (Active Directory Federation Services):

>[!NOTE]
>
>Alcune di queste modifiche potrebbero essere necessarie al reparto IT.

1. Accedi al server ADFS e apri la **Console di gestione ADFS**.
1. Nel pannello a sinistra, espandi **ADFS 2.0**, quindi espandi **Relazioni di trust**.

1. Fai clic sul pulsante **Fiducia nel partito** cartella.
1. Seleziona l’attendibilità del componente configurato in precedenza per l’utilizzo con Workfront, quindi fai clic su nel pannello di destra **Aggiornamento da metadati federativi**.

   Se questa opzione è disattivata e non può essere selezionata, completa quanto segue:

   (L&#39;opzione viene oscurata solo quando l&#39;attendibilità del componente è stata configurata in precedenza utilizzando un file di metadati.)

   1. In Workfront, nell’area Configurazione, copia il **URL metadati** dalla schermata di configurazione di Workfront Single Sign-On.

      Per accedere alle informazioni per **URL metadati**:

      1. Fai clic su **Configurazione** nell’angolo in alto a destra di Adobe Workfront sulla barra di navigazione globale.
      1. Fai clic su > **Sistema** > **Single Sign On (SSO)**.
      1. Fai clic su **Modifica impostazioni.**
      1. Fai clic su **Modifica configurazione**, quindi seleziona **SAML 2.0** in **Tipo** elenco a discesa.
      1. Copia il **URL metadati**, che dovrebbe essere simile al seguente:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   1. Nel server ADFS, fare clic con il pulsante destro del mouse sull&#39;attendibilità del componente configurata in precedenza, quindi fare clic su **Proprietà.**
   1. Fai clic sul pulsante **Monitoraggio** , quindi incolla l’URL copiato da Workfront nel **URL metadati federazione del componente** campo .
   1. Seleziona le opzioni per **Monitorare il gruppo di fiducia** e **Aggiorna automaticamente il componente**.
   1. Fai clic su **OK**.
   1. Seleziona l’attendibilità del componente configurato in precedenza per l’utilizzo con Workfront, quindi fai clic su nel pannello di destra **Aggiornamento da metadati federativi.**


1. Fai clic su **OK** ignorare il messaggio relativo ad alcuni contenuti dei metadati federativi non supportati da ADFS 2.0.
1. Fai clic su **Aggiorna** per completare l’aggiornamento dei metadati della federazione.

Utenti autorizzati ad accedere a Workfront tramite la schermata di accesso nativa utilizzando le credenziali di accesso di Workfront (questa può essere configurata dalla pagina del profilo di ciascun utente nel **Accesso** sezione) può accedere utilizzando il nome utente e la password Workfront navigando al seguente URL: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Utilizzo di altri provider di identità

Quando utilizzi provider di identità diversi da ADFS (ad esempio Ping, Okta o Centrify), devi ricaricare i metadati Workfront nel provider di identità.

Per ulteriori informazioni su come ottenere un nuovo URL di metadati Workfront, vedi [Aggiornare i metadati ADFS](#update-your-adfs-metadata).

Per ulteriori informazioni sull&#39;utilizzo di ADFS (Active Directory Federation Services) con SAML 2.0 in Workfront, vedere [Configurare Adobe Workfront con SAML 2.0 utilizzando ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
