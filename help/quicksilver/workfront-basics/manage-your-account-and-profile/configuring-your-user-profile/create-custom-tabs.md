---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Aggiungere un dashboard nel pannello sinistro di un oggetto o di un'area Workfront
description: Per impostazione predefinita, le informazioni visualizzate nell'applicazione Web  [!DNL Workfront]  vengono spesso visualizzate nelle sezioni nel pannello sinistro. Ogni sezione contiene informazioni diverse su un'area o un oggetto  [!DNL Workfront] .
author: Becky and Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 4%

---

# Aggiungere un dashboard nel pannello sinistro di un oggetto o di un&#39;area Workfront

## [!DNL Adobe Workfront] sezioni

Per impostazione predefinita, le informazioni visualizzate nell&#39;applicazione Web [!DNL Workfront] vengono spesso visualizzate nelle sezioni del pannello sinistro. Ogni sezione contiene informazioni diverse su un&#39;area o un oggetto [!DNL Workfront].

Per ulteriori informazioni sulle aree predefinite di [!DNL Workfront], vedere l&#39;articolo [Informazioni sul layout predefinito [!DNL Adobe Workfront] &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Oltre alle sezioni fornite con [!DNL Workfront] per impostazione predefinita, è possibile aggiungere una dashboard in cui visualizzare informazioni rilevanti per il flusso di lavoro. Non è possibile aggiungere un dashboard a tutte le aree e a tutti gli oggetti.

Nella tabella seguente sono elencate tutte le aree e gli oggetti [!DNL Workfront] che contengono sezioni nel pannello sinistro e quali di essi possono essere personalizzati con un dashboard:

| **[!DNL Workfront]area o oggetto** | **Sezioni di sistema predefinite** | **Dashboard** |
|---|---|---|
| Area [!UICONTROL Progetti] | ✓ | ✓ |
| [!UICONTROL Team] | ✓ |    |
| Area [!UICONTROL Richieste] | ✓ |    |
| Area [!UICONTROL Schede orario] | ✓ |    |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Programma] | ✓ | ✓ |
| [!UICONTROL Progetto] | ✓ | ✓ |
| [!UICONTROL Attività] | ✓ | ✓ |
| [!UICONTROL Problema] | ✓ | ✓ |
| [!UICONTROL Utente] | ✓ | ✓ |
| [!UICONTROL Documento] | ✓ | ✓ |
| [!UICONTROL Area risorse] | ✓ | ✓ |

{style="table-layout:auto"}

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>
   <p>Chiaro o superiore</p>
   <p>Revisione o successiva</p></td>
  </tr> 
  <tr> 
   <td>Autorizzazioni oggetto</td> 
   <td><p>Accesso di visualizzazione al tipo di oggetto</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiungere un dashboard nel pannello sinistro di un oggetto o di un&#39;area [!DNL Workfront]

Prima di aggiungere una dashboard, è necessario crearla con tutte le informazioni che si desidera visualizzare. Puoi anche creare una pagina esterna.

Per ulteriori informazioni sulla creazione di dashboard, vedere l&#39;articolo [Creare un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Per ulteriori informazioni sulla creazione di pagine esterne, vedere l&#39;articolo [Incorporare una pagina Web esterna in un dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Dopo aver generato il dashboard o la pagina esterna, puoi aggiungerli al pannello sinistro.

1. Passare a una delle aree o degli oggetti [!DNL Workfront] in cui è possibile aggiungere un dashboard nel pannello sinistro.

   Per ulteriori informazioni sulle aree e sugli oggetti a cui è possibile aggiungere dashboard, vedere [[!DNL Adobe Workfront] sezioni](#adobe-workfront-sections).

1. Fai clic su **[!UICONTROL Aggiungi dashboard]** nel pannello a sinistra.
1. Digitare un nome per il dashboard nel campo **[!UICONTROL Nome collegamento rapido]**. Questo è visibile solo a te.
1. Inizia a digitare il nome di un dashboard o di una pagina esterna esistente nel campo **[!UICONTROL Scegli un dashboard]**, quindi seleziona il dashboard quando viene visualizzato nell&#39;elenco.
1. Fai clic su **[!UICONTROL Aggiungi]**.
1. (Facoltativo) Trascina le sezioni nell’ordine in cui desideri visualizzarle.

   La sezione superiore è la sezione predefinita della pagina.

   Le dashboard aggiunte sono disponibili solo per te.

## Visualizza dashboard nel pannello sinistro degli oggetti

Per ulteriori informazioni sull&#39;aggiunta di un dashboard in un oggetto, vedere la sezione [[!UICONTROL Aggiungere un dashboard] nel pannello sinistro di un oggetto o di un&#39;area Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) in questo articolo.

Quando aggiungete un dashboard al pannello sinistro di un oggetto, l&#39;oggetto funge da filtro per il dashboard. Se ad esempio si aggiunge un report attività a un dashboard e si aggiunge il dashboard a un progetto, nel dashboard verranno visualizzate solo le attività del progetto visualizzato.

I seguenti oggetti vengono filtrati per l&#39;oggetto sotto il quale vengono visualizzati, se l&#39;oggetto è più alto nella gerarchia:

* Progetto
* Attività
* Problema
* Processo di approvazione
* Nota
* Documento

Per ulteriori informazioni sulla gerarchia e sull&#39;interdipendenza degli oggetti, vedere la sezione [Interdipendenza e gerarchia degli oggetti](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) nell&#39;articolo [Informazioni sugli oggetti in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personalizzare il pannello sinistro in un modello di layout

Le dashboard aggiunte all&#39;istanza [!DNL Workfront] sono visibili solo all&#39;utente.

Solo un amministratore di sistema o di gruppo può condividere i dashboard con altri utenti in un modello di layout. Per ulteriori informazioni sulla personalizzazione del pannello sinistro con un modello di layout, vedere [Personalizzare il pannello sinistro utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
