---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configurare Adobe Workfront con SAML 2.0 utilizzando ADFS
description: È possibile abilitare l’autenticazione in Workfront con SAML 2.0.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Configurare Adobe Workfront con SAML 2.0 utilizzando ADFS

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, è possibile integrare Workfront con una soluzione SAML (Security Assertion Markup Language) 2.0 per il Single Sign-On durante l&#39;utilizzo di Active Directory Federation Services (ADFS).

Questa guida si concentra sulla configurazione di ADFS senza provisioning automatico o mappature di attributi. È consigliabile completare la configurazione e testarla prima di configurare il provisioning automatico.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abilitare l’autenticazione in Workfront con SAML 2.0

Per abilitare l’autenticazione all’applicazione web Workfront e all’applicazione mobile Workfront con SAML 2.0, completa le sezioni seguenti:

* [Recupera il file di metadati SSO di Workfront](#retrieve-the-workfront-sso-metadata-file)
* [Configura trust relying party](#configure-relying-party-trusts)
* [Configura regole attestazione](#configure-claim-rules)
* [Carica il file di metadati e verifica la connessione](#upload-the-metadata-file-and-test-the-connection)

### Recuperare il file di metadati SSO di Workfront {#retrieve-the-workfront-sso-metadata-file}

{{step-1-to-setup}}

1. Nel pannello a sinistra, fare clic su **Sistema** > **Single Sign-On (SSO)**.
1. Nel menu a discesa **Tipo**, fare clic su **SAML 2.0** per visualizzare ulteriori informazioni e opzioni.
1. Copia l&#39;URL visualizzato dopo **URL metadati**.
1. Passare alla sezione seguente, [Configurare trust relying party](#configure-relying-party-trusts).

### Configura trust tra componente {#configure-relying-party-trusts}

1. Aprire **ADFS Manager** utilizzando Windows Server 2008 R2 (la versione può variare).
1. Vai a **Inizio.**
1. Fare clic su **Strumenti di amministrazione.**
1. Fare clic su **Gestione ADFS 2.0.**
1. Selezionare **ADFS** ed espandere **Relazioni di attendibilità**.
1. Fare clic con il pulsante destro del mouse su **Trust relying party**, quindi selezionare **Aggiungi trust relying party** per avviare l&#39;Aggiunta guidata trust relying party.
1. Dalla **pagina di benvenuto**, seleziona **Inizio**.
1. Nella sezione **Seleziona data Source**, incolla l&#39;URL dei metadati da Workfront.
1. Fai clic su **Avanti**.
1. Fare clic su **OK** per confermare il messaggio di avviso.
1. Nella sezione **Specifica nome visualizzato**, aggiungi **Nome visualizzato** e **Note** per distinguere il trust, quindi fai clic su **Avanti**.
1. Selezionare **Consenti a tutti gli utenti di accedere a questo componente** (o **Nessuno** se si desidera configurarlo in un secondo momento).
1. Fai clic su **Avanti**.

   Viene visualizzata la sezione **Pronto per aggiungere trust**.

1. Passare alla sezione seguente [Configurare le regole di attestazione](#configure-claim-rules).

### Configurare le regole di attestazione {#configure-claim-rules}

1. Fare clic su **Avanti** nella sezione **Pronto per aggiungere trust**, quindi verificare che sia selezionata l&#39;opzione **Apri la finestra di dialogo Modifica regole attestazione**.

   In questo modo sarà possibile modificare le regole di attestazione in un passaggio futuro.

1. Fai clic su **Chiudi**.
1. Fai clic su **Aggiungi regola.**
1. Selezionare **Invia attributo LDAP come attestazioni**.
1. Fare clic su **Avanti** per visualizzare il passaggio **Configura regola attestazione**.
1. Specificare i seguenti requisiti minimi per configurare la regola attestazione: (questo valore verrà inserito in **ID federazione** nella configurazione utente e verrà utilizzato per distinguere gli utenti che effettuano l&#39;accesso).


   <table >                
      <tbody>
            <tr>
               <td>Nome regola attestazione
               </td>
               <td>Specificare un nome per la regola attestazione. Ad esempio, "Workfront".</td>
            </tr>
            <tr>
               <td>Archivio attributi</td>
               <td >Selezionare <b>Active Directory</b> dal menu a discesa.</td>
            </tr>
            <tr>
               <td>Attributo LDAP</td>
               <td>Può essere qualsiasi tipo di attributo. È consigliabile utilizzare <b>SAM-Account-Name</b> per questo attributo.</td>
            </tr>
            <tr>
               <td>Tipo di attestazione in uscita</td>
               <td>Selezionare <b>ID nome</b> come tipo di attestazione in uscita</td>
            </tr>
      </tbody>
   </table>

1. (Facoltativo) Per stabilire il provisioning automatico, aggiungere le seguenti attestazioni aggiuntive sia nell&#39;attributo LDAP che nel tipo di attestazione in uscita:

   * Nome assegnato
   * Cognome
   * Indirizzo e-mail

1. Fai clic su **Fine**, quindi fai clic su **OK** nella schermata successiva.
1. Fare clic con il pulsante destro del mouse sul nuovo **trust relying party**, quindi selezionare **Proprietà**.
1. Seleziona la **scheda Avanzate**. In **Algoritmo hash protetto** selezionare SHA-1 o SHA-256.

   >[!NOTE]
   >
   >L’opzione selezionata in Algoritmo hash sicuro deve corrispondere al campo Algoritmo hash sicuro in Workfront in Configurazione > Sistema > Single Sign-ON (SSO).

1. Passare alla sezione seguente [Caricare il file di metadati e verificare la connessione](#upload-the-metadata-file-and-test-the-connection).

### Carica il file di metadati e verifica la connessione {#upload-the-metadata-file-and-test-the-connection}

1. Aprire un browser e passare a `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml`.

   Questo dovrebbe scaricare un file di metadati FederationMetadata.xml.

1. Fare clic su **Scegli file** in **Compila campi da metadati provider identità** e selezionare il file **FederationMetadata.xml**.

1. (Facoltativo) Se le informazioni sul certificato non sono state inserite nel file di metadati, puoi caricare un file separatamente. Selezionare **Scegli file** nella sezione **Certificato**.

1. Fare clic su **Verifica connessione**. Se configurato correttamente, dovresti vedere una pagina simile a quella mostrata di seguito:

   ![Messaggio di successo SAML 2](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Se si desidera impostare la mappatura degli attributi, assicurarsi di copiare gli attributi dalla connessione di prova all&#39;attributo di directory. Per ulteriori informazioni, consulta Mappatura degli attributi utente.

1. Seleziona **Esenzione amministratore** per consentire agli amministratori di Workfront di accedere utilizzando le credenziali di Workfront con l&#39;URL ignorato.

   I segnalibri che indicano `<yourdomain>`.my.workfront.com/login ignorano il reindirizzamento.

1. Selezionare la casella **Abilita** per abilitare la configurazione.
1. Fai clic su **Salva**.

## Informazioni sull&#39;aggiornamento degli utenti per l&#39;SSO

Seguendo questa guida, il **nome utente SSO** sarà il **nome utente Active Directory**.

In qualità di amministratore di Workfront, puoi aggiornare in blocco gli utenti per l’SSO. Per ulteriori informazioni sull&#39;aggiornamento degli utenti per l&#39;SSO, vedere [Aggiornare gli utenti per il Single Sign-On](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

In qualità di amministratore di Workfront, puoi anche assegnare manualmente un ID federazione modificando il profilo dell’utente e completando il campo ID federazione. Per ulteriori informazioni sulla modifica di un utente, vedere [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Quando si modificano i profili degli utenti in modo da includere un ID federazione, se si seleziona **Consenti solo autenticazione SAML 2.0** non sarà più possibile accedere a Workfront utilizzando l&#39;URL bypass (`<yourdomain>`.my.workfront.com/login).
