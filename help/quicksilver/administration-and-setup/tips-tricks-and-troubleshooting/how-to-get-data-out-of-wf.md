---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Esporta dati storici da Adobe Workfront: Profili e contro"'
description: Questo articolo spiega i pro e i contro di 4 opzioni che puoi utilizzare per esportare dati storici da Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Esporta dati storici da [!DNL Adobe Workfron]t: pro e contro

Questo articolo spiega i pro e i contro di 4 opzioni che puoi utilizzare per esportare i dati storici da [!DNL Workfront].

## Utilizza uno dei nostri partner

[!DNL AtAppStore], [!DNL Workfront] partner certificato, dispone di un&#39;app facile da usare che ti consente di scaricare i tuoi dati. Questa app include anche un visualizzatore che consente di visualizzare facilmente i dati.

* **Pro:** Tutte le tue [!DNL Workfront] gli oggetti vengono esportati, inclusi i campi personalizzati. L&#39;interfaccia del visualizzatore è facile da usare e leggere ed è facilmente importabile in un [!DNL MS Access] Database.

* **Cons:** I documenti non vengono esportati. Dovrai scaricarli separatamente. Per ulteriori informazioni, consulta [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Richiedere un [!DNL Postgres] file di dump dati dal nostro team di database

Il tuo Account Executive può inviare una richiesta al nostro team di database per esportare un file di dump di database (.dmp [!DNL Postgres] file) con i tuoi dati. Una richiesta aggiuntiva verrà inviata al nostro team AOS per recuperare tutti i documenti archiviati.

* **Pro**: Puoi ottenere l’intero caricamento dei dati, inclusi i campi personalizzati, nonché i documenti memorizzati nel sistema.

* **Contro**: Il file di database è difficile da leggere: non c&#39;è modo di leggere questo file a meno che non lo carichi in un [!DNL Postgres] e ristabilire le relazioni tra le tabelle. I documenti vengono archiviati in un file server separato e devono essere estratti separatamente utilizzando un processo separato da parte del team AOS. In questo modo, i documenti non sono organizzati e il GUID li riporta tutti.
* **Costo**: A seconda di quanto tempo il team deve creare il file, è presente un costo associato a questo download. Per ulteriori informazioni o per avviare il processo, consulta la pagina AE/CAE .

## Esporta tramite [!UICONTROL Avvio]

Che tu abbia o meno ore di consulenza remota, puoi utilizzare uno dei nostri consulenti per esportare i tuoi dati sotto forma di report o [!UICONTROL avvio]oppure puoi eseguire questi rapporti autonomamente:

* **Pro**: Le relazioni sono facili da leggere e possono essere importate in diverse applicazioni; possono essere personalizzati per includere tutti i raggruppamenti e le visualizzazioni desiderati.

* **Contro**: I documenti dovranno essere scaricati separatamente.

* **Costo**: È gratuito se puoi eseguire i rapporti da solo (tutto ciò di cui hai bisogno è un accesso dell&#39;amministratore di sistema) o se puoi utilizzare le restanti ore di consulenza remota. Se siete interessati ad acquistare consulenza remota per questo, si prega di parlare con il vostro AE/CAE.

   Per ulteriori informazioni sull’utilizzo di Kick-Starts per esportare i dati, consulta [Esporta dati da [!DNL Adobe Workfront] tramite [!UICONTROL Avvio]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utilizza la nostra API aperta

se disponi delle risorse adeguate all’interno dell’organizzazione, puoi creare un’API personalizzata per recuperare tutti i dati da Workfront:

* **Pro**: Hai il controllo delle esportazioni dal sistema.

* **Contro**: Il tempo viene impiegato dal tuo lato e dovrai trovare le risorse per codificare l’API ed eseguire l’esportazione.

* **Costo**: Interno alla tua organizzazione.
