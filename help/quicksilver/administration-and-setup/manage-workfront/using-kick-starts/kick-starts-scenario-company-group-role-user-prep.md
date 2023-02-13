---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart, calcio d'inizio, kickstart, calcio d'inizio
navigation-topic: use-kick-starts
title: 'Scenario di avvio rapido: Preparazione di Azienda, Gruppo, Ruolo e User Kick-Start"'
description: Quando inizi a implementare Adobe Workfront, invece di inserire manualmente i dati, puoi importare l’elenco dei clienti, i reparti interni, i ruoli e le informazioni utente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 10%

---

# Scenario di partenza: Preparazione per azienda, gruppo, ruolo e avvio utente

Quando inizi a implementare Adobe Workfront, invece di inserire manualmente i dati, puoi importare l’elenco dei clienti, i reparti interni, i ruoli e le informazioni utente.

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

## Cosa importare

Nella tabella seguente vengono visualizzate le società, i gruppi e i ruoli da importare:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aziende</strong> </th> 
   <th><strong>Gruppi</strong> </th> 
   <th><strong>Mansioni</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme, Co</p> <p>Workfront, Inc.</p> <p><em>La tua azienda</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">Finanz</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Agente di Vendita</p> </td> 
   <td valign="top"> <p valign="top">Analista aziendale</p> <p valign="top">Creative controller</p> <p valign="top">Designer</p> <p valign="top">Responsabile risorse</p> <p valign="top">Master Scrum</p> <p valign="top">Redattore tecnico</p> <p valign="top">Sviluppatore web</p> </td> 
  </tr> 
 </tbody> 
</table>

I nomi dei ruoli devono essere univoci. Impossibile importare i ruoli di lavoro esistenti.

Le tabelle seguenti mostrano gli utenti da importare e diversi attributi utente per ciascuno di essi:

### Utente 1

| **Nome** | Chris |
|---|---|
| **Cognome** | Manning |
| **Nome utente/E-mail** | mailto:cmanning@foo.com |
| **Password** | updateMe |
| **Accesso** | Membro team |
| **Azienda** | &lt;*La tua azienda>* |
| **Gruppo Predefinito** | Marketing |
| **Ruolo** | Analista aziendale |

{style=&quot;table-layout:auto&quot;}

### Utente 2

| **Nome** | Jennifer |
|---|---|
| **Cognome** | Campbell |
| **Nome utente/E-mail** | jcampbell@foo.com |
| **Password** | updateMe |
| **Accesso** | Project Manager |
| **Azienda** | &lt;*La tua azienda>* |
| **Gruppo Predefinito** | Marketing |
| **Ruolo** | Project Manager |

{style=&quot;table-layout:auto&quot;}

### Utente 3

| **Nome** | Jill |
|---|---|
| **Cognome** | Sullivan |
| **Nome utente/E-mail** | jsullivan@foo.com |
| **Password** | updateMe |
| **Accesso** | Help Desk |
| **Azienda** | &lt;*La tua azienda>* |
| **Gruppo Predefinito** | Agente di Vendita |
| **Ruolo** | Rappresentante commerciale |

{style=&quot;table-layout:auto&quot;}

### Utente 4

| **Nome** | Marc |
|---|---|
| **Cognome** | Lewis |
| **Nome utente/E-mail** | mlewis@foo.com |
| **Password** | updateMe |
| **Accesso** | Manager portfolio |
| **Azienda** | &lt;*La tua azienda>* |
| **Gruppo Predefinito** | Finanz |
| **Ruolo** | Controller |

{style=&quot;table-layout:auto&quot;}

### Utente 5

| **Nome** | Pam |
|---|---|
| **Cognome** | Reynolds |
| **Nome utente/E-mail** | preynolds@foo.com |
| **Password** | updateMe |
| **Accesso** | Project Manager |
| **Azienda** | *La tua azienda>* |
| **Gruppo Predefinito** | Marketing |
| **Ruolo** | IT |

{style=&quot;table-layout:auto&quot;}

### Utente 6

| **Nome** | Ray |
|---|---|
| **Cognome** | Andrews |
| **Nome utente/E-mail** | randrews@foo.com |
| **Password** | updateMe |
| **Accesso** | Amministratore |
| **Azienda** | *La tua azienda>* |
| **Gruppo Predefinito** | Responsabile risorse |
| **Ruolo** | nessuno |

{style=&quot;table-layout:auto&quot;}

## Scarica un modello di avvio rapido

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Avvio** > **Importa dati.**

1. Fai clic su **Altre opzioni** per visualizzare l’elenco completo delle opzioni di importazione.
1. Selezionare gli oggetti Livello di accesso, Società, Gruppo, Ruolo lavoro e Utente che si desidera importare.

## Informazione della società

1. Apri **Workfront.xlsx** file appena scaricato.

   >[!TIP]
   >
   >Quando si lavora con fogli di dati molto ampi, è possibile utilizzare lo strumento Freeze Pane (o equivalente) dell’editor per fogli di calcolo per semplificare il funzionamento del foglio di calcolo.

1. Vai al foglio &quot;Società CMPY&quot;.

   Dovrebbe essere vuoto a meno che le aziende non siano già nel sistema. ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. Specifica TRUE nel **isNew** colonna.
1. Ripeti questa azione per ogni azienda aggiunta. (In questo esempio, completa questa azione per le righe 3-6, perché vengono aggiunte quattro società.)

   ![](assets/cmpyisnew-350x86.png)

1. Specifica un ID univoco.

   Questa operazione deve essere eseguita per ogni riga della colonna ID. Gli interi a partire da 1 funzionano bene quando si creano nuovi record.

   ![](assets/cmpyisnew-350x86.png)

1. Impostare un Nome.

   Specifica i nomi di ogni cliente nella **setName** colonna.

   ![](assets/companyid-350x78.png)

1. Passare al foglio Gruppo di gruppi.

   A meno che non siano già stati creati gruppi in Workfront, in questo foglio deve essere visualizzato solo il gruppo predefinito predisposto per ogni account di Workfront.

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. Imposta la **isNew** column.Secondo lo scenario, verranno importati 4 gruppi, quindi specificare TRUE nelle righe da 4 a 7 per la colonna &#39;isNew&#39;.
1. Specifica un ID univoco.

   Questa operazione deve essere eseguita per ogni riga della colonna ID. Gli interi a partire da 1 funzionano bene quando si creano nuovi record.

   ![](assets/groupids-350x85.png)

1. Impostare un Nome.

   Specifica i nomi di ogni reparto nel **setName** colonna.

   ![](assets/groupnames-350x85.png)

   Specifica le informazioni sul ruolo. Passa al foglio Ruolo RUOLO .

1. A meno che non siano già stati creati o eliminati ruoli nel tuo account, in questo foglio devono essere visualizzati 8 ruoli per i quali è stato eseguito il provisioning con ogni account di Workfront.

   ![](assets/groupnames-350x85.png)

1. Imposta l&#39;istruzione True.

   Sono in corso l’importazione di sette ruoli di lavoro, inserisci TRUE nelle righe da 12 a 18 per la colonna &quot;isNew&quot;.

   ![](assets/roleisnew-350x104.png)

1. Specifica un ID univoco.

   Questa operazione deve essere eseguita per ogni riga della colonna ID. Gli interi a partire da 1 funzionano bene quando si creano nuovi record.

   ![](assets/usersheet-350x16.png)

   ![](assets/roleisnew--1--350x104.png)

1. Immetti un nome per ciascun ruolo digitandolo nella colonna setName.

   ![](assets/roleisnew-350x104.png)

1. Fornisci ulteriori dettagli in base alle esigenze.

   Includere le tariffe di fatturazione, le tariffe di costo e le descrizioni dei ruoli che si stanno creando, in base alle esigenze.

1. Vai al foglio Utente per inserire le Informazioni utente.

   A meno che gli utenti non siano già stati creati nel tuo account, in questo foglio deve essere visualizzato solo l’utente amministratore che viene fornito con ogni account di Workfront.

   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)

1. Imposta il valore True specificando TRUE nelle righe da 4 a 9 per la colonna &#39;isNew&#39;, in quanto vengono importati 6 utenti.

   ![](assets/userisnew-350x52.png)

1. Imposta un ID univoco specificando un ID univoco in ogni riga per la colonna ID. In genere i numeri interi a partire da 1 funzionano bene per i nuovi record.

   ![](assets/userisnew-350x52.png)

1. Inserisci i nomi di ogni utente nelle colonne &#39;setFirstName&#39; e &#39;setLastName&#39;.

   ![](assets/usernames-350x52.png)

1. Imposta i valori di dettaglio specificando i valori nelle colonne &#39;setEmail,&#39; &#39;setPassword&#39; e &#39;setUsername&#39;.

   ![](assets/usercredentials-350x52.png)

1. Specificare i valori del livello di accesso.

   Ad esempio, Chris Manning, membro del team, cerca l&#39;ID nel foglio del livello di accesso ACSLVL per il livello di accesso al membro del team. Copia l&#39;ID negli Appunti e incollalo nel foglio Utente UTENTE **setAccessLevelID** nella riga di Chris.

   Ripeti questo passaggio per ogni utente e livello di accesso.

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. Specifica i dettagli del gruppo home.

   Secondo lo scenario, Chris Manning appartiene al gruppo Marketing. Nel foglio Gruppo, individua l&#39;ID del gruppo Marketing, copialo negli appunti e, nel foglio Utente UTENTE, incollalo nel **setHomeGroupID** nella riga di Chris. &#x200B;Ripetere questo passaggio per ogni assegnazione utente e gruppo.

   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)

1. Specifica i dettagli aziendali.

   Tutti gli utenti in questo scenario appartengono alla stessa azienda. Sul foglio della società CMPY, individua l’ID della società *La tua azienda *Società, copia l’ID negli appunti e, nella scheda Utente UTENTE, incolla questo valore in ogni riga della colonna &#39;setCompanyID&#39;. &#x200B;

   Ripetere questo passaggio per ogni assegnazione utente e gruppo.

   ![](assets/companyid--1--350x78.png)

   ![](assets/pastecompanyid-350x84.png)

1. Specifica i dettagli del ruolo del lavoro.

   Secondo lo scenario, Chris Manning avrà il ruolo di Business Analyst. Nel foglio Ruolo RUOLO individuare l&#39;ID per il ruolo Analista aziendale, copiarlo negli Appunti e nel foglio Utente UTENTE incollarlo nella colonna &#39;setRoleID&#39; nella riga Chris&#39;. &#x200B;Ripetere questo passaggio per ogni assegnazione utente e gruppo.

   ![](assets/copyroleid-350x149.png)

   ![](assets/pasteroleid-350x95.png)

1. Inserisci altri dettagli utente, se necessario, quindi salva il file.
1. Importa il file Excel.

   Seguire le indicazioni fornite nel **Importazione di file di avvio del pulcino** sezione di questo articolo.
