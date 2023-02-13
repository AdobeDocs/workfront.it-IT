---
navigation-topic: use-lists
title: Applicare il filtro rapido a un elenco
description: È possibile utilizzare il filtro rapido in un elenco di oggetti per individuare solo gli elementi importanti per l’utente, in modo da poterli rivedere, aggiornare o condividere rapidamente con altri utenti.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# Applicare il filtro rapido a un elenco

<!--
{{highlighted-preview}}
-->

È possibile utilizzare il filtro rapido in un elenco di oggetti per individuare solo gli elementi importanti per l’utente, in modo da poterli rivedere, aggiornare o condividere rapidamente con altri utenti.

>[!IMPORTANT]
>
>È possibile trovare elementi che contengono una parola di ricerca utilizzando filtri rapidi, indipendentemente dal fatto che l’elemento sia stato fisicamente visualizzato sullo schermo o venga visualizzato dopo lo scorrimento nella parte inferiore della pagina. Quando utilizzi le funzionalità di ricerca del browser, puoi trovare solo gli elementi fisicamente visualizzati sullo schermo. Se l’elenco include più pagine, i filtri rapidi non individuano gli elementi presenti nelle pagine che non vengono visualizzati.

Per salvare un filtro rapido, è consigliabile creare un filtro permanente per l’elenco.\
Per informazioni su come creare i filtri in [!DNL Adobe Workfront], vedi l&#39;articolo [Panoramica dei filtri in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Il filtro rapido è attualmente disponibile nelle seguenti aree


È possibile utilizzare filtri rapidi temporanei in tutti gli elenchi, fatta eccezione per quanto segue:

* La [!UICONTROL Rapporti] area
* Elenchi di documenti e rapporti
* Diversi [!UICONTROL Configurazione] aree
   >[!NOTE]
   >
   >I filtri rapidi sono disponibili nelle seguenti aree di configurazione: [!UICONTROL Gruppi], [!UICONTROL Team], [!UICONTROL Aziende], [!UICONTROL Pianificazioni], [!UICONTROL Modelli di layout]e [!UICONTROL Forms personalizzato].


Quando si applicano filtri rapidi a un elenco, tenere presente quanto segue:

* È possibile utilizzare le parole chiave per filtrare qualsiasi campo visualizzato nella visualizzazione dell’elenco. Sono inclusi campi personalizzati o campi complessi come [!UICONTROL Predecessori], [!UICONTROL Assegnazioni], [!UICONTROL Assegnazione] e [!UICONTROL Stato], [!UICONTROL Approvatore] e [!UICONTROL Stato], ecc.
* Se l’elenco contiene raggruppamenti compressi, questi vengono espansi automaticamente quando si utilizzano filtri rapidi. Quando si rimuove il filtro rapido, i raggruppamenti vengono nuovamente compressi.
* I raggruppamenti conservano le informazioni aggregate dell’elenco originale indipendentemente dai filtri rapidi applicati o da eventuali modifiche apportate agli oggetti dell’elenco.
* I filtri rapidi sono temporanei. La modifica del raggruppamento, della visualizzazione, del filtro o dell’ordinamento dell’elenco comporta la rimozione dei criteri di filtro rapido.
* Non è possibile salvare un filtro rapido. Per salvare un filtro per utilizzarlo nuovamente, è consigliabile creare un filtro permanente per l’elenco.
* Se nell’elenco sono presenti più raggruppamenti e il filtro rapido trova gli elementi in un solo raggruppamento, viene visualizzato solo quel raggruppamento con gli elementi trovati. Tutti gli altri raggruppamenti sono nascosti.
* In un elenco di attività o sottoattività, la gerarchia delle attività viene rimossa quando vengono visualizzati i risultati del filtro rapido.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] piano*</b></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] licenza*</b></td> 
   <td> <p>[!UICONTROL Request] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Configurazioni a livello di accesso*</b></td> 
   <td> <p>Visualizza l'accesso all'area in cui si trova l'elenco</p> <p>Ad esempio, per applicare un filtro rapido a un progetto, è necessario disporre dell’accesso alla visualizzazione Progetti.</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso.<br>Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Autorizzazioni oggetto</b></td> 
   <td> <p>[!UICONTROL View]</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Applicazione di un filtro rapido a un elenco

1. Passa a un elenco o a un rapporto che supporta i filtri rapidi, quindi fai clic sul pulsante **[!UICONTROL Filtro rapido] icona** ![](assets/qs-quick-filter-icon.png) nella barra degli strumenti.

   Oppure

   A seconda del sistema operativo o del browser in uso e quando si utilizza una tastiera QWERTY standard, premere il seguente set di comandi per avviare il filtro rapido:

   * ALT+F per [!DNL Windows] computer
   * ALT/Opzione+F per [!DNL Mac] computer

      >[!TIP]
      >
      >Se si preme CTRL+F o CMD+F, accanto al filtro rapido viene visualizzata una descrizione comandi che ricorda questi comandi. I comandi vengono visualizzati anche all’interno della casella di ricerca del filtro rapido.

1. In **[!UICONTROL Filtra pagina]** immettere la parola chiave per cui si desidera filtrare.

   È possibile utilizzare qualsiasi parola attualmente visualizzata nella visualizzazione dell’elenco.

   >[!NOTE]
   >
   >Se utilizzi una parola che potrebbe essere visualizzata in un’altra pagina dell’elenco, il filtro rapido non rileva alcun risultato.

   Un elenco di elementi che corrispondono ai criteri di ricerca viene visualizzato nell’elenco in modo dinamico durante la digitazione e tutti gli altri elementi sono nascosti. La parola chiave utilizzata nella ricerca viene evidenziata in giallo in tutti i campi indipendenti e complessi. Alcuni esempi di campi complessi sono colonne condivise o uno dei seguenti elementi: [!UICONTROL Assegnazioni], [!UICONTROL Assegnazioni] e [!UICONTROL Stato], [!UICONTROL Percentuale completata], [!UICONTROL Predecessori], [!UICONTROL Approvatori e stato], [!UICONTROL Manager risorse], [!UICONTROL Categorie], [!UICONTROL Condizione], [!UICONTROL Aggiornamento delle condizioni], ecc.

1. (Facoltativo) Per modificare in serie gli elementi trovati dal filtro rapido:

   1. Seleziona tutti o più elementi dell’elenco, quindi fai clic su **[!UICONTROL Modifica]** per modificare in blocco gli elementi.
   1. Dopo aver completato le modifiche, fai clic su **[!UICONTROL Salva modifiche]**.

1. (Facoltativo) Per esportare gli elementi trovati dal filtro rapido, seleziona tutti o più elementi nell’elenco, quindi fai clic su **[!UICONTROL Esporta]**.

   ![select_all_projects_with_highlight_1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Solo gli elementi trovati nell’esportazione di ricerca filtro rapido nel file selezionato. Se non selezionate alcun elemento prima di esportare l’elenco, viene esportato l’elenco completo e non filtrato.\
   >Per ulteriori informazioni, consulta [Esportare un elenco](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Facoltativo) Per cancellare i risultati filtrati, fai clic sul pulsante **[!UICONTROL Filtro rapido]** nell’angolo in alto a destra della finestra.\
   Oppure\
   Aggiorna la pagina.
