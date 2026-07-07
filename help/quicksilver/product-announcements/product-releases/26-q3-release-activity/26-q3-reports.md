---
title: Miglioramenti al reporting per il terzo trimestre 2026
description: Miglioramenti al reporting per il terzo trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 0c7265c477030137d14e95f42eaf67580589d70b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 1%

---

# Miglioramenti al reporting per il terzo trimestre 2026

Questa pagina descrive i miglioramenti apportati all’ambiente di anteprima nella versione del terzo trimestre 2026 per la generazione di rapporti. Tali miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del terzo trimestre 2026, consulta [Panoramica sulla versione del terzo trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Controllo automatico dell&#39;accesso per Workfront Planning in Snowflake

>[!NOTE]
>
>Anteprima e produzione per tutti i clienti: 16 luglio 2026Fuori pianificazione&rbrack;{type=Neutral}

Questa versione introduce la gestione degli accessi automatizzata e basata sui diritti per i dati di Workfront Planning in Snowflake come parte di Workfront Data Connect.
Si inizia estendendo la generazione di viste sicure alle tabelle di Planning che stabiliscono le basi necessarie per il controllo degli accessi a valle e rendendo possibili le sovvenzioni basate sui diritti.Sulla base di questo, il provisioning dell’account di lettura ora controlla i diritti TMS al momento della creazione e applica automaticamente o trattiene le sovvenzioni al database Planning, garantendo la correttezza.
Prima di questo miglioramento, questo era disponibile solo per Workfront.
L’aggiornamento include le seguenti funzionalità: 

* Un processo giornaliero automatizzato rileva le modifiche di adesione per i clienti esistenti
* I nuovi job concedono, revocano o conservano l&#39;accesso in base ai diritti
* Copertura completa del ciclo di vita per provisioning, creazione di account e modifiche continue dei diritti.

L&#39;articolo del dizionario dati [Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md) verrà aggiornato dopo la data di rilascio.

## Aggiunta del supporto per dati personalizzati per nuovi oggetti

>[!NOTE]
>
>Anteprima e produzione per tutti i clienti: 7 luglio 2026Fuori pianificazione&rbrack;{type=Neutral}

Durante il secondo trimestre del 2026 sono stati aggiunti nuovi oggetti per supportare i miglioramenti delle operazioni aziendali in Workfront.Con la versione corrente, verrà aggiunto anche il supporto per dati personalizzati per diversi nuovi oggetti nel dashboard di Canvas.

Per informazioni, vedere [Panoramica del dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md).

## Impostazioni predefinite del prompt del dashboard di Canvas e persistenza delle preferenze utente

>[!NOTE]
>
>Anteprima: 25 giugno 2026Versione rapida di produzione: 15 luglio 2026Produzione per tutti: 16 luglio 2026

Per migliorare l’efficienza degli utenti che si spostano tra dashboard e record mantenendo il proprio stato di filtro funzionante, i responsabili dei dashboard possono ora definire valori di prompt predefiniti per i dashboard di Canvas. Queste impostazioni predefinite vengono applicate automaticamente a tutti i visualizzatori del dashboard.

Quando un utente aggiorna un messaggio di richiesta, le selezioni vengono salvate e ripristinate al momento dell’aggiornamento, della riapertura o dopo essere passato e tornato a un record.

I responsabili possono reimpostare lo stato predefinito del dashboard in qualsiasi momento. Gli utenti possono anche ripristinare rapidamente le impostazioni predefinite tramite il menu a tre punti.

Prima di questo miglioramento, i prompt del dashboard non disponevano di un valore predefinito configurabile o di una preferenza utente salvata per lo stato del prompt.

Per informazioni, vedere [Filtrare un dashboard Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md).

## Aggiungere più intervalli di indirizzi IP di Power BI al inserisco nell&#39;elenco Consentiti di connessione dati di un&#39;istanza di Windows (Data Connect) per volta

>[!NOTE]
>
>Anteprima: N/DVersione rapida di produzione: 11 giugno 2026Produzione per tutti: 16 luglio 2026

Gli amministratori di Workfront che collegano Microsoft Power BI a Workfront Data Connect ora possono aggiungere al inserisco nell&#39;elenco Consentiti di un intero set di intervalli di indirizzi IP di Azure in un unico passaggio. Nella scheda **Inserisco nell&#39;elenco Consentiti di IP** in **Connessione dati**, il pulsante **Nuovo indirizzo IP** ora include l&#39;opzione **Aggiungi blocchi di indirizzi IP Power BI** che consente di aprire una finestra di dialogo in cui è possibile incollare le voci dei tag di servizio Power BI dal file JSON degli intervalli IP e dei tag di servizio di Microsoft Azure pubblicati.

Questo sostituisce il flusso di lavoro precedente che prevedeva l’aggiunta di ogni blocco CIDR di Power BI uno alla volta, operazione che ha richiesto molto tempo per le aree in cui sono stati pubblicati decine di prefissi di indirizzi.

Per ulteriori informazioni, vedere [Stabilire una connessione a Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).


## Ordinare l’elenco delle dashboard dell’area di lavoro

>[!NOTE]
>
>Anteprima: 11 giugno 2026Versione rapida di produzione: 15 luglio 2026Produzione per tutti: 16 luglio 2026
>
>Canvas Dashboards è attualmente in versione beta.

È ora possibile ordinare l&#39;elenco dei dashboard di Canvas in base alle colonne seguenti: **Nome**, **Descrizione**, **Creato da** o **Data creazione**. Fare clic su un&#39;intestazione di colonna per ordinare l&#39;elenco in base a tale colonna, quindi fare di nuovo clic sulla stessa intestazione per invertire la direzione di ordinamento. Per impostazione predefinita, l&#39;elenco è ordinato per **Nome** dalla A alla Z. L’ordinamento viene mantenuto quando si passa da una scheda all’altra nell’elenco Dashboard di Canvas.

Per ulteriori informazioni, vedere [Utilizzare i dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Modifiche alle ore effettive nelle formule personalizzate

>[!NOTE]
>
>Anteprima: 1 giugno 2026Versione rapida di produzione: 1 giugno 2026Produzione per tutti: 1 giugno 2026

Nel 2025 è stato aggiunto al database di Workfront un nuovo campo Ore effettive come `actualWorkRequiredDouble` e il campo Ore effettive esistente (`actualWorkRequired` nel database) è stato rinominato Ore effettive legacy. Per ulteriori informazioni, consulta la [nota sulla versione](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md).

A giugno 2026, è stata effettuata la migrazione delle formule personalizzate esistenti che utilizzano `actualWorkRequired` (ore effettive legacy) per utilizzare `actualWorkRequiredDouble` (ore effettive). Impossibile utilizzare `actualWorkRequired` nei calcoli e nelle formule.

Inoltre, si consiglia vivamente di utilizzare `actualWorkRequiredDouble` in tutti i report.

Durante la sostituzione del campo, si noti che `actualWorkRequired` memorizza i valori in minuti, mentre `actualWorkRequiredDouble` memorizza i valori in ore con precisione decimale.

Per ulteriori informazioni sulle ore effettive, vedere [Visualizza ore effettive](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).

## Campi di dati valuta personalizzati nei rapporti del dashboard Area di lavoro

>[!NOTE]
>
>Anteprima: 28 maggio 2026Versione rapida di produzione: 11 giugno 2026Produzione per tutti: 16 luglio 2026

I rapporti del dashboard Canvas ora supportano campi di dati valuta personalizzati come colonne, filtri, raggruppamenti e aggregazioni, anche quando nella configurazione del sistema sono configurati più tassi di cambio. Quando un campo dati valuta personalizzato viene visualizzato come colonna o aggregazione, i valori vengono convertiti nella valuta selezionata nell’interruttore del tasso di cambio del dashboard, a meno che il campo non sia bloccato a livello di report.

Vengono ora visualizzati i rapporti che in precedenza non riuscivano con un messaggio di &quot;campo limitato&quot; dopo l’aggiunta di una seconda valuta del tasso di cambio. I campi della valuta di pianificazione rimangono limitati quando vengono definiti più tassi di cambio.

Per ulteriori informazioni, vedere [Utilizzare i campi di valuta nei dashboard di Canvas](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Miglioramento della precisione dei dati nei rapporti del dashboard di Canvas

>[!NOTE]
>
>Anteprima: 14 maggio 2026Versione rapida di produzione: 11 giugno 2026Produzione per tutti: 16 luglio 2026
>
>Canvas Dashboards è attualmente in versione beta.

I dashboard dell’area di lavoro ora strutturano le query dei rapporti in modo da evitare righe duplicate quando i filtri o i campi attraversano record correlati, in modo che i conteggi, le somme e altri aggregati restituiscano valori precisi.

In precedenza, un join tra record correlati poteva ripetere i record padre una volta per ogni record correlato. Ad esempio, in un report di progetto filtrato per le attività assegnate a un utente specifico, ogni progetto viene ripetuto una volta per ogni attività corrispondente. Un indicatore KPI con il budget del progetto sommato potrebbe mostrare 6.000 dollari invece dei 1.250 dollari corretti.

Non sono state apportate modifiche all’interfaccia del dashboard di Canvas. I rapporti esistenti restituiscono automaticamente dati precisi dopo questa versione.

