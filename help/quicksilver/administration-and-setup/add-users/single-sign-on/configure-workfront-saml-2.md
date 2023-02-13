---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configurare Adobe Workfront con SAML 2.0
description: In qualità di amministratore di Adobe Workfront, puoi configurare le applicazioni web e mobili Workfront per l’integrazione con una soluzione SAML (Security Assertion Markup Language) 2.0 per il single sign-on (SSO).
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 7%

---

# Configurare Adobe Workfront con SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

{{important-admin-console-onboard}}

In qualità di amministratore di Adobe Workfront, puoi configurare le applicazioni web e mobili Workfront per l’integrazione con una soluzione SAML (Security Assertion Markup Language) 2.0 per il single sign-on (SSO).

Dopo aver configurato SAML 2.0 in Workfront, come descritto nelle sezioni seguenti, puoi mantenere la configurazione, come descritto in [Aggiornare i metadati SAML 2.0 nel provider di identità](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Single Sign-On (SSO).**

1. In **Tipo** elenco a discesa, fai clic su **SAML 2.0.**

1. Fai clic su nella parte superiore delle opzioni visualizzate. **Scarica i metadati SAML 2.0** per scaricare il file sul computer.

   Il provider di identità SAML 2.0 richiede un file XML con informazioni generate nella tua istanza Workfront. Dopo aver scaricato il file, devi andare sul server del provider di identità SAML 2.0 e caricare lì il file XML di metadati Workfront SAML 2.0.

1. Specifica le seguenti informazioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ID provider servizi </td> 
      <td> Questo URL, già popolato per te, identifica Workfront nel provider di identità. Ad esempio: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo di associazione</span> </td> 
      <td> <p>Seleziona il metodo supportato dal server IDP per l’invio delle informazioni di autenticazione:</p> 
       <ul> 
        <li>POST</li> 
        <li>REINDIRIZZAMENTO</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compila i campi dai metadati del provider di identità </td> 
      <td>Nella soluzione del provider di identità SAML 2.0, esporta un file XML di metadati del provider di servizi e salvalo in una posizione temporanea sul computer. Seleziona <strong>Scegli file</strong>, quindi trova e seleziona il file salvato per aggiungerlo alla configurazione Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL portale di accesso</span> </td> 
      <td>Specifica il portale di accesso comune della tua organizzazione. Questo è l'URL a cui gli utenti accedono per accedere a Workfront e a tutte le altre applicazioni integrate con SAML 2.0.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL disconnessione</span> </td> 
      <td> <p>Specifica l’URL di disconnessione per il server IDP. Workfront invia una richiesta HTTP a questo URL prima di disconnettersi da Workfront. In questo modo la sessione dell'utente viene chiusa sul server remoto quando la sessione di Workfront viene chiusa.</p> <p><b>NOTA</b>: Viene reindirizzato all’URL di disconnessione solo se nel profilo utente è abilitata l’opzione Consenti solo autenticazione SAML 2.0 .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cambia URL password </td> 
      <td> <p> Specifica l’URL a cui gli utenti verranno reindirizzati per modificare le loro password. </p> <p>Poiché le credenziali SAML 2.0 sono utilizzate per accedere a Workfront, gli utenti devono essere reindirizzati a una pagina in cui possono modificare la password SAML 2.0 invece di completare questa attività tramite Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Algoritmodi Hash sicuro </td> 
      <td> <p>Seleziona l’algoritmo di hash sicuro (SHA) supportato dal tuo IDP:</p> 
       <ul> 
        <li>SHA-1</li> 
        <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fornitura automatica utenti</span> </td> 
      <td> <p>Crea automaticamente un utente nel sistema quando un nuovo utente con nome utente e password di una directory tenta di accedere a Workfront per la prima volta.</p> <p>Per creare utenti in Workfront, è necessario mappare gli attributi dei dati Workfront con i seguenti attributi dei dati utente nel provider di directory:</p> 
       <ul> 
        <li>Nome</li> 
        <li>Cognome</li> 
        <li>Indirizzo Email</li> 
       </ul> 
       <p>Vengono visualizzate le seguenti opzioni per eseguire questa operazione:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Selezionare l'attributo utente di Workfront da mappare dall'elenco a discesa, quindi specificare l'attributo di directory corrispondente nella directory utente.</p> 
       <p>La <strong>Attributo directory</strong> Il campo deve contenere il nome dell'attributo di directory dalla tabella dell'attributo utente salvata durante il test della configurazione SAML 2.0.</p> 
       <p>Puoi impostare un valore Workfront predefinito nel <strong>Valore predefinito</strong> campo . Puoi anche impostare regole in base ai valori del provider di identità SAML 2.0.</p> 
       <p><b>AVVISO</b>: Workfront tenta di mappare gli attributi elencati di seguito ogni volta che un utente accede al sistema. Per questo motivo, si sconsiglia di mappare i livelli di accesso. Puoi rimuovere facilmente l’accesso amministrativo se un attributo viene mappato in modo errato. Fai clic su Aggiungi mappatura per aggiungere altre regole.
       </p> 
       <p>Puoi mappare i seguenti attributi di Workfront:</p> 
      <ul> 
      <li> <p>Livello di accesso</p> </li> 
      <li> <p>Indr</p> </li> 
      <li> <p>Indirizzo2</p> </li> 
      <li> <p>Fatturazione ad Ore</p> </li> 
      <li> <p>Città</p> </li> 
      <li> <p>Azienda</p> </li> 
      <li> <p>Costo al Ora</p> </li> 
      <li> <p>Indirizzo Email</p> </li> 
      <li> <p>Interno</p> </li> 
      <li> <p>Nome</p> </li> 
      <li> <p>Gruppo Predefinito</p> </li> 
      <li> <p>Team predefinito</p> </li> 
      <li> <p>Ruolo</p> </li> 
      <li> <p>Cognome</p> </li> 
      <li> <p>Modello di layout</p> </li> 
      <li> <p>Manager</p> </li> 
      <li> <p>Cellulare</p> </li> 
      <li> <p>Numero di telefono</p> </li> 
      <li> <p>Codice Postale</p> </li> 
      <li> <p>Pianificazione</p> </li> 
      <li> <p>Stato</p> </li> 
      <li> <p>Profilo scheda orario</p> </li> 
      <li> <p>Titolo</p> </li> 
      </ul> </td> 
          <td> </td> 
         </tr> 
        </tbody> 
        <p>Fai clic su <strong>Salva</strong> una volta completata la mappatura degli attributi utente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Certificato </td> 
      <td> <p>Carica un certificato SSL valido per garantire una connessione sicura tra il servizio di autenticazione e Workfront. Per gli account OnDemand, è sempre necessario un certificato. Puoi ottenere questo certificato dal tuo amministratore di sistema SAML 2.0.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eccezione amm. </td> 
      <td> <p>Consente agli amministratori di Workfront di accedere a Workfront utilizzando il proprio accesso a Workfront. Se questa opzione non è selezionata, gli amministratori Workfront devono utilizzare il nome utente e la password SAML 2.0.</p> 
      <p>Workfront tenta innanzitutto di accedere a Workfront tramite SAML 2.0 per gli utenti con il livello di accesso amministratore di sistema di Workfront. Se l'autenticazione SAML 2.0 non riesce, Workfront utilizza l'autenticazione locale per gli amministratori di Workfront.</p> 
      <p>È consigliabile selezionare sempre questa opzione in modo che l’amministratore di Workfront possa accedere a Workfront se il provider SAML 2.0 non è al momento disponibile.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abilita </td> 
      <td> <p>Attiva SSO sul sistema Workfront. Assicurati di aver comunicato le istruzioni di accesso agli utenti.</p> <p>Dopo aver abilitato la configurazione SSO in Workfront, devi attivare la <strong>Consenti solo autenticazione SAML 2.0</strong> per tutti gli utenti in modo che possano utilizzare SSO.</p> <p>Per ulteriori informazioni sull'aggiornamento degli utenti per SSO, vedi <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Aggiornare gli utenti per il single sign-on</a>.</p> <p>Per ulteriori informazioni sulle impostazioni utente, consulta <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modificare il profilo di un utente</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Conferma configurazione </td> 
      <td> 
      <p>Fai clic su <strong>Prova connessione</strong> per verificare che Workfront e il provider di identità SAML 2.0 possano comunicare tra loro. Questa connessione ha esito positivo solo se i file XML sono stati scambiati.
      </p> 
      <p>Dopo aver verificato con successo il collegamento tra il provider di identità SAML 2.0 e Workfront, viene visualizzata una schermata simile a quella riportata di seguito.</p>
      <p><b>NOTA</b>: Questa schermata viene visualizzata in un pop-up del browser, in modo da assicurarti di disabilitare i blocchi pop-up nel browser.</p>
      <p>Salva le informazioni visualizzate nella tabella per un uso successivo.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Salva** per salvare la configurazione SAML 2.0.
