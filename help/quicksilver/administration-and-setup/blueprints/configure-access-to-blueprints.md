---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configurare l’accesso alle blueprint
description: In qualità di amministratore di sistema, puoi consentire agli utenti di accedere per richiedere l’installazione dei progetti impostando una coda di richiesta per archiviare le richieste. Qui, disponi di una singola posizione per monitorare e aggiornare le richieste.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Configurare l’accesso alle blueprint

Tutto [!DNL Adobe Workfront] gli utenti possono consultare il catalogo dei progetti.

In qualità di amministratore di sistema, puoi effettuare le seguenti operazioni:

* Aggiungi [!UICONTROL Blueprint] al menu principale nei modelli di layout e assegna il modello di layout a utenti o gruppi. Per ulteriori informazioni, consulta [Personalizzare [!UICONTROL Menu principale] utilizzo di un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) e [Assegnare gli utenti a un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   >[!NOTE]
   >
   >* Gli utenti a cui non è stato assegnato un modello di layout visualizzeranno il [!UICONTROL Blueprint] nella [!UICONTROL Menu principale].
   >* Quando si crea un nuovo modello di layout, la [!UICONTROL Blueprint] è inclusa nella [!UICONTROL Elementi attivi] elenco per [!UICONTROL Menu principale] per impostazione predefinita.



* Abilita l’accesso per gli utenti per richiedere l’installazione dei progetti impostando una coda di richieste per archiviare le richieste. Qui, disponi di una singola posizione per monitorare e aggiornare le richieste. Per ulteriori informazioni, segui la procedura seguente.
* Installa i progetti. Per informazioni, consulta [Installare una blueprint](../../administration-and-setup/blueprints/blueprints-install.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano</strong></td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licenza</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisiti {#prerequisites}

* Devi utilizzare una coda di richiesta esistente per memorizzare le richieste di blueprint. Il progetto deve essere salvato come coda di richiesta e deve essere in [!UICONTROL Corrente] stato.
* La coda delle richieste deve essere pubblica. Nei dettagli della coda di richiesta, &quot;[!UICONTROL Chi può aggiungere richieste a questa coda?]&quot; deve essere impostato su **[!UICONTROL Chiunque]**.

>[!TIP]
>
>Per creare una nuova coda di richiesta per le richieste blueprint, è necessario generarla prima di configurare l’accesso alle blueprint. Per informazioni sulla creazione di una coda di richiesta, consulta [Creare una coda di richiesta](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Seleziona la coda di richiesta per memorizzare le richieste di blueprint

Prima che gli utenti possano richiedere l’installazione dei progetti, devi selezionare una coda di richiesta per tali richieste. Fino a quando la coda di richiesta non è definita, gli utenti possono solo sfogliare il catalogo delle blueprint.

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Blueprint]**.
1. Fai clic su **[!UICONTROL Configurare le richieste blueprint]** in alto a destra nella schermata del catalogo.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. Sulla **[!UICONTROL Configurare le blueprint]** inizia a digitare il nome di una coda di richiesta attiva e selezionala quando viene visualizzata nei risultati della ricerca.

   >[!IMPORTANT]
   >
   >In questo elenco vengono visualizzate solo le code di richiesta pubblica. Per rendere pubblica la coda di richiesta, vedi [Prerequisiti](#prerequisites) sezione precedente.

   La preferenza della coda di richiesta è impostata e gli utenti possono ora richiedere l’installazione blueprint.

   ![Configurare la coda di richiesta](assets/Blueprints_access_setup_request_queue.png)

1. (Facoltativo) Per apportare modifiche alla coda di richiesta effettiva, fai clic su **[!UICONTROL Modifica questa coda di richiesta]**.

   Il progetto della coda di richiesta si apre in una nuova scheda del browser ed è possibile aggiornarlo in base alle esigenze.

1. (Facoltativo) Se la coda di richiesta contiene gruppi di argomenti o argomenti della coda, puoi selezionarli dall’elenco.
1. Per tornare al catalogo blueprint, fai clic su **[!UICONTROL Chiudi]**.

>[!NOTE]
>
>Quando installi una blueprint richiesta, devi modificare lo stato del problema in **[!UICONTROL Chiuso]** o **[!UICONTROL Risolto]** nella coda delle richieste in modo che il richiedente venga informato. Per informazioni sull&#39;installazione di una blueprint, vedi [Installare una blueprint](../../administration-and-setup/blueprints/blueprints-install.md).
