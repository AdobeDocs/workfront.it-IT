---
navigation-topic: use-lists
title: Applicare il filtro rapido a un elenco
description: Potete usare il filtro rapido in un elenco di oggetti per individuare solo gli elementi che sono importanti per voi, in modo da poterli esaminare, aggiornare o condividere rapidamente con altri utenti.
feature: Get Started with Workfront
author: Courtney
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 5%

---

# Applicare il filtro rapido a un elenco

<!--Audited:11/2024-->

Potete usare il filtro rapido in un elenco di oggetti per individuare solo gli elementi che sono importanti per voi, in modo da poterli esaminare, aggiornare o condividere rapidamente con altri utenti.

>[!IMPORTANT]
>
>È possibile trovare elementi che contengono una parola da ricercare utilizzando i filtri rapidi, sia che l&#39;elemento sia stato fisicamente visualizzato sullo schermo o che verrà visualizzato dopo lo scorrimento nella parte inferiore della pagina. Quando si utilizzano le funzionalità di ricerca del browser, è possibile trovare solo gli elementi fisicamente visualizzati sullo schermo. Se l’elenco contiene più pagine, i filtri rapidi non consentono di trovare gli elementi presenti nelle pagine che non vengono visualizzate.

Se si desidera salvare un filtro rapido, è consigliabile creare un filtro permanente per l&#39;elenco.\
Per informazioni su come compilare i filtri in [!DNL Adobe Workfront], vedere l&#39;articolo [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Il filtro rapido è attualmente disponibile nelle seguenti aree


Potete usare filtri rapidi temporanei in tutti gli elenchi, eccetto i seguenti:

* Area [!UICONTROL Report]
* Elenchi di documenti e report
* Diverse aree [!UICONTROL Configurazione]

  >[!NOTE]
  >
  >I filtri rapidi sono disponibili nelle seguenti aree di installazione: [!UICONTROL Gruppi], [!UICONTROL Team], [!UICONTROL Società], [!UICONTROL Pianificazioni], [!UICONTROL Modelli layout] e [!UICONTROL Forms personalizzato].


Quando si applicano filtri rapidi a un elenco, considera quanto segue:

* È possibile utilizzare le parole chiave per filtrare qualsiasi campo visualizzato nella visualizzazione dell&#39;elenco. Ciò include campi personalizzati o complessi come [!UICONTROL Predecessori], [!UICONTROL Assegnazioni], [!UICONTROL Assegnazione] e [!UICONTROL Stato], [!UICONTROL Approvatore] e [!UICONTROL Stato], ecc.
* Se l’elenco contiene raggruppamenti compressi, questi vengono espansi automaticamente quando utilizzate i filtri rapidi. Quando rimuovete il filtro rapido, i raggruppamenti vengono compressi di nuovo.
* I raggruppamenti conservano le informazioni aggregate dell&#39;elenco originale indipendentemente dai filtri rapidi applicati o dalle modifiche apportate agli oggetti nell&#39;elenco.
* I filtri rapidi sono temporanei. Se si modifica il raggruppamento, la visualizzazione, il filtro o l&#39;ordinamento dell&#39;elenco, vengono rimossi i criteri del filtro rapido.
* Non è possibile salvare un filtro rapido. Se si desidera salvare un filtro per riutilizzarlo, è consigliabile creare un filtro permanente per l&#39;elenco.
* Se nell&#39;elenco sono presenti più raggruppamenti e il filtro rapido trova elementi in un solo raggruppamento, solo tale raggruppamento viene visualizzato con gli elementi trovati. Tutti gli altri raggruppamenti sono nascosti.
* In un elenco di attività o sottoattività, la gerarchia delle attività viene rimossa quando vengono visualizzati i risultati del filtro rapido.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo. 

Per eseguire i passaggi descritti in questo articolo, devi disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
    <p>Novità:</p>
   <ul><li><p>Collaboratore o successiva </p></li>
   </ul>

<p>Corrente:</p>
   <ul><li><p>Richiedente o successiva</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione all'area in cui si trova l'elenco</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Autorizzazioni di [!UICONTROL View] per l'oggetto in cui si trova l'elenco</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Applicare un filtro rapido a un elenco

1. Accedi a un elenco o a un report che supporta i filtri rapidi, quindi fai clic sull&#39;icona **[!UICONTROL Filtro rapido]** ![Icona Filtro rapido](assets/qs-quick-filter-icon.png) nella barra degli strumenti.

   Oppure

   A seconda del sistema operativo o del browser utilizzato e quando si utilizza una tastiera QWERTY standard, premere il seguente set di comandi per avviare il filtro rapido:

   * ALT+F per [!DNL Windows] computer
   * ALT/Opzione+F per [!DNL Mac] computer

     >[!TIP]
     >
     >Se si preme CTRL+F o CMD+F, accanto al filtro rapido viene visualizzata una descrizione che ricorda tali comandi. I comandi vengono visualizzati anche all’interno della casella di ricerca del filtro rapido.

1. Nella casella **[!UICONTROL Pagina filtro]** immettere la parola chiave in base alla quale si desidera filtrare.

   È possibile utilizzare qualsiasi parola attualmente visualizzata nell&#39;elenco.

   >[!NOTE]
   >
   >Se si utilizza una parola che potrebbe essere visualizzata in un&#39;altra pagina dell&#39;elenco, il filtro rapido non rileva alcun risultato.

   Un elenco di elementi che corrispondono ai criteri di ricerca viene visualizzato dinamicamente durante la digitazione e tutti gli altri elementi vengono nascosti. La parola chiave utilizzata nella ricerca viene evidenziata in giallo in tutti i campi autonomi e complessi. Alcuni esempi di campi complessi sono colonne condivise o uno dei seguenti: [!UICONTROL Assegnazioni], [!UICONTROL Assegnazioni] e [!UICONTROL Stato], [!UICONTROL Percentuale completata], [!UICONTROL Predecessori], [!UICONTROL Approvatori e stato], [!UICONTROL Responsabili risorse], [!UICONTROL Categorie], [!UICONTROL Condizione], [!UICONTROL Aggiornamento condizione] e così via.

1. (Facoltativo) Per modificare in blocco gli elementi trovati dal filtro rapido:

   1. Seleziona tutti o alcuni elementi dell&#39;elenco, quindi fai clic su **[!UICONTROL Modifica]** per modificare gli elementi in blocco.
   1. Dopo aver completato le modifiche, fai clic su **[!UICONTROL Salva modifiche]**.

1. (Facoltativo) Per esportare gli elementi trovati dal filtro rapido, selezionate tutti o alcuni elementi dell&#39;elenco, quindi fate clic sull&#39;icona **[!UICONTROL Esporta]** ![Icona Esporta](assets/export.png).

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Solo gli elementi trovati nella ricerca del filtro rapido vengono esportati nel file selezionato. Se non selezionate alcuna voce prima di esportare l’elenco, viene esportato l’elenco completo, non filtrato.\
   >Per ulteriori informazioni, vedere [Esportare un elenco](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Facoltativo) Per cancellare i risultati filtrati, fare clic sull&#39;icona **[!UICONTROL Filtro rapido]** nell&#39;angolo superiore destro della finestra.
Oppure
Aggiorna la pagina.
