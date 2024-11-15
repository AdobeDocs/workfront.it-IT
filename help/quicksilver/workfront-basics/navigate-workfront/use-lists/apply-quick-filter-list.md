---
navigation-topic: use-lists
title: Applicare il filtro rapido a un elenco
description: È possibile utilizzare il filtro rapido in un elenco di oggetti per individuare solo gli elementi importanti, in modo da poterli esaminare, aggiornare o condividere rapidamente con altri utenti.
feature: Get Started with Workfront
author: Nolan
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 261ac44eb0d13ffbd61a2c70213adb591bf018aa
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Applicare il filtro rapido a un elenco

<!--Audited:11/2024-->

È possibile utilizzare il filtro rapido in un elenco di oggetti per individuare solo gli elementi importanti, in modo da poterli esaminare, aggiornare o condividere rapidamente con altri utenti.

>[!IMPORTANT]
>
>Puoi trovare gli elementi che contengono una parola da cercare utilizzando i filtri rapidi, sia che l’elemento sia stato fisicamente visualizzato sullo schermo o che verrà visualizzato dopo lo scorrimento alla parte inferiore della pagina. Quando utilizzi le funzionalità di ricerca del browser, puoi trovare solo gli elementi fisicamente visualizzati sullo schermo. Se l’elenco contiene più pagine, i filtri rapidi non individuano gli elementi presenti nelle pagine che non vengono visualizzate.

Se desideri salvare un filtro rapido, ti consigliamo invece di creare un filtro permanente per l’elenco.\
Per informazioni su come creare filtri in [!DNL Adobe Workfront], vedere l&#39;articolo [Panoramica sui filtri](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Il filtro rapido è attualmente disponibile nelle seguenti aree


È possibile utilizzare filtri rapidi temporanei in tutti gli elenchi, ad eccezione dei seguenti:

* Area [!UICONTROL Report]
* Elenchi e report di documenti
* Diverse [!UICONTROL aree di installazione]

  >[!NOTE]
  >
  >I filtri rapidi sono disponibili nelle seguenti aree di installazione: [!UICONTROL Gruppi], [!UICONTROL Team], [!UICONTROL Società], [!UICONTROL Pianificazioni], [!UICONTROL Modelli layout] e [!UICONTROL Forms personalizzato].


Quando si applicano filtri rapidi a un elenco, considera quanto segue:

* È possibile utilizzare le parole chiave per filtrare qualsiasi campo visualizzato nella visualizzazione dell&#39;elenco. Ciò include campi personalizzati o campi complessi come [!UICONTROL Predecessori], [!UICONTROL Assegnazioni], [!UICONTROL Assegnazione] e [!UICONTROL Stato], [!UICONTROL Approvatore] e [!UICONTROL Stato], ecc.
* Se l’elenco contiene raggruppamenti compressi, questi vengono espansi automaticamente quando si utilizzano i filtri rapidi. Quando si rimuove il filtro rapido, i raggruppamenti vengono nuovamente compressi.
* I raggruppamenti mantengono le informazioni aggregate dell&#39;elenco originale indipendentemente dai filtri rapidi applicati o dalle modifiche apportate agli oggetti dell&#39;elenco.
* I filtri rapidi sono temporanei. Se si modifica il raggruppamento, la visualizzazione, il filtro o l&#39;ordinamento dell&#39;elenco, verranno rimossi i criteri di filtro rapido.
* Impossibile salvare un filtro rapido. Se desideri salvare un filtro per utilizzarlo nuovamente, puoi creare un filtro permanente per l’elenco.
* Se nell&#39;elenco sono presenti più raggruppamenti e il filtro rapido trova gli elementi in un solo raggruppamento, viene visualizzato solo tale raggruppamento con gli elementi trovati. Tutti gli altri raggruppamenti sono nascosti.
* In un elenco di attività o sottoattività, la gerarchia delle attività viene rimossa quando vengono visualizzati i risultati del filtro rapido.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
    <p>Nuovo:</p>
   <ul><li><p>Collaboratore o versione successiva </p></li>
   </ul>

<p>Corrente:</p>
   <ul><li><p>Richiedi o superiore</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione all'area in cui si trova l'elenco</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Autorizzazioni di [!UICONTROL View] per l'oggetto in cui si trova l'elenco</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Applicare un filtro rapido a un elenco

1. Vai a un elenco o a un report che supporta i filtri rapidi, quindi fai clic sull&#39;icona **[!UICONTROL Filtro rapido]** ![](assets/qs-quick-filter-icon.png) nella barra degli strumenti.

   Oppure

   A seconda del sistema operativo o del browser in uso e quando si utilizza una tastiera QWERTY standard, premere il seguente set di comandi per avviare il filtro rapido:

   * ALT+F per [!DNL Windows] computer
   * ALT/ Opzione+F per [!DNL Mac] computer

     >[!TIP]
     >
     >Se si preme CTRL+F o CMD+F, accanto al filtro rapido viene visualizzata una descrizione comando che ricorda questi comandi. I comandi vengono visualizzati anche all&#39;interno della casella di ricerca del filtro rapido.

1. Nella casella **[!UICONTROL Filtra pagina]** immettere la parola chiave in base alla quale si desidera filtrare.

   È possibile utilizzare qualsiasi parola visualizzata nella visualizzazione dell&#39;elenco.

   >[!NOTE]
   >
   >Se utilizzi una parola che potrebbe essere visualizzata in un’altra pagina dell’elenco, il filtro rapido non trova alcun risultato.

   Un elenco di elementi che corrispondono ai criteri di ricerca viene visualizzato dinamicamente durante la digitazione e tutti gli altri elementi vengono nascosti. La parola chiave utilizzata nella ricerca viene evidenziata in giallo in tutti i campi autonomi e complessi. Alcuni esempi di campi complessi sono colonne condivise o uno dei seguenti: [!UICONTROL Assegnazioni], [!UICONTROL Assegnazioni] e [!UICONTROL Stato], [!UICONTROL Percentuale Completata], [!UICONTROL Predecessori], [!UICONTROL Approvatori e Stato], [!UICONTROL Responsabili risorse], [!UICONTROL Categorie], [!UICONTROL Condizione], [!UICONTROL Aggiornamento condizione], ecc.

1. (Facoltativo) Per modificare in blocco gli elementi trovati dal filtro rapido:

   1. Seleziona tutti o alcuni elementi dell&#39;elenco, quindi fai clic su **[!UICONTROL Modifica]** per modificare gli elementi in blocco.
   1. Dopo aver completato le modifiche, fai clic su **[!UICONTROL Salva modifiche]**.

1. (Facoltativo) Per esportare gli elementi trovati dal filtro rapido, selezionare tutti o alcuni elementi nell&#39;elenco, quindi fare clic sull&#39;icona **[!UICONTROL Esporta]** ![](assets/export.png).

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Solo gli elementi trovati nell&#39;esportazione di ricerca a filtro rapido vengono esportati nel file selezionato. Se non si selezionano elementi prima di esportare l&#39;elenco, verrà esportato l&#39;elenco completo non filtrato.\
   >Per ulteriori informazioni, vedere [Esportare un elenco](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Facoltativo) Per cancellare i risultati filtrati, fai clic sull&#39;icona **[!UICONTROL Filtro rapido]** nell&#39;angolo in alto a destra della finestra.
Oppure
Aggiorna la pagina.
