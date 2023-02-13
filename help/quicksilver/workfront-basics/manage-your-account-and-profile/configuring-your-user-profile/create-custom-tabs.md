---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Creazione di sezioni personalizzate
description: Le informazioni visualizzate nel [!DNL Workfront] l’applicazione web viene spesso visualizzata nelle sezioni del pannello a sinistra per impostazione predefinita. Ogni sezione contiene informazioni diverse su [!DNL Workfront] area o oggetto.
author: Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 2%

---

# Creazione di sezioni personalizzate

## [!DNL Adobe Workfront] sezioni

Le informazioni visualizzate nel [!DNL Workfront] l’applicazione web viene spesso visualizzata nelle sezioni del pannello a sinistra per impostazione predefinita. Ogni sezione contiene informazioni diverse su [!DNL Workfront] area o oggetto.\
Per ulteriori informazioni sulle aree predefinite di [!DNL Workfront], vedi l&#39;articolo [Informazioni sul valore predefinito [!DNL Adobe Workfront] layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Oltre alle sezioni che vengono fornite con [!DNL Workfront] per impostazione predefinita, puoi aggiungere un dashboard in cui visualizzare informazioni rilevanti per il flusso di lavoro. Non è possibile aggiungere un dashboard a tutte le aree e a tutti gli oggetti.

Nella tabella seguente sono elencati tutti i [!DNL Workfront] aree e oggetti che contengono sezioni nel pannello a sinistra e quali di esse possono essere personalizzate:

| **[!DNL Workfront]area o oggetto** | **Sezioni di sistema predefinite** | **Sezioni personalizzate** |
|---|---|---|
| [!UICONTROL Progetti] area | ✓ | ✓ |
| [!UICONTROL Team] | ✓ |   |
| [!UICONTROL Richieste] area | ✓ |   |
| [!UICONTROL Schede temporali] area | ✓ |   |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Programma] | ✓ | ✓ |
| [!UICONTROL Progetto] | ✓ | ✓ |
| [!UICONTROL Attività] | ✓ |  ✓ |
| [!UICONTROL Problema] |  ✓ |  ✓ |
| [!UICONTROL Utente] |  ✓ |  ✓ |
| [!UICONTROL Documento] |  ✓ |  ✓ |

{style=&quot;table-layout:auto&quot;}

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
   <td> <p>[!UICONTROL Review] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td>Revisore [!UICONTROL] o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td>Visualizza l’accesso al tipo di oggetto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano o tipo di licenza hai, contatta il tuo [!DNL Workfront] amministratore.

## Aggiungi un dashboard nel pannello a sinistra di un [!DNL Workfront] oggetto o area

Prima di poter aggiungere un dashboard, è necessario creare il dashboard con tutte le informazioni che si desidera visualizzare. Puoi anche creare una pagina esterna.\
Per ulteriori informazioni sulla creazione di dashboard, consulta l’articolo [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Per ulteriori informazioni sulla creazione di pagine esterne, consulta l’articolo [Incorporare una pagina web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Dopo aver creato il dashboard o la pagina esterna, puoi aggiungerli al pannello di sinistra.

1. Vai a uno dei [!DNL Workfront] aree o oggetti in cui è possibile aggiungere una sezione personalizzata nel pannello a sinistra.\
   Oppure
1. Passa a un oggetto in cui è possibile aggiungere un [!UICONTROL dashboard] nel pannello a sinistra.\
   Per ulteriori informazioni sulle aree e sugli oggetti a cui è possibile aggiungere sezioni personalizzate, consulta [[!DNL Adobe Workfront] sezioni](#adobe-workfront-sections).
1. Fai clic su **[!UICONTROL Aggiungi dashboard]** nel pannello a sinistra.
1. Digita un nome per il dashboard nel **[!UICONTROL Nome collegamento rapido]** campo . Questo è visibile solo a voi.
1. Inizia a digitare il nome di un dashboard esistente o di una pagina esterna nel **[!UICONTROL Scegliere un dashboard]** , quindi seleziona il dashboard quando viene visualizzato nell’elenco.
1. Fai clic su **[!UICONTROL Aggiungi]**.
1. (Facoltativo) Trascina e rilascia le sezioni nell’ordine in cui desideri visualizzarle.

   La sezione superiore è la sezione predefinita per la pagina.

   Le sezioni create per i singoli oggetti vengono visualizzate quando si accede a tutti gli oggetti dello stesso tipo e sono disponibili solo per l&#39;utente.

## Visualizzare le dashboard nel pannello a sinistra degli oggetti

Per ulteriori informazioni sull’aggiunta di un dashboard sotto un oggetto, consulta la sezione . [[!UICONTROL Aggiungi un dashboard] nel pannello a sinistra di un oggetto o area Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) in questo articolo.

Quando si aggiunge un dashboard a una sezione personalizzata sotto un oggetto, l&#39;oggetto funge da filtro per il dashboard. Ad esempio, se aggiungi un rapporto attività su un dashboard e aggiungi il dashboard a un progetto, la sezione personalizzata che contiene il dashboard del progetto visualizza solo le attività sul progetto che stai visualizzando.

I seguenti oggetti vengono filtrati per l&#39;oggetto sotto il quale vengono visualizzati, se l&#39;oggetto è più gerarchia rispetto ad essi:

* Progetto
* Attività
* Problema
* Processo di approvazione
* Nota
* Documento

Per ulteriori informazioni sulla gerarchia e l’interdipendenza degli oggetti, vedere la sezione [Interdipendenza e gerarchia degli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) nell&#39;articolo [Comprendere gli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personalizzare il pannello a sinistra in un modello di layout

Quando aggiungi delle dashboard al tuo [!DNL Workfront] Per esempio, sono visibili solo a voi.

Puoi personalizzare le sezioni in [!DNL Workfront] e condividere il nuovo layout con diversi utenti in un modello di layout. Solo un amministratore di sistema o di gruppo può condividerli con altri utenti in un modello di layout. Per ulteriori informazioni sulla personalizzazione del pannello di sinistra con un modello di layout, consulta [Personalizzare il pannello a sinistra utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
