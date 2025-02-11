---
content-type: reference
navigation-topic: search
title: Utilizza il numero di riferimento degli oggetti
description: In [!DNL Adobe Workfront] gli elementi sono identificati come oggetti. Gli oggetti corrispondono al database e vengono utilizzati per correlare i dati con un elemento. I numeri di riferimento sono utili per distinguere due oggetti altrimenti simili, ad esempio attività con lo stesso nome. Puoi cercare i numeri di riferimento e includerli nei rapporti.
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Utilizza il numero di riferimento degli oggetti

In [!DNL Adobe Workfront] gli elementi sono identificati come oggetti. Gli oggetti corrispondono al database e vengono utilizzati per correlare i dati con un elemento.

Workfront assegna automaticamente a ciascuno dei seguenti oggetti un numero di riferimento univoco al momento della creazione dell&#39;oggetto:

* Progetti
* Attività
* Problemi
* Documenti

I numeri di riferimento sono utili per distinguere due oggetti altrimenti simili, ad esempio attività con lo stesso nome. Puoi cercare i numeri di riferimento e includerli nei rapporti.

>[!IMPORTANT]
>
>* [!DNL Workfront] assegna numeri di riferimento in modo continuo a tutti i clienti e a tutti gli oggetti. Ad esempio, quando si crea un&#39;attività, [!DNL Workfront] potrebbe assegnarle un numero di riferimento di 00005. Se un altro cliente crea successivamente un progetto, il progetto potrebbe ricevere il successivo numero di riferimento disponibile, ad esempio 00006. Se si crea un problema successivamente, il problema potrebbe ricevere il numero di riferimento 00007 e così via.
>* Non è possibile controllare la sequenza dei numeri di riferimento per gli oggetti in [!DNL Workfront]. La sequenza è sempre controllata dal nostro database.
>



## Visualizzare il numero di riferimento di un oggetto

I numeri di riferimento vengono visualizzati per impostazione predefinita per le attività e i problemi. È inoltre possibile configurare facilmente [!DNL Workfront] per visualizzare i numeri di riferimento per altri tipi di oggetti.

* [Visualizza numeri di riferimento per attività e problemi](#view-reference-numbers-for-tasks-and-issues)
* [Visualizza numeri di riferimento per altri oggetti](#view-reference-numbers-for-other-objects)
* [Visualizzare i numeri di riferimento nei rapporti](#view-reference-numbers-in-reports)

### Visualizza numeri di riferimento per attività e problemi

I numeri di riferimento vengono visualizzati per impostazione predefinita quando si visualizza un’attività o un problema.  Per visualizzare il numero di riferimento, fai clic su **[!UICONTROL Dettagli attività]** o **[!UICONTROL Dettagli problema]** nel pannello a sinistra, quindi individua la sezione **[!UICONTROL Informazioni di base]** nella panoramica.

![Numero di riferimento](assets/reference-number-nwe-350x184.png)

### Visualizza numeri di riferimento per altri oggetti

Per visualizzare i numeri di riferimento per gli oggetti, è possibile creare una visualizzazione personalizzata o modificare una visualizzazione esistente e aggiungere il campo [!UICONTROL Numero di riferimento] a una colonna della visualizzazione. Ad esempio, puoi modificare la visualizzazione [!UICONTROL Progetti] per visualizzare il numero di riferimento per tutti i tuoi progetti.

Per informazioni su come creare o modificare una visualizzazione, vedere [Panoramica delle visualizzazioni in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Visualizzare i numeri di riferimento nei rapporti

È possibile visualizzare il numero di riferimento per gli oggetti nei report aggiungendo la colonna [!UICONTROL Numero di riferimento] al report.

Per informazioni su come aggiungere una colonna a un report, vedere [Creare un report personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Cerca un oggetto per numero di riferimento

[!DNL Workfront] consente di cercare un oggetto per numero di riferimento.

Digitare il numero di riferimento di un oggetto nel campo **[!UICONTROL Ricerca]**, quindi premere **[!UICONTROL Invio]**.

Per ulteriori informazioni sulla ricerca in Workfront, vedere [Ricerca [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
