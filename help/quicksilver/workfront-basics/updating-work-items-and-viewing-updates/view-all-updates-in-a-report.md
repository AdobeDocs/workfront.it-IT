---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visualizzare tutti gli aggiornamenti in un report Nota
description: Visualizzare tutti gli aggiornamenti in un report Nota
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 158af1f48fba264b98108b5f0a573b7904eb875e
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 1%

---

# Visualizzare tutti gli aggiornamenti in un report Nota

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Per impostazione predefinita, nell&#39;area Aggiornamenti di un oggetto viene visualizzato un numero massimo di 200 aggiornamenti. Per visualizzare tutti gli aggiornamenti inseriti da un utente per un oggetto, è possibile creare un report di note che visualizza tutti gli aggiornamenti.

>[!NOTE]
>
>È possibile creare un report per visualizzare gli aggiornamenti sugli oggetti in Anteprima con il report Voce diario. Per ulteriori informazioni, vedere [Report sull&#39;area Aggiornamenti con un report sulle voci diario](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>piano Adobe Workfront</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licenza Adobe Workfront*</strong></td> 
   <td> <p>Nuovo: Standard </p>
   <p>Corrente: Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Creare rapporti, dashboard e calendari</p> </li> 
     <li> <p>Creare filtri, visualizzazioni e raggruppamenti</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizza</p> <p><b>NOTA</b></p>
   <p>Se non si dispone dell'autorizzazione di visualizzazione o di un'autorizzazione successiva per un oggetto, le informazioni relative a tale oggetto non vengono visualizzate nel report.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, vedere [Requisiti di accesso in Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creare un rapporto di nota

La creazione di un report per Notes per qualsiasi oggetto è identica, indipendentemente dall&#39;oggetto.

Ad esempio, per creare un rapporto Note per tutte le note di un progetto:

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront.

1. Fai clic su **Rapporti**.
1. Fai clic su **Nuovo rapporto**, quindi scegli **Nota**.

1. (Facoltativo) Fai clic su **Viste**, quindi su **Aggiungi colonna** per aggiungere **Nome** del **Progetto** alla visualizzazione del report. 

1. (Facoltativo) Fai clic su **Raggruppamenti**, quindi su **Aggiungi raggruppamento** per raggruppare in base al **Nome progetto**, se esegui report su più progetti contemporaneamente.\
   In questo modo le note vengono raggruppate in base ai rispettivi progetti, facilitando la lettura del rapporto. 

1. (Facoltativo) Fai clic su **Filtri,** quindi su **Aggiungi regola filtro**.
1. Aggiungi un filtro per **Nota** > **Testo nota** > **Non è vuoto**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Se un campo di progetto è stato aggiornato ma non è stata aggiunta alcuna nota al momento dell&#39;aggiornamento, il **Testo nota** dell&#39;aggiornamento verrà visualizzato come **(Nessun testo aggiunto da aggiornare)**.


1. (Facoltativo) Aggiungi un altro filtro per **Progetto** > **Nome** > **È uguale a** e aggiungi uno o più nomi di progetto per i quali vuoi visualizzare le note.
1. Fai clic su **Salva e Chiudi**.\
   Nel rapporto vengono visualizzati tutti gli aggiornamenti immessi nel progetto da tutti gli utenti con autorizzazioni almeno per Visualizza il progetto.
