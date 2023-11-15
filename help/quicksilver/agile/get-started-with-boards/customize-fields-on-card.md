---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personalizzare i campi visualizzati su una scheda
description: È possibile personalizzare i campi visualizzati su una scheda disattivando un campo in modo che non venga visualizzato nella visualizzazione a schede complete o ridotta oppure nascondendo un campo nella visualizzazione a schede ridotta.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 63d043a85c2e5300d8b5872b2ec7983de4ba1f50
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Personalizzare i campi visualizzati su una scheda

Per impostazione predefinita, tutti i campi disponibili vengono visualizzati su una scheda, sia nella visualizzazione completa quando la scheda è aperta, sia nella visualizzazione ridotta sulla scheda. Puoi personalizzare i campi visualizzati in base a:

* Disabilitazione di un campo in modo che non venga visualizzato in nessuna delle due visualizzazioni
* Nascondere un campo nella visualizzazione scheda ridotta

Se un campo contiene un valore e si disattiva il campo, il valore viene mantenuto se si riattiva il campo in un secondo momento.

Puoi visualizzare e nascondere anche le sezioni (che vengono visualizzate come opzioni di navigazione a sinistra nei dettagli della scheda).

Puoi anche visualizzare i campi personalizzati creati in precedenza. Non puoi progettare e creare nuovi campi personalizzati all’interno di una bacheca.

>[!NOTE]
>
>Tutte le personalizzazioni dei campi apportate vengono applicate solo alla bacheca in cui stai lavorando.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano*</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Request] o versione successiva</p> </td> 
  </tr>
   </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare [!DNL Workfront] amministratore.

## Configurare le schede {#configure-cards}

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Schede]**.
1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Clic [!UICONTROL **Configura**] sulla destra della bacheca per aprire il pannello Configura.
1. Espandi [!UICONTROL **Schede**].

   La maggior parte dei campi e delle sezioni è attivata per impostazione predefinita.

1. Disattiva un campo o una sezione per disattivarla in entrambe le visualizzazioni a schede.
1. Fai clic sull’icona Nascondi ![Nascondi icona](assets/eye-hide-icon.png) accanto a un campo o a una sezione per nasconderlo nella visualizzazione ridotta.
1. Per visualizzare tutti i campi e le sezioni in entrambe le visualizzazioni, fare clic su [!UICONTROL **Ripristina tutti i campi ai valori predefiniti**].
1. Clic [!UICONTROL **Nascondi configurazione**] per chiudere il pannello Configura.

## Aggiungere campi personalizzati alle schede

I campi personalizzati sono disponibili sulle schede collegate. Sono visibili solo nella vista a schede completa, non nella vista a condensa sulla bacheca.

I dati sui campi personalizzati sono modificabili sulla scheda, anche se alcuni elementi personalizzati potrebbero essere disponibili per la modifica solo sul campo originale e non sulla scheda.

1. Accedi a una bacheca e fai clic su [!UICONTROL **Configura**] per aprire il pannello Configura.
1. Espandi [!UICONTROL **Schede**].
1. Sotto [!UICONTROL Campi scheda], fai clic su [!UICONTROL **Aggiungi campo personalizzato**].
1. Seleziona [!UICONTROL **Attività**] o [!UICONTROL **Problema**].

   Vengono visualizzate le categorie dei campi disponibili per le attività o i problemi. Espandere una categoria per visualizzare tutti i campi. È inoltre possibile cercare un campo.

   ![Cerca campo personalizzato](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Non sono disponibili i seguenti tipi di campo da aggiungere alle schede: Adobe XD, Immagine, PDF, Video.

1. Selezionare il nome del campo.
1. (Facoltativo) Fai clic su nella **[!UICONTROL Valore campo]** per cambiare il campo personalizzato.
1. (Facoltativo) Modifica il **[!UICONTROL Etichetta campo]** al nome del campo che si desidera visualizzare sulle schede.
1. Una volta apportate le modifiche desiderate, fare clic su [!UICONTROL **Salva campo**].

   ![Valore campo personalizzato ed etichetta](assets/save-custom-field-value-label.png)

   Il campo personalizzato viene aggiunto all’elenco dei campi disponibili ed è abilitato per impostazione predefinita. Puoi disattivare il campo personalizzato seguendo la procedura descritta nella sezione [Configurare le schede](customize-fields-on-card.md#configure-cards) , modificare il campo o eliminarlo da tutte le schede.

>[!NOTE]
>
>Se successivamente rinominate il campo personalizzato in Workfront, è necessario modificare l’etichetta del campo nel pannello Configura in modo che corrisponda, altrimenti il campo non viene visualizzato sulle schede.
