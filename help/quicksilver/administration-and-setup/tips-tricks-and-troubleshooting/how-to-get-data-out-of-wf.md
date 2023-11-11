---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Esportare dati storici da Adobe Workfront: pro e contro"
description: In questo articolo vengono illustrati i pro e i contro di 4 opzioni che è possibile utilizzare per esportare dati storici da Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Esporta dati storici da [!DNL Adobe Workfron]t: pro e contro

Questo articolo spiega i pro e i contro di 4 opzioni che puoi utilizzare per esportare dati storici da [!DNL Workfront].

## Utilizza uno dei nostri partner

[!DNL AtAppStore], a [!DNL Workfront] partner certificato, dispone di un’app facile da usare che ti consente di scaricare i tuoi dati. Questa app include anche un visualizzatore che ti consente di visualizzare facilmente i dati.

* **Pro:** Tutti i tuoi [!DNL Workfront] vengono esportati gli oggetti, inclusi i campi personalizzati. L&#39;interfaccia del visualizzatore è facile da usare e da leggere ed è facilmente importabile in un [!DNL MS Access] Database.

* **Contro:** I documenti non vengono esportati. Dovrai scaricarli separatamente. Per ulteriori informazioni, consulta [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Richiedi [!DNL Postgres] file di dump dei dati dal nostro team di database

Il tuo Account Executive può inviare una richiesta al nostro team di database per esportare un file di dump del database (.dmp [!DNL Postgres] file) con i dati. Un’ulteriore richiesta andrà al nostro team AOS per recuperare tutti i documenti memorizzati.

* **Pro**: puoi ottenere l’intero caricamento dei dati, inclusi i campi personalizzati, e i documenti memorizzati nel sistema.

* **Contro**: il file di database è di difficile lettura: non è possibile leggerlo a meno che non venga caricato in un [!DNL Postgres] e ristabilire le relazioni tra le tabelle. I documenti vengono memorizzati in un file server separato e devono essere estratti separatamente utilizzando un processo separato dal team AOS. In questo modo, non esiste alcuna organizzazione per i documenti, a cui viene fatto riferimento tramite il relativo GUID.
* **Costo**: questo download comporta dei costi, a seconda di quanto tempo il team impiega per creare il file. Per ulteriori informazioni o per iniziare il processo, rivolgiti al tuo AE/CAE.

## Esporta tramite [!UICONTROL Kick-Start]

Che tu disponga o meno di ore di consulenza in remoto, puoi utilizzare uno dei nostri consulenti per esportare i tuoi dati sotto forma di rapporti o [!UICONTROL kick-start]oppure puoi eseguire questi rapporti autonomamente:

* **Pro**: i rapporti sono di facile lettura e possono essere importati in diverse applicazioni; possono essere personalizzati per includere qualsiasi raggruppamento e visualizzazione desiderati.

* **Contro**: i documenti dovranno essere scaricati separatamente.

* **Costo**: è gratuito se puoi eseguire i rapporti autonomamente (tutto ciò di cui hai bisogno è un accesso come amministratore di sistema), o se puoi utilizzare gli orari di consulenza remota rimanenti. Se ti interessa acquistare consulenza remota per questo, contatta il tuo AE/CAE.

  Per ulteriori informazioni sull&#39;utilizzo di Kick-Start per esportare i dati, consulta [Esporta dati da [!DNL Adobe Workfront] tramite [!UICONTROL Kick-Start]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utilizza la nostra API aperta

se disponi delle risorse giuste all’interno dell’organizzazione, può creare un’API personalizzata per recuperare tutti i dati da Workfront:

* **Pro**: hai il controllo delle esportazioni dal sistema.

* **Contro**: il tempo viene trascorso al tuo fianco e dovrai trovare le risorse per codificare l’API ed eseguire l’esportazione.

* **Costo**: interno all’organizzazione.
