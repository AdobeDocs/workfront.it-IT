---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Livelli di autorizzazione per  [!DNL Workfront]  per Outlook
description: Il componente aggiuntivo  [!DNL Workfront for Outlook]  richiede l'accesso in lettura/scrittura alle cassette postali. L'integrazione di  [!DNL Workfront for Outlook] richiede le autorizzazioni di livello più alto perché dispone della funzionalità per scaricare gli allegati di posta elettronica dal server di Exchange di Outlook e caricarli in [!DNL Workfront], quando l'utente invia una richiesta da un indirizzo di posta elettronica contenente allegati.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Livelli di autorizzazione per [!DNL Workfront for Outlook]

>[!IMPORTANT]
>
>Microsoft [È in corso la disabilitazione del supporto per i token online di Exchange legacy](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), attualmente utilizzati dal componente aggiuntivo di Workfront Outlook per l&#39;autenticazione. Questa modifica di Microsoft ha già iniziato a interessare i clienti e continuerà a essere implementata in più fasi fino a ottobre 2025.
>
>* **Dopo la completa disattivazione di questi token da parte di Microsoft, l&#39;integrazione di Workfront per Microsoft Outlook non funzionerà più.**
>
>Come parte di questa modifica, Microsoft ha deciso di cambiare il modo in cui i token vengono riabilitati. Dopo il **30 giugno 2025**, gli amministratori non saranno più in grado di riabilitare i token personalmente. Solo il supporto Microsoft può concedere eccezioni. **Il 1° ottobre 2025, i token legacy verranno disattivati per tutti i tenant. Le eccezioni non verranno concesse.**

[!DNL Workfront for Outlook] richiede il più alto dei quattro livelli di autorizzazioni consentiti nei componenti aggiuntivi di [!DNL Outlook].

Per informazioni dettagliate sulle autorizzazioni nei componenti aggiuntivi [!DNL Outlook], vedere [Privacy, autorizzazioni e sicurezza per  [!DNL Outlook] componenti aggiuntivi](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) nella documentazione di [!DNL Microsoft].

Il componente aggiuntivo [!DNL Workfront for Outlook] richiede l&#39;accesso in lettura/scrittura alle cassette postali (`ReadWriteMailbox`), che rappresenta l&#39;ambito di autorizzazione più elevato.
L&#39;integrazione di [!DNL Workfront for Outlook] richiede le autorizzazioni di livello più alto perché dispone della funzionalità per scaricare gli allegati di posta elettronica dal server Exchange [!DNL Outlook] e caricarli in [!DNL Workfront], quando l&#39;utente invia una richiesta da un indirizzo di posta elettronica contenente allegati. Affinché questa funzionalità funzioni, [!DNL Workfront for Outlook] utilizza la funzione `mailbox.getCallbackTokenAsync()` dell&#39;API JavaScript del componente aggiuntivo [!DNL Office] per ottenere il token e utilizzarlo per scaricare gli allegati di posta elettronica dal server Exchange. L&#39;unica autorizzazione che consente l&#39;utilizzo di tale funzione è `ReadWriteMailbox`. Per ulteriori informazioni, vedere [Privacy, autorizzazioni e protezione per i componenti aggiuntivi di Outlook](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) nella documentazione di Microsoft.

Il componente aggiuntivo [!DNL Workfront for Outlook] richiede anche l&#39;autorizzazione `ReadWriteItem` (inclusa in `ReadWriteMailbox`), che viene utilizzata per leggere il corpo dell&#39;e-mail e leggere/aggiornare i metadati dell&#39;e-mail:

* Leggi corpo dell’e-mail:

  [!DNL Workfront for Outlook] legge il corpo dell&#39;e-mail quando un utente invia la richiesta o invia il corpo dell&#39;e-mail come aggiornamento all&#39;oggetto [!DNL Adobe Workfront].
* Leggi/aggiorna metadati e-mail:

  [!DNL Workfront for Outlook] aggiorna le intestazioni e-mail quando un utente invia una richiesta da un indirizzo e-mail. Questa operazione viene eseguita per memorizzare le informazioni sull&#39;oggetto [!DNL Adobe Workfront] inviato, in modo che alla successiva apertura del componente aggiuntivo per la stessa e-mail vengano visualizzate le informazioni sulle azioni precedenti eseguite con tale e-mail.

[!DNL Workfront for Outlook] accede alla cassetta postale di un utente solo quando l&#39;utente esegue un&#39;azione all&#39;interno del componente aggiuntivo. Non dispone di alcuna funzionalità di background. Workfront per Outlook accede alla cassetta postale dell&#39;utente solo nel seguente scenario:

* L&#39;utente tenta di inviare una richiesta, creare un&#39;attività o inviare un messaggio e-mail come aggiornamento da [!DNL Workfront for Outlook] (apertura del componente aggiuntivo e selezione di un&#39;azione)
   * [!DNL Workfront for Outlook] legge il corpo dell&#39;e-mail da compilare nel modulo all&#39;interno del componente aggiuntivo.
   * [!DNL Workfront for Outlook] legge i metadati e-mail per visualizzare informazioni sul componente aggiuntivo sulle azioni precedenti eseguite con lo stesso messaggio e-mail.
* Quando un utente invia una richiesta, crea un&#39;attività o invia un messaggio e-mail come aggiornamento da [!DNL Workfront for Outlook] (facendo clic sul pulsante [!UICONTROL invia] sul componente aggiuntivo):
   * [!DNL Workfront for Outlook] legge il corpo dell&#39;e-mail per inviarla a Workfront come descrizione di richiesta o commento.
   * [!DNL Workfront for Outlook] aggiorna i metadati e-mail per memorizzare informazioni sulle richieste inviate o sull&#39;oggetto aggiornato.
   * [!DNL Workfront for Outlook] scarica gli allegati di posta elettronica dal server di exchange per caricarli nelle richieste inviate, nelle attività create o negli oggetti aggiornati.
