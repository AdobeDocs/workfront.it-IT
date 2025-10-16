---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filtro: rapporto Approvazione bozza per omettere le versioni di bozza precedenti'
description: In un rapporto Proof Approval (Approvazione bozza) è possibile utilizzare il filtro Is Current Document Version (È versione corrente del documento) per includere solo le versioni correnti delle bozze in attesa di approvazione.
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Filtro: rapporto Proof Approval (Approvazione della bozza) per omettere le versioni precedenti della bozza

<!--Audited: 10/2024-->

In un report Proof Approval (Approvazione bozza) è possibile utilizzare il filtro **Is Current Document Version** (È la versione corrente del documento) per includere solo le versioni correnti delle bozze in attesa della propria approvazione.

Ciò è utile, ad esempio, se ti è stato chiesto di approvare bozze che hanno più versioni. Quando si esegue il rapporto Proof Approval (Approvazione della bozza) con il filtro Is Current Document Version (È versione corrente del documento), nel rapporto viene elencata solo la versione corrente di ogni bozza in attesa di approvazione, omettendo le versioni precedenti su cui non è più necessario lavorare.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o richiesta di modifica di un filtro </p>
   <p>Standard o piano per modificare un rapporto</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrare il rapporto Proof Approval (Approvazione della bozza) per omettere le versioni precedenti della bozza

Puoi creare un filtro per un rapporto Proof Approval (Approvazione della bozza).

1. Se disponi già di un rapporto Proof Approval (Approvazione della bozza), aprilo.

   Oppure

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Per creare un report Proof Approval personalizzato, fai clic sull&#39;icona **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro o sull&#39;icona **Main Menu** ![Main Menu lines](assets/lines-main-menu.png) nell&#39;angolo superiore sinistro, se disponibile, quindi fai clic su **Reports** ![Reports icon](assets/reports-in-main-menu.png).

1. Fare clic su **Nuovo report**. Viene visualizzato l&#39;elenco dei tipi di oggetto.
1. Fare clic su **Approvazione bozza** nell&#39;elenco.
Viene aperto Report Builder (Generatore report).
1. Fai clic su **Filtri**, quindi fai clic su **Aggiungi una regola filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Fai clic nella casella **Imposta regole filtro per il report**, quindi seleziona **Approvazione bozza** dall&#39;elenco.
1. Fare clic su **Is Current Document Version** nell&#39;elenco dell&#39;oggetto **Proof Approval**.
1. Scegliere Uguale per il modificatore di filtro, quindi selezionare True.
1. Fai clic su **Salva + Chiudi** nell&#39;angolo inferiore sinistro di Adobe Workfront, quindi fai clic su **Applica** nella casella visualizzata.

   Nel rapporto Proof Approval (Approvazione bozza) vengono visualizzate solo le bozze associate alle versioni correnti di qualsiasi documento, se le approvazioni di bozza corrispondono a questi criteri di filtro.
