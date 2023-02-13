---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Condivisione di un rapporto calendario
description: È possibile condividere un calendario con altri utenti e renderlo disponibile pubblicamente, consentendo a un utente senza un [!DNL Adobe Workfront] licenza per visualizzarlo.
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Condivisione di un rapporto calendario

È possibile condividere un calendario con altri utenti e renderlo disponibile pubblicamente, consentendo a un utente senza un [!DNL Adobe Workfront] licenza per visualizzarlo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>[!UICONTROL View] o accesso successivo [!UICONTROL a Reports], [!UICONTROL Dashboards] e [!UICONTROL Calendari]</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Visualizzazione calendario o autorizzazioni successive, con accesso alla condivisione</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Condividi un calendario con [!DNL Workfront] utenti {#share-a-calendar-with-workfront-users}

La condivisione di un calendario è simile alla condivisione di altri oggetti. Per ulteriori informazioni sulla condivisione di oggetti in [!DNL Adobe Workfront], vedi [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

I calendari condivisi con l&#39;utente vengono visualizzati con un asterisco (&#42;) accanto al nome del calendario.

Per condividere un calendario all&#39;interno di [!DNL Workfront]:

1. Passa al calendario che desideri condividere.
1. Fai clic su **[!UICONTROL Azioni calendario]**, quindi fai clic su **[!UICONTROL Condivisione]**.

1. In **[!UICONTROL Assegna a Calendario l&#39;accesso a]** inizia a digitare il nome dell&#39;utente, del team, del ruolo, del gruppo o della società che desideri condividere il calendario, quindi fai clic sul nome quando viene visualizzato nell&#39;elenco a discesa.\
   Per informazioni sull&#39;impostazione delle autorizzazioni, vedi [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Facoltativo) Ripetere il passaggio 3 per ogni utente, team, ruolo o gruppo a cui si desidera concedere l&#39;accesso al calendario.
1. Specifica le autorizzazioni per ogni utente, team, ruolo, gruppo o società aggiunto al passaggio 3 facendo clic sul menu a discesa, quindi seleziona il livello di autorizzazione che desideri concedere:

   * **[!UICONTROL Visualizza]:** Gli utenti possono rivedere e condividere il calendario.

      ![Condividere il calendario con Visualizza accesso](assets/calendar-share-view-permissions-350x249.png)

   * **[!UICONTROL Gestisci]:** Gli utenti hanno accesso completo al calendario, senza diritti amministrativi, concessi a livello di accesso e con tutte le autorizzazioni di visualizzazione.

      ![Condividere il calendario con Gestisci accesso](assets/calendar-share-manage-permissions-350x241.png)

      >[!NOTE]
      >
      >La [!DNL Workfront] l&#39;amministratore e il creatore del calendario possono rimuovere le autorizzazioni da queste entità.

1. (Facoltativo) A seconda del ruolo di un utente, puoi fare clic su **[!UICONTROL Opzioni avanzate]**, quindi fai clic su **[!UICONTROL Condividi]**&#x200B; per consentire all’utente di condividere il calendario con altri utenti.

   Per ulteriori informazioni sui livelli di autorizzazione, vedi [Panoramica della condivisione delle autorizzazioni sugli oggetti](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Facoltativo) Per rendere il calendario disponibile a tutti [!DNL Workfront] utenti, fai clic sull’icona a forma di ingranaggio, quindi fai clic su nel menu a discesa **[!UICONTROL Rendere visibile il sistema a livello di sistema]** per rendere l’oggetto disponibile a tutti [!DNL Workfront] utenti.\
   Tutti gli utenti possono visualizzare l’oggetto in base alle autorizzazioni impostate.

1. Fai clic su **[!UICONTROL Salva]**.

## Condividere un calendario con un collegamento pubblico

Puoi rendere un calendario pubblico e condividere un collegamento con persone che non hanno un [!DNL Workfront] licenza.

1. Passa al calendario che desideri condividere.
1. Fai clic su **[!UICONTROL Azioni calendario]**, quindi fai clic su **[!UICONTROL Condivisione]**.

1. Fai clic sull’icona a forma di ingranaggio, quindi fai clic su **[!UICONTROL Rendi pubblico a utenti esterni]**.
1. Fai clic su **[!UICONTROL Copia collegamento]**.
1. Fai clic su **[!UICONTROL Salva]**.

## Condividere un calendario con un collegamento privato

Puoi condividere un collegamento di calendario privato con [!DNL Workfront] utenti. Gli utenti devono accedere per visualizzare il calendario quando utilizzano il collegamento.

1. Passa al calendario che desideri condividere.
1. Fai clic su **[!UICONTROL Azioni calendario]**, quindi fai clic su **[!UICONTROL Ottieni collegamento condivisibile]**.

1. Fai clic su **[!UICONTROL Copia collegamento]**.

   >[!NOTE]
   >
   >[!DNL Workfront] gli utenti devono avere accesso al calendario per accedervi con il collegamento. Per concedere l&#39;accesso, vedi [Condividi un calendario con [!DNL Workfront] utenti](#share-a-calendar-with-workfront-users).\
   >Se gli utenti non hanno accesso, possono richiederlo dopo aver incollato il collegamento nel browser.
