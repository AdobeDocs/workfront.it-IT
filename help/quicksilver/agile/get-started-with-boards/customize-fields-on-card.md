---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personalizzare i campi visualizzati su una scheda
description: È possibile personalizzare i campi visualizzati su una scheda disattivando un campo in modo che non venga visualizzato nella visualizzazione a schede complete o ridotta oppure nascondendo un campo nella visualizzazione a schede ridotta.
author: Courtney
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 7%

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
>Eventuali personalizzazioni dei campi applicate solo alla bacheca in cui stai lavorando.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o successiva</p> 
   <p>Richiedente o successiva</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare le schede {#configure-cards}

{{step1-to-boards}}

1. Accedi a una bacheca. Per informazioni, consulta [Creare o modificare una bacheca](../../agile/get-started-with-boards/create-edit-board.md).
1. Fai clic su [!UICONTROL **Configura**] a destra della bacheca per aprire il pannello Configura.
1. Espandi [!UICONTROL **Schede**].

   La maggior parte dei campi e delle sezioni è attivata per impostazione predefinita.

1. Disattiva un campo o una sezione per disattivarla in entrambe le visualizzazioni a schede.
1. Fare clic sull&#39;icona Nascondi ![Icona Nascondi](assets/eye-hide-icon.png) accanto a un campo o a una sezione per nasconderlo nella visualizzazione condensata.
1. Per visualizzare tutti i campi e le sezioni in entrambe le visualizzazioni, fare clic su [!UICONTROL **Ripristina tutti i campi sul valore predefinito**].
1. Fai clic su [!UICONTROL **Nascondi configurazione**] per chiudere il pannello Configura.

## Aggiungere campi personalizzati alle schede

I campi personalizzati sono disponibili sulle schede collegate. Sono visibili solo nella vista a schede completa, non nella vista a condensa sulla bacheca.

I dati sui campi personalizzati sono modificabili sulla scheda, anche se alcuni elementi personalizzati potrebbero essere disponibili per la modifica solo sul campo originale e non sulla scheda.

1. Accedi a una bacheca e fai clic su [!UICONTROL **Configura**] per aprire il pannello Configura.
1. Espandere [!UICONTROL **Schede**].
1. In [!UICONTROL Campi carta], fai clic su [!UICONTROL **Aggiungi campo personalizzato**].
1. Selezionare [!UICONTROL **Attività**] o [!UICONTROL **Problema**].

   Vengono visualizzate le categorie dei campi disponibili per le attività o i problemi. Espandere una categoria per visualizzare tutti i campi. È inoltre possibile cercare un campo.

   ![Cerca campo personalizzato](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >I seguenti tipi di campo non sono disponibili per l’aggiunta alle schede: Adobe XD, Image, PDF, Video.

1. Selezionare il nome del campo.
1. (Facoltativo) Fare clic nel campo **[!UICONTROL Valore campo]** per cambiare il campo personalizzato.
1. (Facoltativo) Modificare l&#39;**[!UICONTROL etichetta del campo]** nel nome del campo che si desidera visualizzare sulle schede.
1. Dopo aver apportato le modifiche desiderate, fare clic su [!UICONTROL **Salva campo**].

   ![Etichetta e valore campo personalizzato](assets/save-custom-field-value-label.png)

   Il campo personalizzato viene aggiunto all’elenco dei campi disponibili ed è abilitato per impostazione predefinita. Puoi disabilitare il campo personalizzato seguendo i passaggi descritti nella sezione [Configurare le schede](customize-fields-on-card.md#configure-cards) precedente, modificare il campo o eliminarlo da tutte le schede.

>[!NOTE]
>
>Se successivamente rinominate il campo personalizzato in Workfront, dovete modificare l’etichetta del campo nel pannello Configura in modo che corrisponda, altrimenti il campo non verrà visualizzato sulle schede.

## Visualizzare o nascondere le schede archiviate

È necessario attivare un&#39;impostazione di configurazione per visualizzare le schede archiviate su una bacheca.

1. Accedi a una bacheca e fai clic su [!UICONTROL **Configura**] per aprire il pannello Configura.
1. Espandere [!UICONTROL **Schede**].
1. Attiva [!UICONTROL **Visualizza schede archiviate sulla scheda**].

   Ora puoi filtrare la bacheca per visualizzare tutte le schede archiviate. Per i dettagli, consulta [Filtrare e cercare in una bacheca](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

1. Fai clic su [!UICONTROL **Nascondi configurazione**] per chiudere il pannello Configura.

## Configurare la perdita di dati della scheda

Per rimuovere automaticamente le schede dalla bacheca dopo un determinato periodo di tempo, vedere [Configurazione del decadimento delle schede](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).
