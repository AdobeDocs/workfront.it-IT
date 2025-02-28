---
product-area: projects
navigation-topic: manage-projects
title: Richiede l'approvazione del tempo per un progetto
description: Richiede l'approvazione del tempo per un progetto
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 0%

---

# Richiede l&#39;approvazione del tempo per un progetto

<!--audited: 08/2024-->

Puoi configurare il progetto in modo che le ore registrate vengano approvate dal proprietario del progetto. Se configurate in questo modo, le ore devono prima essere approvate dal proprietario del progetto prima di poter essere utilizzate in un record di fatturazione.\
Per ulteriori informazioni sui record di fatturazione, vedere l&#39;articolo [Creare record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>L&#39;abilitazione di questa opzione non rimuove la capacità di un approvatore della scheda orario di approvare le ore nella scheda orario. Se il proprietario del progetto non approva o rifiuta l&#39;ora, un approvatore della scheda orario può comunque approvarla in una scheda orario.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Per richiedere l'approvazione del tempo per il progetto:</p>
   <ul><li>Nuovo: Standard</li>
   <li>Corrente: Piano</li></ul>

<p>Per approvare le ore registrate in un progetto:</p>
   <ul><li>Nuovo: Chiaro o superiore</li>
   <li>Revisione o successiva</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica l'accesso ai Progetti o versione successiva</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza le autorizzazioni per il progetto o versione successiva</p>
  </tr> 
  <tr> 
   <td role="rowheader">Accesso aggiuntivo</td> 
   <td> <p>Per approvare l’orario in un progetto, devi soddisfare almeno una delle seguenti condizioni:</p> 
    <ul> 
     <li>Sei il proprietario del progetto con l’accesso e le autorizzazioni specificati sopra. In questo caso, se esiste una delle condizioni seguenti, puoi effettuare le seguenti operazioni: 
      <ul>
       <li>Se disponi delle autorizzazioni di gestione per il progetto, puoi approvare o rifiutare le ore registrate sul progetto da qualsiasi altro utente.</li>
       <li> Se disponete dell'accesso Contribuisci o Visualizza al progetto, potrete approvare o rifiutare solo le ore registrate dall'utente o da qualsiasi altro utente che vi segnala.<br></li>
      </ul></li> 
     <li>Disponi di una licenza Pianificazione con accesso amministrativo alle schede orario e alle ore. In questo caso:
      <ul>
       <li>Puoi approvare o rifiutare qualsiasi ora per i progetti per i quali disponi almeno delle autorizzazioni di visualizzazione. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Richiede l&#39;approvazione del tempo per un progetto

Per richiedere l&#39;approvazione del project manager per le ore relative al progetto:

1. Vai al progetto per il quale desideri richiedere l’approvazione per le ore.
1. Fai clic sull&#39;icona **Altro** ![Icona Altro](assets/more-icon.png) a destra del nome del progetto, quindi fai clic su **Modifica**.\
   Viene visualizzata la finestra di dialogo Modifica progetto.

1. Nella sezione **Impostazioni progetto**, seleziona **Richiedi l&#39;approvazione del tempo per questo progetto**.
1. Fai clic su **Salva**.\
   Ora, quando l’ora viene registrata e approvata, viene bloccata e non può essere modificata dall’utente che l’ha inserita nel progetto o nella scheda orario. Solo un amministratore Workfront può regolare l&#39;ora di registrazione.

## Approvare e rifiutare il tempo su un progetto

In qualità di project manager, puoi approvare o rifiutare le ore registrate per attività, problemi o il progetto.

L’approvazione delle ore a livello di progetto non ha alcun impatto sulla scheda orario di nessuno degli utenti che hanno registrato le ore. Ad esempio, le ore nel progetto possono essere approvate dal project manager, ma la scheda orario deve ancora essere approvata dal manager dell&#39;utente o dall&#39;approvatore della scheda orario.

Se si imposta un progetto per richiedere l&#39;approvazione sulle ore registrate, il project manager deve approvare le ore affinché siano disponibili per essere incluse in una fatturazione per il progetto. Per ulteriori informazioni sulla creazione di record di fatturazione, vedere l&#39;articolo [Creare record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md).

Per approvare o rifiutare le ore di un progetto:

1. Vai al progetto.
1. Fai clic sull&#39;area **Ore** nel pannello a sinistra. Potrebbe trovarsi nell&#39;area **Mostra altro**.

1. Vengono visualizzate le ore registrate per problemi, attività e progetto con lo stato **Inviato**.\
   Fai clic sulla casella a sinistra delle voci orarie per selezionare le ore da approvare.

1. Fai clic sull&#39;icona **Approva** ![](assets/approve-hours-icon.png) in alto nell&#39;elenco delle ore.\
   Lo stato delle ore cambia in **Approvato**.\
   Se successivamente si rifiutano le ore approvate, lo stato delle ore cambia in **Non approvato**.\
   Quando si includono le ore approvate in un record di fatturazione, lo stato delle ore cambia in **Fatturate e Approvate**. Le ore aggiunte a un record di fatturazione non possono essere eliminate. Per ulteriori informazioni sulla creazione di record di fatturazione, vedere l&#39;articolo [Creare record di fatturazione](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Facoltativo) Fai clic sull&#39;icona ![](assets/reject-hours-icon.png) di tipo **Rifiuta** per rifiutare le voci di ora nel progetto.\
   Lo stato delle ore diventa **Rifiutato**.

   >[!NOTE]
   >
   >   Se le ore selezionate sono incluse in una fatturazione contrassegnata come Fatturata o Fatturata e approvata, le icone Approva e Rifiuta non vengono visualizzate. Puoi approvare solo le ore che non sono già fatturate in un record fatturazione.

