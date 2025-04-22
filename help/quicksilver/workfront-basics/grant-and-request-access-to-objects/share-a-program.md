---
title: Condividere un programma
product-area: projects
keywords: condivisione,programma,autorizzazioni
navigation-topic: grant-and-request-access-to-objects
description: L’amministratore di Adobe Workfront può concederti l’accesso per visualizzare o modificare i programmi al momento dell’assegnazione del livello di accesso. Per poter accedere alla modifica di un programma è necessario disporre di una licenza Pianificazione.
author: Courtney
feature: Get Started with Workfront
exl-id: bfa6ce97-24ad-44b3-9c2f-7fac6b748f94
source-git-commit: eb4bf18407562b88bf0c946c905b202e5b62a5fe
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# Condividere un programma


L’amministratore di Adobe Workfront può concederti l’accesso per visualizzare o modificare i programmi al momento dell’assegnazione del livello di accesso. Per poter accedere alla modifica di un programma è necessario disporre di una licenza Pianificazione. Per ulteriori informazioni, vedere [Concedere l&#39;accesso ai programmi](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md).

Oltre al livello di accesso concesso, è possibile ricevere autorizzazioni per visualizzare o gestire programmi specifici da utenti che possono condividerli con l&#39;utente. Per ulteriori informazioni sui livelli di accesso e sulle autorizzazioni, vedere [Funzionamento dei livelli di accesso e delle autorizzazioni](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Le autorizzazioni sono specifiche per ciascun elemento in Workfront e definiscono quali azioni gli utenti possono intraprendere su tale elemento.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per condividere gli oggetti, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Nuovo: Standard</p> 
   Oppure
   <p>Corrente: Lavoro o versione successiva</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o superiore agli oggetti da condividere</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizzare le autorizzazioni o versioni successive per gli oggetti da condividere</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sulla condivisione di un programma

Oltre alle considerazioni riportate di seguito, vedere anche [Panoramica sulle autorizzazioni di condivisione per gli oggetti](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un amministratore di Workfront può aggiungere o rimuovere autorizzazioni per qualsiasi elemento del sistema, per tutti gli utenti, senza esserne il proprietario.

* Per impostazione predefinita, l’autore di un programma dispone delle autorizzazioni di gestione.

* È possibile condividere i programmi singolarmente o più programmi contemporaneamente.

  Per ulteriori informazioni sulla condivisione di elementi in Workfront, vedere [Condividere un oggetto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* È possibile concedere le autorizzazioni Visualizza o Gestisci solo ai programmi:

* Quando si condivide un programma, per impostazione predefinita gli utenti ereditano le stesse autorizzazioni per tutti gli oggetti figlio associati al programma.

  Per ulteriori informazioni sulla gerarchia degli oggetti in Workfront, vedere [Informazioni sugli oggetti in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Puoi rimuovere le autorizzazioni ereditate dal programma. Per ulteriori informazioni sulla rimozione delle autorizzazioni dagli oggetti, vedere  [Rimuovi le autorizzazioni dagli oggetti](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Condividere un programma

{{step1-to-programs}}

1. Nella pagina **Programmi** selezionare il programma che si desidera condividere. Viene visualizzata la pagina del programma.

1. A destra del nome del programma, fai clic su **Condividi**. Viene visualizzata la finestra di dialogo **Condividi [Nome programma]**.

   ![Pulsante Condividi programma](assets/share-program-button.png)

1. Nel campo **Concedi l&#39;accesso al programma**, inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui si desidera condividere il programma, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >Puoi condividere un programma solo con utenti attivi, team, ruoli o aziende.


1. (Facoltativo) Selezionare l&#39;elenco a discesa **Chi ha accesso** e selezionare il livello di accesso del programma:

   * **Solo gli utenti invitati possono accedere a:** Solo gli utenti invitati al programma possono accedervi (impostazione predefinita).
   * **Tutti gli utenti del sistema possono visualizzare**: tutti gli utenti del sistema possono visualizzare il programma senza un invito.


1. Fai clic sull’elenco a discesa a destra del nome dell’utente e seleziona il relativo livello di autorizzazione per questo programma:

   * **Visualizza**: l&#39;utente può rivedere e condividere il programma.
   * **Gestisci**: l&#39;utente ha accesso completo al programma senza diritti amministrativi, che sono concessi al livello di accesso (include anche tutte le autorizzazioni di visualizzazione).

1. (Facoltativo) Fai clic sull’icona delle opzioni avanzate accanto al livello di autorizzazione concesso per configurare autorizzazioni specifiche per il programma.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-options-icon.png)

1. (Facoltativo) Per disattivare le autorizzazioni ereditate per gli oggetti figlio del programma, fare clic su **Disattiva** in linea con **Autorizzazioni ereditate**.

1. (Facoltativo) Per condividere rapidamente il programma utilizzando un collegamento, fare clic su **Copia collegamento** e quindi inoltrarlo al destinatario.

1. Fai clic su **Salva**.

## Condivisione di programmi in blocco

{{step1-to-programs}}

1. Nella pagina **Programmi**, seleziona la casella a sinistra di ogni programma che desideri condividere, quindi fai clic sull&#39;icona **Condividi** ![Condividi icona](assets/share-icon.png) nella parte superiore della pagina. Viene visualizzata la finestra modale di condivisione.

   ![Programmi di condivisione in blocco](assets/bulk-share-programs.png)

1. Nel campo **Concedi l&#39;accesso al programma**, inizia a digitare il nome dell&#39;utente, del team, della mansione, del gruppo o della società con cui desideri condividere i programmi, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.

   >[!TIP]
   >
   >Puoi condividere i programmi solo con utenti attivi, team, ruoli o aziende.


1. (Facoltativo) Selezionare l&#39;elenco a discesa **Chi ha accesso** e selezionare il livello di accesso dei programmi:

   * **Solo gli utenti invitati possono accedere a:** Solo gli utenti invitati ai programmi possono accedervi (impostazione predefinita).
   * **Tutti gli utenti del sistema possono visualizzare**: tutti gli utenti del sistema possono visualizzare i programmi senza un invito.


1. Fai clic sull’elenco a discesa a destra del nome dell’utente e seleziona il relativo livello di autorizzazione per i programmi:

   * **Visualizza**: l&#39;utente può esaminare e condividere i programmi.
   * **Gestisci**: l&#39;utente ha accesso completo ai programmi senza diritti amministrativi, che sono concessi al livello di accesso (include anche tutte le autorizzazioni di visualizzazione).

1. (Facoltativo) Fai clic sull’icona delle opzioni avanzate accanto al livello di autorizzazione concesso per configurare autorizzazioni specifiche per i programmi.

   ![Opzioni di autorizzazione avanzate configurate](assets/advanced-options-icon.png)

1. Fai clic su **Salva**.

## Autorizzazioni del programma

Nella tabella seguente vengono visualizzate le autorizzazioni che è possibile concedere agli utenti quando si consente loro di visualizzare o gestire un programma:

| **Azioni** | **Gestisci** | **Visualizza** |
|---|---|---|
| Modifica dettagli programma | ✓ |   |
| Visualizzare un programma | ✓ | ✓ |
| Eliminare un programma | ✓ |   |
| Allegare un modulo personalizzato | ✓ |   |
| Modificare un campo personalizzato | ✓ |   |
| Aggiungere o rimuovere un progetto&#42; | ✓ |   |
| Approvare un progetto | ✓ |   |
| Aggiungi cartella documenti&#42; | ✓ | ✓ |
| Aggiungi un documento | ✓ | ✓ |
| Aggiungi aggiornamenti/commenti | ✓ | ✓ |
| Condividi | ✓ | ✓ |
| Condividi a livello di sistema |   | ✓ |

*Queste autorizzazioni sono controllate dal livello di accesso e dalle autorizzazioni su altri oggetti, come i progetti.


