---
title: Panoramica dei tipi di record di connessione
description: Un modo per indicare la correlazione tra i singoli tipi di record consiste nel collegarli. Inoltre, è possibile collegare i tipi di record di Adobe Workfront Planning con i tipi di oggetto di altre applicazioni per migliorare l'esperienza degli utenti e mantenere lo stato attivo in un'unica applicazione.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '1086'
ht-degree: 1%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Panoramica sulla connessione dei tipi di record

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

È possibile indicare che i singoli tipi di record sono correlati tra loro o a oggetti di altre applicazioni collegandoli.

Questo articolo offre una panoramica delle connessioni dei tipi di record e descrive i tipi di connessioni che è possibile stabilire tra tipi di record e tipi di oggetto.

Per informazioni sulla connessione dei tipi di record, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

## Considerazioni sulla connessione dei tipi di record

* È possibile connettere le seguenti entità in Adobe Workfront Planning:

   * Due tipi di record.

     Per impostazione predefinita, è possibile connettere due tipi di record dallo stesso workspace. È inoltre possibile impostare tipi di record per la connessione con tipi di record di altre aree di lavoro.
   * Tipo di record e tipo di oggetto di un&#39;altra applicazione.

* È possibile connettere i tipi di record di Workfront Planning ai tipi di oggetto seguenti delle applicazioni seguenti:

   * Adobe Workfront:

      * Progetti
      * Portfolio
      * Programmi
      * Aziende
      * Gruppi

   * Adobe Experience Manager Assets:

      * Immagini
      * Cartelle

     >[!IMPORTANT]
     >
     >È necessario disporre di una licenza Adobe Experience Manager Assets e l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Business Platform o Adobe Admin Console per collegare i record di Workfront Planning ad Adobe Experience Manager Assets.
     >
     >Se hai domande sull&#39;onboarding in Adobe Admin Console, consulta le [Domande frequenti sull&#39;esperienza unificata di Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Dopo aver creato singoli record per un tipo di record, è possibile selezionare i record a cui ci si connette dal campo del tipo di record collegato. Per informazioni, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

* Dopo aver collegato un tipo di record a un altro tipo di record o a un tipo di oggetto di un&#39;altra applicazione, si verificano i seguenti scenari:

   * **Quando si connettono due tipi di record**: viene creato un campo record collegato nel tipo di record da cui si sta effettuando la connessione. Un campo record collegato simile viene creato nel tipo di record a cui ci si connette.

     Ad esempio, se colleghi il tipo di record &quot;Campagna&quot; al tipo di record &quot;Prodotto&quot;, nel tipo di record Campagna viene creato un campo record collegato denominato &quot;Prodotto collegato&quot;. Nel tipo di record Prodotto viene creato automaticamente un tipo di record collegato denominato &quot;Campaign&quot;.

   * **Quando si connette un tipo di record con un tipo di oggetto di un&#39;altra applicazione**:

      * Nel tipo di record da cui si sta effettuando la connessione viene creato un campo record collegato. Nessun campo record collegato viene creato automaticamente sul tipo di oggetto dell&#39;altra applicazione.

      * I campi dei record di Planning non sono accessibili dagli oggetti di Workfront.
      * I campi dei record di pianificazione sono accessibili da Experience Manager Assets quando l’amministratore Workfront configura la mappatura dei metadati tramite l’integrazione tra Workfront e Adobe Experience Manager Assets. Per ulteriori informazioni, consulta [Configurare la mappatura dei metadati delle risorse tra Adobe Workfront e Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

   * **Quando si aggiungono campi collegati (o di ricerca) dal record o dall&#39;oggetto a cui ci si connette**: oltre a creare un campo record collegato, è anche possibile connettersi ai campi del record o del tipo di oggetto connesso denominati campi di ricerca. Un campo di ricerca collegato con le informazioni del record a cui ci si connette viene visualizzato nel record da cui ci si connette.

     È possibile collegare campi di altri tipi di record o oggetti di un&#39;altra applicazione al tipo di record di Workfront Planning.

     I campi collegati sono di sola lettura e visualizzano automaticamente le informazioni dei record o degli oggetti connessi quando si collegano i record o gli oggetti.

     È possibile fare riferimento a campi di ricerca di altri tipi di record o oggetti in formule, filtri o raggruppamenti.

     Ad esempio, se si collega il tipo di record &quot;Campagna&quot; a un progetto Workfront e si seleziona di inserire il campo Data di completamento pianificata del progetto nel record Pianificazione di Workfront, per la campagna viene automaticamente creato un campo collegato denominato Data di completamento pianificata (da progetto). Impossibile modificare manualmente il campo collegato. Nel campo Data di completamento pianificata (da progetto) viene visualizzata la Data di completamento pianificata dei progetti collegati.

     >[!IMPORTANT]
     >
     >Tutti gli utenti con autorizzazioni View (Visualizzazione) o superiori all&#39;area di lavoro possono visualizzare le informazioni nei campi di ricerca, indipendentemente dalle autorizzazioni o dal livello di accesso nell&#39;applicazione dei tipi di oggetto collegato <!--or their permissions in other workspaces-->.

<!--see the commented out text above for the release of cross-workspace connections-->

* I campi record collegati sono preceduti dall&#39;icona di relazione ![](assets/relationship-field-icon.png).

  I campi collegati sono preceduti da un’icona che identifica il tipo di campo. Ad esempio, i campi collegati (o di ricerca) sono preceduti da icone che indicano che un campo è un numero, un paragrafo o una data.


## Tipi di connessione

Dopo aver stabilito una connessione tra due tipi di record o tra un record e un tipo di oggetto da un&#39;altra applicazione, è possibile aggiungere record nei campi dei record connessi.

A seconda del numero di record che è possibile aggiungere a un campo record connesso, i tipi di connessione disponibili per la connessione dei tipi di record sono i seguenti:

* [Da uno a molti](#one-to-many-connection-type)
* [Da uno a uno](#many-to-one-connection-type)
* [Da molti a uno](#many-to-one-connection-type)
* [Da molti a molti](#many-to-many-connection-type)

>[!WARNING]
>
>Queste opzioni non sono disponibili quando si collegano i seguenti elementi:
>* Due record da aree di lavoro diverse
>
>* Un tipo di record e risorse AEM


<!-- add screen shots for each type of connection below-->

### Tipo di connessione uno-a-molti

![](assets/one-to-many-connection-picker.png)

Quando si seleziona il tipo di connessione uno-a-molti tra tipi di record, è possibile collegare un record in un secondo momento a più record a cui ci si connette.

Ad esempio, se colleghi le campagne ai progetti, puoi collegare una campagna a più progetti. Tuttavia, un progetto può essere connesso a una sola campagna.

Quando si seleziona questo tipo di connessione, è possibile modificarlo in un secondo momento solo in un tipo di connessione molti-a-molti.

### Tipo di connessione uno-a-uno

![](assets/one-to-one-connection-picker.png)

Quando si seleziona il tipo di connessione uno-a-uno tra i tipi di record, è possibile collegare un record in un secondo momento a un altro record a cui ci si connette.

Ad esempio, se colleghi le campagne ai progetti, puoi collegare una campagna a un progetto. Un progetto può essere connesso a una sola campagna.

Quando selezioni questo tipo di connessione, puoi successivamente modificarlo in qualsiasi altro tipo di connessione.

### Tipo di connessione molti-a-uno

![](assets/many-to-one-connection-picker.png)

Quando si seleziona il tipo di connessione molti-a-uno tra tipi di record, è possibile collegare più record in un secondo momento con un solo record a cui ci si connette.

Ad esempio, se colleghi le campagne ai progetti, puoi collegare più campagne a un unico progetto. Un progetto può essere connesso a più campagne.

Quando si seleziona questo tipo di connessione, è possibile modificarlo in un secondo momento solo in un tipo di connessione molti-a-molti.

### Tipo di connessione da molti-a-molti

![](assets/many-to-many-connection-picker.png)

Quando si seleziona il tipo di connessione molti-a-molti tra tipi di record, è possibile collegare più record in un secondo momento.

Ad esempio, se colleghi le campagne ai progetti, puoi collegare più campagne a più progetti. Puoi anche collegare più progetti a più campagne.

Quando si seleziona questo tipo di connessione, non è possibile modificarlo dopo averlo salvato.

