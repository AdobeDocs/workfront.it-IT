---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configurare Adobe Workfront con SAML 2.0 utilizzando ADFS
description: È possibile abilitare l’autenticazione a Workfront con SAML 2.0.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Configurare Adobe Workfront con SAML 2.0 utilizzando ADFS

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, è possibile integrare Workfront con una soluzione SAML (Security Assertion Markup Language) 2.0 per il single sign-on durante l&#39;utilizzo di ADFS (Active Directory Federation Services).

Questa guida si concentra sulla configurazione di ADFS senza provisioning automatico o mappature degli attributi. È consigliabile completare l&#39;installazione e testarla prima di configurare il provisioning automatico.

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

## Abilitare l’autenticazione a Workfront con SAML 2.0

Per abilitare l’autenticazione all’applicazione web Workfront e all’applicazione mobile Workfront con SAML 2.0, completa le sezioni seguenti:

* [Recupera il file di metadati Workfront SSO](#retrieve-the-workfront-sso-metadata-file)
* [Configurare gli trust del gruppo](#configure-relying-party-trusts)
* [Configurare le regole di attestazione](#configure-claim-rules)
* [Carica il file di metadati e verifica la connessione](#upload-the-metadata-file-and-test-the-connection)

### Recupera il file di metadati Workfront SSO {#retrieve-the-workfront-sso-metadata-file}

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).
1. Nel pannello a sinistra, fai clic su **Sistema** > **Single Sign-On (SSO)**.
1. In **Tipo** menu a discesa, fai clic su **SAML 2.0** per visualizzare informazioni e opzioni aggiuntive.
1. Copia l’URL che viene visualizzato dopo **URL metadati**.
1. Procedi alla sezione seguente, [Configurare gli trust del gruppo](#configure-relying-party-trusts).

### Configurare gli trust del gruppo {#configure-relying-party-trusts}

1. Apri **Gestione ADFS** utilizzo del server Windows 2008 R2 (la versione può variare).
1. Vai a **Iniziate.**
1. Fai clic su **Strumenti di amministrazione.**
1. Fai clic su **Gestione ADFS 2.0.**
1. Seleziona **ADFS** ed espandersi **Relazioni di trust**.
1. Fai clic con il pulsante destro del mouse **Fiducia nel partito**, quindi seleziona **Aggiungi attendibilità parte relazionale** per avviare l&#39;Aggiunta guidata attendibilità parte relying.
1. Da **Pagina di benvenuto**, seleziona **Inizio**.
1. In **Seleziona origine data** incolla l’URL dei metadati da Workfront.
1. Fai clic su **Successivo**.
1. Fai clic su **OK** per confermare il messaggio di avviso.
1. In **Specifica nome visualizzato** aggiungi una sezione **Nome visualizzato** e **Note** per distinguere il trust, fare clic su **Successivo**.
1. Seleziona **Consenti a tutti gli utenti di accedere a questo componente** (o **Nessuno** per configurarlo in un secondo momento).
1. Fai clic su **Successivo**.

   Questo ti porta al **Pronto per aggiungere attendibilità** sezione .

1. Procedi alla sezione seguente [Configurare le regole di attestazione](#configure-claim-rules).

### Configurare le regole di attestazione {#configure-claim-rules}

1. Fai clic su **Successivo** in **Pronto per aggiungere attendibilità** , quindi assicurati che **Apre la finestra di dialogo Modifica regole attestazione** è selezionata.

   In questo modo potrai modificare le Regole attestazione in un passaggio futuro.

1. Fai clic su **Chiudi**.
1. Fai clic su **Aggiungi regola.**
1. Seleziona **Invia attributo LDAP come attestazioni**.
1. Fai clic su **Successivo** per visualizzare **Configura regola attestazione** passo.
1. Specifica i seguenti requisiti minimi per configurare la regola di attestazione: (Questo verrà inserito nella sezione **ID federazione** nella configurazione utente e viene utilizzato per distinguere chi effettua l&#39;accesso.)


   <table >                
      <tbody>
            <tr>
               <td>Nome della regola di attestazione
               </td>
               <td>Specifica un nome per la regola di attestazione. Ad esempio, "Workfront".</td>
            </tr>
            <tr>
               <td>Archiviazione attributi</td>
               <td >Seleziona <b>Active Directory</b> dal menu a discesa.</td>
            </tr>
            <tr>
               <td>Attributo LDAP</td>
               <td>Può essere un qualsiasi tipo di attributo. Si consiglia di utilizzare <b>Nome account SAM</b> per questo attributo.</td>
            </tr>
            <tr>
               <td>Tipo di attestazione in uscita</td>
               <td>Selezionare <b>ID nome</b> come tipo di attestazione in uscita</td>
            </tr>
      </tbody>
   </table>

1. (Facoltativo) Per stabilire il provisioning automatico, aggiungi le seguenti attestazioni aggiuntive sia nell&#39;attributo LDAP che nel tipo di attestazione in uscita:

   * Nome
   * Cognome
   * Indirizzo e-mail

1. Fai clic su **Fine**, quindi fai clic su **OK** nella schermata successiva.
1. Fai clic con il pulsante destro del mouse sul nuovo **Affidabilità del gruppo**, quindi seleziona **Proprietà**.
1. Seleziona la **Scheda Avanzate**. E sotto **Algoritmo hash sicuro** selezionare SHA-1 o SHA-256.

   >[!NOTE]
   >
   >L&#39;opzione selezionata in Algoritmo hash sicuro deve corrispondere al campo Algoritmo hash sicuro in Workfront in Configurazione > Sistema > Single Sign-ON (SSO).

1. Procedi alla sezione seguente [Carica il file di metadati e verifica la connessione](#upload-the-metadata-file-and-test-the-connection).

### Carica il file di metadati e verifica la connessione {#upload-the-metadata-file-and-test-the-connection}

1. Apri un browser e passa a `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Questo dovrebbe scaricare un file di metadati FederationMetadata.xml.

1. Fai clic su **Scegli file** sotto **Compilare campi da metadati del provider di identità**, quindi seleziona la **FederationMetadata.xml** file.

1. (Facoltativo) Se le informazioni sul certificato non sono state compilate con il file di metadati, puoi caricare un file separatamente. Seleziona **Scegli file** in **Certificato** sezione .

1. Fai clic su **Prova connessione**. Se impostato correttamente, dovresti vedere una pagina simile a quella mostrata di seguito:

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Se si desidera impostare la mappatura degli attributi, assicurarsi di copiare gli attributi dalla connessione di prova all&#39;attributo di directory. Per ulteriori informazioni, consulta Mapping degli attributi utente .

1. Seleziona **Esenzione dall&#39;amministratore** per consentire agli amministratori di Workfront di effettuare l&#39;accesso utilizzando le credenziali Workfront con l&#39;url di bypass.

   Segnalibri che puntano a `<yourdomain>`.my.workfront.com/login bypassare il reindirizzamento.

1. Seleziona la **Abilita** per abilitare la configurazione.
1. Fai clic su **Salva**.

## Informazioni sull&#39;aggiornamento degli utenti per SSO

Seguendo questa guida, le **Nome utente SSO** saranno loro **Nome utente di Active Directory**.

In qualità di amministratore Workfront, puoi aggiornare in massa gli utenti per SSO. Per ulteriori informazioni sull&#39;aggiornamento degli utenti per SSO, vedi [Aggiornare gli utenti per il single sign-on](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

In qualità di amministratore di Workfront, puoi anche assegnare manualmente un ID federativo per modificare il profilo dell’utente e completare il campo ID federazione . Per ulteriori informazioni sulla modifica di un utente, consulta [Modificare il profilo di un utente](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Durante la modifica dei profili degli utenti per includere un ID federativo, seleziona **Consenti solo autenticazione SAML 2.0** rimuove la possibilità di accedere a Workfront utilizzando l&#39;url di bypass (`<yourdomain>`.my.workfront.com/login).
