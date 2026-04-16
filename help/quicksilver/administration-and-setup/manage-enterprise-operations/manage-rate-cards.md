---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Gestisci schede tariffa
description: Una scheda tariffa rappresenta l’accordo contrattuale con il cliente in cui vengono definite le tariffe orarie per le mansioni che completeranno il lavoro. In una scheda tariffa è possibile definire più tariffe di fatturazione per mansione, in base agli attributi.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 2%

---

# Gestire le schede tariffa

Una scheda tariffa rappresenta l’accordo contrattuale con il cliente in cui vengono definite le tariffe orarie per le mansioni che completeranno il lavoro. In una scheda tariffa è possibile definire più tariffe di fatturazione per mansione, in base ad attributi quali agenzia, ubicazione o centro di costo. Gli attributi univoci della tariffa sono configurati nell’area Configura. Per ulteriori informazioni, vedere [Definire gli attributi del tasso](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

Ad esempio, potresti avere un ruolo di Designer con sede a Parigi per l’Agenzia A, un altro Designer con sede a Parigi per l’Agenzia B e un terzo Designer con sede a New York non assegnato a un’agenzia, ciascuno con tariffe di fatturazione diverse. Tuttavia, gli attributi non sono necessari per le mansioni su una scheda tariffa. Gli attributi fungono da strumenti per stabilire tassi più granulari. Una tariffa di fatturazione su una scheda tariffa può anche essere data di validità, in modo che la tariffa inizi e termini in date specificate.

Puoi anche bloccare le tariffe su una scheda delle tariffe per evitare che vengano ignorate a livello di progetto o di attività. Le tariffe bloccate sono le più alte nella gerarchia delle tariffe di fatturazione, ad eccezione delle tariffe mantenute su un progetto. Per ulteriori informazioni, vedere [Panoramica sulla gerarchia dei ricavi e dei costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td>Flusso di lavoro Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica accesso a [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Per modificare una scheda delle tariffe condivisa con te, devi disporre delle autorizzazioni di gestione per tale scheda.</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungi una scheda tariffa

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Fai clic su [!UICONTROL **Nuova scheda**], quindi fai clic su [!UICONTROL **Crea nuova scheda**].
1. Digitare un nome e una descrizione per la scheda tariffe nella casella [!UICONTROL **Nuova scheda tariffe**].

   Il nome deve essere univoco.

   ![Finestra di dialogo Nuova scheda tariffe](assets/new-rate-card-dialog.png)

1. (Facoltativo) Seleziona un [!UICONTROL **Gruppo**] per la scheda della tariffa. Questa è l&#39;agenzia che definisce la scheda tariffaria.
1. (Facoltativo) Seleziona una [!UICONTROL **società**] per la scheda tariffa. Questo è il cliente per il quale sono state stipulate le tariffe.

   >[!NOTE]
   >
   >Il Gruppo e l’Azienda vengono utilizzati non solo nei dettagli della scheda tariffa, ma anche come filtri quando si allega una scheda tariffa a un progetto.

1. Fai clic su **Crea**.

   Viene visualizzata la schermata Scheda tariffa > Ruoli e tariffe.

1. Fai clic su [!UICONTROL **Aggiungi mansione**].
1. Nella casella [!UICONTROL **Nuova tariffa di fatturazione**], seleziona una [!UICONTROL **mansione**] per definire le tariffe di fatturazione.

   ![Finestra di dialogo Nuova tariffa di fatturazione](assets/new-job-role-rate-on-rate-card.png)

1. (Facoltativo) Selezionare gli attributi per la tariffa di fatturazione, ad esempio Agenzia, Ubicazione o Centro di costo.

   >[!NOTE]
   >
   >Questi attributi vengono definiti separatamente e possono influire sui calcoli dei ricavi e dei costi. Per ulteriori informazioni, vedere [Definire gli attributi del tasso](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Seleziona una [!UICONTROL **Valuta**] per la tariffa di fatturazione.
1. (Facoltativo) Immetti un alias [!UICONTROL **per la mansione**].

   Se il nome dell&#39;alias digitato non esiste già, è possibile aggiungerlo.

   Quando la scheda tariffa è collegata a un progetto, l&#39;alias viene visualizzato in informazioni quali assegnazioni segnaposto, spese e rapporti, anziché nel nome della mansione interna.

   >[!NOTE]
   >
   >* Può esistere un solo alias per ogni mansione e combinazione di attributi all&#39;interno di una singola scheda tariffa.
   >* Un alias deve essere aggiornato nella scheda tariffa e non può essere modificato in un progetto.

1. Nel campo [!UICONTROL **Tariffa di fatturazione**] immettere la tariffa di fatturazione per questa mansione e i relativi attributi.
1. (Facoltativo) Seleziona [!UICONTROL **Frequenza di blocco**] per bloccare questa frequenza e non consentirne la modifica a livello di progetto o di attività. Se necessario, puoi sbloccarlo in un secondo momento.
1. (Facoltativo) Fai clic su [!UICONTROL **Aggiungi data tariffa effettiva**] per applicare le date di validità alla tariffa di fatturazione.
1. (Facoltativo) Fai clic di nuovo su [!UICONTROL **Aggiungi tariffa effettiva data**] per aggiungere altre tariffe di fatturazione con date di validità per questa mansione e i relativi attributi.
1. (Condizionale) Se si stanno aggiungendo più tariffe di fatturazione per questa mansione, inserire le seguenti informazioni:

   * [!UICONTROL **Tariffa di fatturazione**]: il valore della tariffa di fatturazione per il periodo di tempo.
   * [!UICONTROL **Data inizio**]: la data di inizio della tariffa.
   * [!UICONTROL **Data di fine**]: la data in cui termina la tariffa.

     La prima tariffa di fatturazione non deve avere una data di inizio e l’ultima tariffa di fatturazione non deve avere una data di fine. Sono consentiti intervalli tra le date del tasso, ma non sono consentite date sovrapposte. Durante un intervallo, altre aree della gerarchia delle tariffe di fatturazione vengono utilizzate per determinare la tariffa di fatturazione, in base al tipo di ricavi di un&#39;attività. Per ulteriori informazioni, vedere [Panoramica sulla gerarchia dei ricavi e dei costi](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

1. Fai clic su [!UICONTROL **Salva**].
1. (Facoltativo) Per aggiungere un&#39;altra tariffa di fatturazione, per la stessa mansione con attributi diversi o per una mansione separata, fare clic su [!UICONTROL **Aggiungi mansione**].

   Le tariffe per ogni ruolo vengono aggiunte alla scheda delle tariffe durante la creazione. Il tasso di validità corrente, basato sulle date, è indicato con l&#39;icona ![Icona tasso corrente](assets/current-rate-icon.png).

   ![Scheda tariffe con tariffe visualizzate](assets/rates-on-rate-card.png)

## Modifica dettagli e tariffe della scheda tariffe

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Per modificare una scheda tariffa esistente, fare clic sul nome della scheda tariffa nell&#39;elenco Schede tariffa.
1. Per aggiornare i dettagli della scheda tariffaria, fai clic su [!UICONTROL **Dettagli**] nel pannello a sinistra.
1. (Facoltativo) Per allegare un modulo personalizzato alla scheda tariffe, fare clic sul campo [!UICONTROL **Aggiungi modulo personalizzato**] nell&#39;angolo superiore destro della pagina Dettagli e selezionare un modulo personalizzato dall&#39;elenco visualizzato.

   Per ulteriori informazioni su come allegare un modulo personalizzato, vedere [Aggiungere un modulo personalizzato a un oggetto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Fai clic su [!UICONTROL **Salva modifiche**] dopo aver modificato i dettagli della scheda tariffe.
1. Fai clic su [!UICONTROL **Ruoli e tariffe**] nel pannello a sinistra per modificare le tariffe di fatturazione.
1. Per modificare una tariffa, seleziona la casella di controllo accanto alla tariffa e fai clic su [!UICONTROL **Modifica**] nella barra delle azioni nella parte inferiore dello schermo.

   Per ulteriori informazioni sulla barra delle azioni, vedere [Utilizzare elenchi avanzati](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

   >[!NOTE]
   >
   >Poiché ogni tasso è associato alla combinazione di ruolo e attributi per creare un tasso univoco, il ruolo e gli attributi non possono essere modificati quando si modifica un tasso.

1. Per eliminare una tariffa di fatturazione dalla scheda tariffe, selezionare la casella di controllo accanto alla tariffa e fare clic su [!UICONTROL **Elimina**] sulla barra delle azioni.
1. Per bloccare una tariffa, selezionare la casella di controllo accanto alla tariffa e fare clic su [!UICONTROL **Blocca**] sulla barra delle azioni.

   Le tariffe bloccate non possono essere modificate a livello di progetto o di attività. Accanto alle tariffe bloccate nell&#39;elenco viene visualizzata un&#39;icona di blocco.

   Puoi anche sbloccare una frequenza bloccata dalla barra delle azioni.

1. Per adeguare i tassi in base a una percentuale, eseguire la procedura seguente:

   1. Selezionare tutte le tariffe che si desidera regolare nella schermata Scheda tariffa > Ruoli e tariffe.

      Puoi scegliere una o più tariffe. Tutti saranno corretti della stessa percentuale.

   1. Fai clic su [!UICONTROL **Regola tariffe**] nella barra delle azioni.
   1. Nella casella [!UICONTROL **Regola tariffe mansioni**] scegliere se si desidera che la rettifica venga eseguita nel periodo di tempo selezionato (date di validità esistenti) o in un intervallo di date personalizzato definito dall&#39;utente.

      ![Casella Regola tariffe mansioni](assets/adjust-job-role-rates-dialog.png)

   1. Inserire il valore di adeguamento per i tassi.

      Questo valore viene applicato come percentuale. Ad esempio, se immetti 10, i tassi selezionati aumenteranno del 10%.

   1. Fai clic su [!UICONTROL **Aggiorna tariffe**].
   1. Fai clic su [!UICONTROL **Aggiorna**] nel messaggio di conferma.

      I tassi selezionati vengono aumentati della percentuale.

## Importa una scheda tariffe

Consulta l&#39;articolo [Importare schede tariffarie da un modello](/help/quicksilver/administration-and-setup/manage-enterprise-operations/import-rate-cards.md).

## Copiare una scheda tariffa

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Seleziona la casella di controllo accanto alla scheda delle tariffe nell&#39;elenco e fai clic sull&#39;icona **Copia** ![Copia icona](assets/copy-icon.png).
1. Digitare un nome per la nuova scheda tariffaria nella casella [!UICONTROL **Copia scheda tariffaria**]. Quindi fare clic su [!UICONTROL **Crea**].

   La nuova scheda tariffe viene salvata. Modifica i dettagli della scheda della tariffa, le mansioni e le tariffe in base alle esigenze.

## Eliminare un&#39;intera scheda tariffaria

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Selezionare la casella di controllo accanto alla scheda delle tariffe nell&#39;elenco e fare clic sull&#39;icona **Elimina** ![Elimina icona](assets/delete.png).

   >[!NOTE]
   >
   >Una scheda di tariffa allegata a un progetto verrà eliminata dal progetto.

