---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Esportare dati storici da Adobe Workfront: pro e contro'
description: In questo articolo vengono illustrati i pro e i contro di 4 opzioni che è possibile utilizzare per esportare dati storici da Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Esporta dati storici da [!DNL Adobe Workfront]: pro e contro

<!-- Audited: 5/2025 -->

Questo articolo spiega i pro e i contro di 4 opzioni che puoi utilizzare per esportare dati storici da Adobe Workfront.

## Utilizza uno dei nostri partner

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) dispone di un&#39;app di facile utilizzo (la relativa soluzione [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/)) che ti consente di scaricare i tuoi dati da solo. Un visualizzatore opzionale (la relativa soluzione [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)) consente di visualizzare facilmente i dati offline.

* **Pro:** Tutti gli oggetti [!DNL Workfront] principali vengono esportati, inclusi i campi e le note personalizzati, e memorizzati in un database [!DNL MS Access] facilmente accessibile. L&#39;interfaccia del visualizzatore è di facile utilizzo e lettura. L&#39;estrazione di documenti è disponibile separatamente come servizio, con l&#39;output organizzato in una struttura logica di cartelle mappata a ciascun documento e alle versioni precedenti.

* **Contro:** esiste una limitazione tecnica di 2 GB di dati, ma AtAppStore consente di acquistare solo ciò che ti serve.

* **Costi:** Per ulteriori informazioni, visitare il sito Web [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).

## Richiedi un file di dump dei dati [!DNL Postgres] dal nostro team di database

È necessario inviare una richiesta al nostro team di Assistenza clienti, che invierà quindi una richiesta al nostro team di database per esportare un file di dump del database (file con estensione dmp [!DNL Postgres]) con i tuoi dati. Verrà inviata una richiesta aggiuntiva al nostro team NOC per recuperare tutti i documenti archiviati.

* **Pro**: ottieni l&#39;intero caricamento dei dati, inclusi i campi personalizzati, nonché i documenti archiviati nel sistema.

* **Contro**: non è possibile leggere questo file a meno che non venga caricato in un database [!DNL Postgres] e non vengano ristabilite le relazioni tra le tabelle. I documenti vengono memorizzati in un file server separato e devono essere estratti separatamente utilizzando un processo separato dal team NOC. In questo modo, non esiste alcuna organizzazione per i documenti, a cui viene fatto riferimento tramite il relativo GUID.

* **Costo**: esiste un costo associato a questo download a seconda del tempo impiegato dal team per creare il file. Per ulteriori informazioni o per iniziare il processo, rivolgiti al tuo AE/CAE.

## Esporta tramite [!UICONTROL Kick-Start]

Che tu disponga o meno di ore di consulenza remota, puoi utilizzare uno dei nostri consulenti per esportare i tuoi dati sotto forma di report o [!UICONTROL avvii], oppure puoi eseguire questi report autonomamente:

* **Pro**: i report sono facili da leggere e possono essere importati in diverse applicazioni. Possono essere personalizzate in modo da includere i raggruppamenti e le viste desiderate.

* **Contro**: i documenti dovranno essere scaricati separatamente.

* **Costo**: è gratuito se è possibile eseguire i report autonomamente (tutto ciò di cui hai bisogno è un accesso amministratore di sistema) o se è possibile utilizzare gli orari di consulenza remota rimanenti. Se ti interessa acquistare consulenza remota per questo, contatta il tuo AE/CAE.

  Per ulteriori informazioni sull&#39;utilizzo di Kick-Start per esportare dati, vedere [Esportare dati da [!DNL Adobe Workfront] tramite [!UICONTROL Kick-Start]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utilizza la nostra API aperta

se disponi delle risorse giuste all’interno dell’organizzazione, può creare un’API personalizzata per recuperare tutti i dati da Workfront:

* **Pro**: hai il controllo delle esportazioni dal sistema.

* **Contro**: il tempo è trascorso al tuo fianco e dovrai trovare le risorse per codificare l&#39;API ed eseguire l&#39;esportazione.

* **Costo**: è interno alla tua organizzazione.
