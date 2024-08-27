---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personalizzare i campi visualizzati su una scheda
description: È possibile personalizzare i campi visualizzati su una scheda disattivando un campo in modo che non venga visualizzato nella visualizzazione a schede complete o ridotta oppure nascondendo un campo nella visualizzazione a schede ridotta.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '667'
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

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> 
   <p>Nuovo: [!UICONTROL Contributor] o versione successiva</p> 
   <p>oppure</p>
   <p>Corrente: [!UICONTROL Request] o versione successiva</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare le schede {#configure-cards}

{{step1-to-boards}}

1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fai clic su [!UICONTROL **Configura**] a destra della bacheca per aprire il pannello Configura.
1. Espandi [!UICONTROL **Schede**].

   La maggior parte dei campi e delle sezioni è attivata per impostazione predefinita.

1. Disattiva un campo o una sezione per disattivarla in entrambe le visualizzazioni a schede.
1. Fare clic sull&#39;icona Nascondi ![Icona Nascondi](assets/eye-hide-icon.png) accanto a un campo o a una sezione per nasconderlo nella visualizzazione ridotta.
1. Per visualizzare tutti i campi e le sezioni in entrambe le visualizzazioni, fare clic su [!UICONTROL **Ripristina tutti i campi sul valore predefinito**].
1. Fai clic su [!UICONTROL **Nascondi configurazione**] per chiudere il pannello Configura.

## Aggiungere campi personalizzati alle schede

I campi personalizzati sono disponibili sulle schede collegate. Sono visibili solo nella vista a schede completa, non nella vista a condensa sulla bacheca.

I dati sui campi personalizzati sono modificabili sulla scheda, anche se alcuni elementi personalizzati potrebbero essere disponibili per la modifica solo sul campo originale e non sulla scheda.

1. Accedi a una bacheca e fai clic su [!UICONTROL **Configura**] per aprire il pannello Configura.
1. Espandi [!UICONTROL **Schede**].
1. In [!UICONTROL Campi scheda], fai clic su [!UICONTROL **Aggiungi campo personalizzato**].
1. Seleziona [!UICONTROL **Attività**] o [!UICONTROL **Problema**].

   Vengono visualizzate le categorie dei campi disponibili per le attività o i problemi. Espandere una categoria per visualizzare tutti i campi. È inoltre possibile cercare un campo.

   ![Cerca campo personalizzato](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Non sono disponibili i seguenti tipi di campo da aggiungere alle schede: Adobe XD, Immagine, PDF, Video.

1. Selezionare il nome del campo.
1. (Facoltativo) Fai clic nel campo **[!UICONTROL Valore campo]** per modificare il campo personalizzato in un altro.
1. (Facoltativo) Modifica l&#39;**[!UICONTROL etichetta campo]** con il nome del campo che desideri visualizzare sulle schede.
1. Dopo aver apportato le modifiche desiderate, fare clic su [!UICONTROL **Salva campo**].

   ![Etichetta e valore campo personalizzato](assets/save-custom-field-value-label.png)

   Il campo personalizzato viene aggiunto all’elenco dei campi disponibili ed è abilitato per impostazione predefinita. Puoi disabilitare il campo personalizzato seguendo i passaggi descritti nella sezione [Configurare le schede](customize-fields-on-card.md#configure-cards) precedente, modificare il campo o eliminarlo da tutte le schede.

>[!NOTE]
>
>Se successivamente rinominate il campo personalizzato in Workfront, è necessario modificare l’etichetta del campo nel pannello Configura in modo che corrisponda, altrimenti il campo non viene visualizzato sulle schede.

## Visualizzare o nascondere le schede archiviate

È necessario attivare un&#39;impostazione di configurazione per visualizzare le schede archiviate su una bacheca.

1. Accedi a una bacheca e fai clic su [!UICONTROL **Configura**] per aprire il pannello Configura.
1. Espandi [!UICONTROL **Schede**].
1. Attiva [!UICONTROL **Visualizza schede archiviate sulla bacheca**].

   Ora puoi filtrare la bacheca per mostrare tutte le schede che sono state archiviate. Per ulteriori dettagli, vedere [Filtrare ed eseguire ricerche in una bacheca](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

1. Fai clic su [!UICONTROL **Nascondi configurazione**] per chiudere il pannello Configura.

## Configurare la perdita di dati della scheda

Per rimuovere automaticamente le schede dalla bacheca dopo un certo periodo di tempo, vedi [Configurare la perdita di dati delle schede](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).
