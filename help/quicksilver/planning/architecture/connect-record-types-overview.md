---
title: Panoramica sui tipi di record collegati
description: Un modo per indicare la correlazione tra i singoli tipi di record consiste nel collegarli. Inoltre, è possibile collegare i tipi di record di Adobe Workfront Planning con i tipi di oggetto di altre applicazioni per migliorare l'esperienza degli utenti e mantenere lo stato attivo in un'unica applicazione.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Panoramica sui tipi di record collegati

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

È possibile indicare che i singoli tipi di record sono correlati tra loro o a oggetti di altre applicazioni collegandoli.

Questo articolo offre una panoramica delle connessioni dei tipi di record e descrive i tipi di connessioni che è possibile stabilire tra tipi di record e tipi di oggetto.

Per informazioni sulla connessione dei tipi di record, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).

## Considerazioni sulla connessione dei tipi di record

In Workfront Planning sono disponibili due passaggi per le connessioni:

1. Innanzitutto, è necessario stabilire una connessione tra due tipi di record o un tipo di record e un tipo di oggetto da un&#39;altra applicazione. Per informazioni su come connettere i tipi di record, vedere [Connetti tipi di record](/help/quicksilver/planning/architecture/connect-record-types.md).
1. In secondo luogo, è possibile collegare singoli record di un tipo a record di un altro tipo dopo aver connesso i due tipi di record. Per informazioni sulla connessione dei record, vedere [Connetti record](/help/quicksilver/planning/records/connect-records.md).

Considerare le seguenti informazioni sulla connessione dei tipi di record:

* È possibile connettere le seguenti entità in Adobe Workfront Planning:

   * Due tipi di record.

     Per impostazione predefinita, è possibile connettere due tipi di record dallo stesso workspace. È inoltre possibile impostare tipi di record per la connessione con tipi di record di altre aree di lavoro. Per informazioni, vedere [Modifica tipi di record](/help/quicksilver/planning/architecture/edit-record-types.md).
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
     >Tutti gli utenti con autorizzazioni View (Visualizzazione) o superiori all&#39;area di lavoro possono visualizzare le informazioni nei campi di ricerca, indipendentemente dalle autorizzazioni o dal livello di accesso nell&#39;applicazione dei tipi di oggetto collegati o dalle autorizzazioni in altre aree di lavoro.

     I campi record collegati sono preceduti dall&#39;icona di relazione ![](assets/relationship-field-icon.png).

     I campi collegati sono preceduti da un’icona che identifica il tipo di campo. Ad esempio, i campi collegati (o di ricerca) sono preceduti da icone che indicano che un campo è un numero, un paragrafo o una data.

<!--## Connection types

After you establish a connection between two record types or between a record and an object type from another application, you can add records in the connected record fields. 

Depending on how many records you can add to a connected record field, the following are the connection types you can choose from when connecting record types: 

* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)

>[!WARNING]
>
>These options are not available when connecting the following: 
>* Two records from different workspaces
>
>* A record type and AEM assets

### Many-to-many connection type

![](assets/many-to-many-connection-picker.png)

When you select the many-to-many connection type between record types, you can later connect many records with multiple records you're connecting to. 

For example, if you connect campaigns with projects and you choose this type of connection, you can connect several campaigns with multiple projects. You can also connect the same projects you are connecting to the campaigns to more than one campaign. 

A real-life example of a many-to-many relationship type is the relationship between customers and products: customers can purchase multiple products; and those products can also be purchased by many other customers. 

When you select this connection type, you cannot change the connection type after you save it. 

### One-to-many connection type

![](assets/one-to-many-connection-picker.png)

When you select the one-to-many connection type between record types, you can later connect one record with multiple records you're connecting to. 

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with multiple projects. But one of the projects you're connecting to the campaigns can be connected only to one campaign at a time. 

A real-life example of a one-to-many relationship type is the relationship between libraries and books: a library has many books in its inventory; but one particular book can only be in one library at a given point in time. 

When you select this connection type, you can later change it only to a many-to-many connection type. 
 
### Many-to-one connection type

![](assets/many-to-one-connection-picker.png)

When you select the many-to-one connection type between record types, you can later connect many records with only one record you're connecting to. 

For example, if you connect campaigns with projects and you choose this type of connection, you can add only one project to a campaign. But you can add multiple campaigns to one project. 

A real-life example of a many-to-one relationship type is the relationship between many movies and one actor: one actor can be in many movies, but each movie can only have a specific actor once in its cast. 

When you select this connection type, you can later change it only to a many-to-many connection type.

### One-to-one connection type

![](assets/one-to-one-connection-picker.png)

When you select the one-to-one connection type between record types, you can later connect one record with one other record that you're connecting to. 

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with one project. One project can be connected only to one campaign. 

A real-life example of a one-to-one relationship is the one existing between a person and their country's unique identifier (like a Social Security Number, Passport ID, local identification ID): each person has only one unique identifier for a country and each unique identifier can be linked to only one person. 

When you select this connection type, you can later change it to any other connection type. 

-->



