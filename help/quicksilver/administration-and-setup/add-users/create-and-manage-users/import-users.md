---
title: Importare utenti
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: È possibile importare gli utenti nel sito Adobe Workfront sincronizzando gli utenti da un servizio di directory di rete (ad esempio Active Directory o un'altra directory LDAP) oppure importando gli utenti utilizzando un file di importazione del foglio di calcolo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

# Importare utenti

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per istruzioni su come modificare il profilo di un utente in Adobe Admin Console, consulta la sezione &quot;Aggiungere utenti&quot; nell’articolo [Caricamento in blocco degli utenti](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) oppure contatta l’amministratore Adobe Admin Console.
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

È possibile importare gli utenti mediante un file di importazione per foglio di calcolo.

Prima di creare un nuovo utente, assicurarsi innanzitutto di aver creato tutti gli oggetti che si desidera associare all&#39;utente. Ad esempio, se non è stata creata una pianificazione, non è possibile assegnarla al nuovo utente e il campo utilizzato per associare una pianificazione al nuovo utente non viene visualizzato nella schermata Nuovo utente.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

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
   <td> <p>Devi disporre di una delle seguenti caratteristiche:</p> 
    <ul> 
     <li> <p>Livello di accesso amministratore di sistema. Per informazioni, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>. </p> </li> 
     <li> <p><b>Utenti</b> impostazione nel livello di accesso configurato per <b>Modifica</b> accesso, con <b>Crea</b> e almeno uno dei due <b>Amministratore utente</b> opzioni attivate in <b>Ottimizzare le impostazioni</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Di queste due opzioni, se Utente <b>Amministratore (utenti del gruppo)</b> è abilitato, devi essere un amministratore di gruppo di un gruppo in cui l’utente è membro.</p> <p>Per ulteriori informazioni sulla <b>Utenti</b> impostazione in un livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concedere l’accesso agli utenti</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Utilizzare un file di importazione per fogli di calcolo per importare gli utenti

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).

1. Fai clic sul pulsante **Nuovo utente** freccia a discesa, quindi fai clic su **Importa utenti**.

1. In **Importa utenti** che viene visualizzata, scarica il file di esempio, quindi aggiorna il file di esempio per includere le informazioni personali del tuo utente.

   Ogni riga include i campi seguenti:

   * **Nome**
   * **Cognome**
   * **Indirizzo Email**

      Gli indirizzi e-mail devono essere univoci.

   * **Livello di accesso**

      I livelli di accesso sono sensibili all’uso di maiuscole e minuscole.

   * **ID accesso SSO**

      Questo campo è incluso solo se l&#39;SSO è abilitato nel sistema. È necessario aggiungere l&#39;ID federazione in questo campo per ogni utente. Quando crei un utente dalla scheda Persone, puoi impostare una password per l’utente se desideri consentire agli utenti di accedere senza SSO. Tuttavia, la funzione di importazione non consente di lasciare vuoto l’ID ACCESSO SSO SSO.

   * Assicurati che non esistano spazi aggiuntivi prima o dopo l’indirizzo e-mail di un utente.

   Una volta completata la riga, l’aspetto dovrebbe essere il seguente:

   ![import-new-users.png](assets/importing-new-users.png)

1. Salva il file in una posizione sulla tua workstation.
1. Fai clic su **Scegli file** in **Importa utenti** scatola.

1. Individua e seleziona il file salvato.
1. (Facoltativo) Seleziona la **Invia un messaggio e-mail di invito a questo utente** per inviare un invito e-mail all’utente, avvisandolo della creazione di un account Workfront e chiedendo loro di impostare la password.

   Deseleziona questa opzione se desideri impostare la password per l’utente.

1. Fai clic su **Importa**.

   Nella parte superiore della schermata viene visualizzato un messaggio di conferma del corretto inserimento dell’utente.
