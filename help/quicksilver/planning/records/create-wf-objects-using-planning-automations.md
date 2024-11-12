---
title: Creazione di oggetti Workfront mediante le automazioni dei record di Workfront Planning
description: In Workfront Planning è possibile configurare automazioni che, se attivate, creano oggetti in Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: d8631e16234486479aa70233aa3770b28ea0d218
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---


# Creazione di oggetti Workfront mediante le automazioni dei record di Workfront Planning

In Workfront Planning è possibile configurare automazioni che, se attivate, creano oggetti in Workfront.

L’automazione viene attivata nei record. L&#39;oggetto in Workfront è connesso al record Planning in cui è stata attivata l&#39;automazione.

Ad esempio, è possibile creare un&#39;automazione che accetta una campagna di Workfront Planning e crea un progetto in Workfront per tenere traccia dell&#39;avanzamento della campagna. Il progetto sarà collegato alla campagna di pianificazione di Workfront.

Per ulteriori informazioni sui record connessi, vedere [Panoramica sui record connessi](/help/quicksilver/planning/records/connected-records-overview.md).


## Configurare un&#39;automazione in Workfront Planning

È necessario configurare un&#39;automazione in Workfront Planning prima di poterla utilizzare per creare oggetti di Workfront.

1. Fare clic sul menu **Altro** ![](assets/more-menu.png) e selezionare **Automazioni**.

   Viene visualizzato l’elenco delle automazioni disponibili.

1. Fai clic su **Crea nuova automazione** nell&#39;angolo superiore destro dello schermo.
1. Nel campo **Testo pulsante** immettere il testo che si desidera visualizzare sul pulsante. Gli utenti faranno clic su questo pulsante quando utilizzano l’automazione per creare un oggetto Workfront.
1. (Facoltativo) Per aggiungere un’icona al pulsante, seleziona un’icona tra le opzioni disponibili.
1. Nel campo **Crea un tipo di**, selezionare l&#39;oggetto che si desidera creare con l&#39;automazione.

   Gli oggetti disponibili sono:

   * Progetto
   * Portfolio
   * Programma
   * Gruppo

1. In **Selezionare il campo da utilizzare nel campo nome progetto**, selezionare un campo record. Il nuovo progetto in Workfront avrà come nome il contenuto di questo campo.
1. Nel campo **Seleziona il campo per ricollegare il progetto creato**, seleziona un campo record. Il nuovo progetto in Workfront verrà visualizzato in questo campo quando si visualizza il record in Workfront Planning.
1. Selezionare le altre opzioni disponibili per il tipo di oggetto che si sta creando.
1. Fai clic su **Crea**

L’automazione viene visualizzata nell’elenco delle automazioni ed è disponibile per l’utilizzo nei record.

## Utilizzare un&#39;automazione di Workfront Planning per creare un oggetto Workfront

1. In Workfront Planning aprire la pagina del tipo di record contenente i record che si desidera utilizzare per creare oggetti Workfront.
1. Selezionare uno o più record.
1. Fai clic sul pulsante di automazione nell’angolo inferiore destro dello schermo.

   In questo esempio, si tratta del pulsante Crea progetto.

   ![Pulsante di automazione](assets/automation-custom-button.png)

>[!NOTE]
>
>È consigliabile verificare che l&#39;oggetto sia stato creato e connesso come previsto.

