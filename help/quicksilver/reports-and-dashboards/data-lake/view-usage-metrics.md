---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Visualizzare le metriche di utilizzo di Workfront Data Connect
description: Utilizzando la scheda Metriche di Workfront Data Connect, puoi visualizzare le metriche di utilizzo della tua organizzazione in base sia alle ore di calcolo mensili utilizzate che al numero di query eseguite.
author: Nolan
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
source-git-commit: 7764e512a3fb30a89e6645a4d8544a5fcffee231
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# Visualizza metriche di utilizzo [!DNL Workfront Data Connect]

Utilizzando la scheda [!DNL Workfront Data Connect] [!UICONTROL Metriche], puoi visualizzare le metriche di utilizzo della tua organizzazione in base sia alle ore di calcolo utilizzate che al numero di query eseguite. Le organizzazioni dispongono di un numero limitato di ore di calcolo mensili in base al tipo di licenza e agli acquisti del componente aggiuntivo Data Connect. La scheda [!UICONTROL Metriche] visualizza informazioni sulle ore di calcolo mensili disponibili in relazione agli elementi utilizzati.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Flusso di lavoro Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare le metriche di utilizzo e le ore di calcolo disponibili

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon.png) nell&#39;angolo superiore destro di Adobe Workfront oppure, se disponibile, fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) nell&#39;angolo superiore sinistro, quindi fai clic su [!UICONTROL **Setup**].

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Sistema**] > [!UICONTROL **Accesso ai dati**].

1. Fai clic sulla scheda [!UICONTROL **Metriche**]. Le metriche di utilizzo vengono visualizzate nel grafico **Utilizzo calcolo**, mentre il numero di query eseguite viene visualizzato nel grafico **Conteggio query**.

   ![Metriche di utilizzo di Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. (Facoltativo) È possibile utilizzare il menu a discesa [!UICONTROL **Seleziona una visualizzazione**] per modificare l&#39;intervallo di tempo per le informazioni incluse in entrambi i grafici.

1. (Facoltativo) Puoi utilizzare le caselle di controllo sopra il grafico **Utilizzo calcolato** per mostrare o nascondere:
   * [!UICONTROL **Ore di calcolo giornaliere**] - Numero di ore di calcolo utilizzato dall&#39;organizzazione su base giornaliera.
   * [!UICONTROL **Ore di calcolo cumulative mensili**] - Numero totale di ore di calcolo utilizzate dall&#39;organizzazione in un mese. Viene ripristinato a zero ogni mese.
   * [!UICONTROL **Indennità mensile ore di calcolo**]: il numero di ore di calcolo disponibili per l&#39;organizzazione in base agli acquisti di licenze e/o componenti aggiuntivi.
