---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Nome utente già in uso
description: Leggi questi suggerimenti quando ottieni un errore che il nome utente è già preso.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Nome utente già in uso

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza</strong></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Domanda

Quando crei un nuovo utente, un [!UICONTROL Whops] viene visualizzato un errore che indica che il nome utente è già stato preso. Non ci sono altre occorrenze di questo messaggio e-mail nel sistema. Perché viene visualizzato?

## Soluzione

Questo può verificarsi perché il nome utente o l’indirizzo e-mail non è univoco nel [!DNL Adobe Workfront] istanza. Gli utenti possono avere lo stesso nome utente o indirizzo e-mail in istanze separate. Ad esempio, l’utente A potrebbe avere i seguenti indirizzi e-mail associati a un [!DNL Workfront] account: usera@company1.com e usera@company2.com.

>[!NOTE]
>
>Il principale [!DNL Workfront] l&#39;amministratore non può avere lo stesso nome utente o indirizzo e-mail se si trovano in istanze Workfront separate sullo stesso cluster.
>
>Se le istanze si trovano in cluster diversi, l&#39;amministratore principale può avere lo stesso nome utente o indirizzo e-mail. Puoi visualizzare il cluster su cui si trova l&#39;istanza in [!UICONTROL Configurazione] > [!UICONTROL Sistema] > [!UICONTROL Informazioni cliente].

### Controlla se il tuo nome utente è univoco nella tua istanza

Assicurati che il nome utente e l’indirizzo e-mail siano univoci nell’attuale [!DNL Workfront] istanza:

1. Come [!DNL Workfront] amministratore, fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Utenti]**.
1. Nell’elenco delle persone, consulta **[!UICONTROL E-mail]** per garantire che non vi siano e-mail duplicate.
1. Aggiungi una colonna per il nome utente alla visualizzazione.

   1. In **[!UICONTROL Visualizza]** menu a discesa, fai clic su **[!UICONTROL Personalizza visualizzazione]**.
   1. Fai clic su **[!UICONTROL Aggiungi colonna]**.
   1. Nel campo di ricerca, digita *[!UICONTROL username]*.
   1. Seleziona **[!UICONTROL Utente]** > **[!UICONTROL Nome utente]**.
   1. Salva la visualizzazione.\
      In questo modo si visualizzano i nomi utente in cui è possibile cercare il duplicato.

1. Nell’elenco delle persone, consulta **[!UICONTROL Nome utente]** per evitare la presenza di nomi utente duplicati.
