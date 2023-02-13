---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Livelli di autorizzazione per [!DNL Workfront] per Outlook
description: La [!DNL Workfront for Outlook] il componente aggiuntivo richiede l'accesso in lettura/scrittura alla cassetta postale. La [!DNL Workfront for Outlook] L'integrazione richiede le autorizzazioni di livello più elevato perché dispone della funzionalità per scaricare gli allegati e-mail dal server di scambio di Outlook e caricarli in [!DNL Workfront], quando l’utente invia una richiesta da un messaggio e-mail contenente allegati.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Livelli di autorizzazione per [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] richiede il massimo dei quattro livelli di autorizzazioni consentiti in [!DNL Outlook] componenti aggiuntivi.

Per informazioni dettagliate sulle autorizzazioni in [!DNL Outlook] componenti aggiuntivi, vedi [Privacy, autorizzazioni e sicurezza per [!DNL Outlook] componenti aggiuntivi](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in [!DNL Microsoft] documentazione.

La [!DNL Workfront for Outlook] il componente aggiuntivo richiede l&#39;accesso in lettura/scrittura alla cassetta postale (`ReadWriteMailbox`), che è l’ambito di autorizzazione più elevato.
La [!DNL Workfront for Outlook] l’integrazione richiede le autorizzazioni di livello più elevato perché dispone della funzionalità per scaricare gli allegati e-mail da [!DNL Outlook] scambia server e caricali in [!DNL Workfront], quando l’utente invia una richiesta da un messaggio e-mail contenente allegati. Affinché questa funzionalità funzioni, [!DNL Workfront for Outlook] utilizza la funzione `mailbox.getCallbackTokenAsync()` da [!DNL Office] Aggiungi l’API JavaScript per ottenere il Token e utilizzarlo per scaricare gli allegati e-mail dal server di Exchange. L&#39;unica autorizzazione che consente l&#39;utilizzo di quella funzione è `ReadWriteMailbox`. Per ulteriori informazioni, consulta [Privacy, autorizzazioni e sicurezza dei componenti aggiuntivi di Outlook](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) nella documentazione di Microsoft.

La [!DNL Workfront for Outlook] add-in richiede anche `ReadWriteItem` (incluso in `ReadWriteMailbox`), che viene utilizzato per leggere il corpo dell’e-mail e leggere/aggiornare i metadati dell’e-mail:

* Corpo del messaggio e-mail di lettura:

   [!DNL Workfront for Outlook] legge il corpo dell’e-mail quando un utente invia la richiesta o invia il corpo dell’e-mail come aggiornamento a [!DNL Adobe Workfront] Oggetto.
* Metadati e-mail di lettura/aggiornamento:

   [!DNL Workfront for Outlook] aggiorna le intestazioni dell’e-mail quando un utente invia una richiesta da un messaggio e-mail. Questa operazione consente di memorizzare informazioni sull&#39;invio [!DNL Adobe Workfront] quindi, alla successiva apertura del componente aggiuntivo per la stessa e-mail, vengono visualizzate le informazioni sulle azioni precedenti con tale e-mail.

[!DNL Workfront for Outlook] accede alla cassetta postale di un utente solo quando l&#39;utente esegue un&#39;azione all&#39;interno del componente aggiuntivo. Non dispone di funzionalità di sfondo. Workfront for Outlook accede alla cassetta postale dell&#39;utente solo nel seguente scenario:

* L’utente tenta di inviare una richiesta, creare un’attività o inviare un messaggio e-mail come aggiornamento da [!DNL Workfront for Outlook] (Apertura del componente aggiuntivo e selezione di un’azione)
   * [!DNL Workfront for Outlook] legge il corpo dell&#39;e-mail da compilare nel modulo all&#39;interno del componente aggiuntivo.
   * [!DNL Workfront for Outlook] legge i metadati e-mail per visualizzare informazioni sul componente aggiuntivo relative alle azioni precedenti eseguite nel componente aggiuntivo con la stessa e-mail.
* Quando un utente invia una richiesta, crea un’attività o invia un messaggio e-mail come aggiornamento da [!DNL Workfront for Outlook] (facendo clic sul pulsante [!UICONTROL submit] pulsante sul componente aggiuntivo):
   * [!DNL Workfront for Outlook] legge il corpo dell’e-mail per inviarla a Workfront come descrizione della richiesta o come commento.
   * [!DNL Workfront for Outlook] aggiorna i metadati dell’e-mail per memorizzare informazioni sulle richieste inviate o sull’oggetto aggiornato.
   * [!DNL Workfront for Outlook] scarica gli allegati e-mail dal server di Exchange per caricarli nelle richieste inviate, nelle attività create o negli oggetti aggiornati.
