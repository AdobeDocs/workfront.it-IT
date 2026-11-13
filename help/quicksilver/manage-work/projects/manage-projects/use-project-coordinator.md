---
title: Utilizza il collaboratore di Project Coordinator
content-type: reference
description: Scopri come utilizzare Project Coordinator, un collaboratore AI pronto all’uso che monitora lo stato del progetto e dà seguito alle attività scadute.
author: Becky
feature: Work Management, Projects
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 6%

---
# Utilizza il collaboratore di Project Coordinator

{{highlighted-preview-article-level}}

Il coordinatore del progetto è un collaboratore AI pronto all’uso che monitora il progetto e informa le parti interessate in merito a importanti informazioni sullo stato.

L’utilizzo di un coordinatore di progetto non richiede la configurazione di un agente al di fuori di Workfront.

Per istruzioni sulla configurazione di un coordinatore di progetto, vedere [Configurare un coordinatore di progetto](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) nell&#39;articolo Configurare i collaboratori di IA.

Per informazioni sui collaboratori IA in genere, vedere [Configurare i collaboratori IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Seleziona, Prime o Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Per assegnare un coordinatore di progetto è necessario disporre dell'autorizzazione Gestione per i progetti.</td> 
  </tr>
  </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Panoramica di Project Coordinator

Il coordinatore del progetto monitora il progetto e aiuta a mantenere il lavoro sulla strada giusta. Quando viene assegnato a un progetto, invia gli aggiornamenti del progetto in base a una pianificazione configurata dall’amministratore. Gli aggiornamenti possono includere:

* Riepilogo dei progressi compiuti
* Stato del progetto
* Attività o approvazioni scadute o a rischio
* Campi o assegnazioni mancanti

Il coordinatore del progetto può anche commentare il progetto e le sue attività.

L’amministratore configura la frequenza con cui vengono inviati gli aggiornamenti, l’ora in cui vengono inviati e chi li riceve.

Puoi anche eseguire Project Coordinator on demand menzionandolo in un aggiornamento del progetto. Il coordinatore del progetto viene eseguito quando è menzionato, anche se non è pianificato per l’esecuzione in tale momento.

>[!NOTE]
>
>Il comportamento del coordinatore del progetto può cambiare prima della disponibilità generale.

## Aggiungere il coordinatore del progetto a un progetto

Un amministratore deve innanzitutto creare il coordinatore del progetto e aggiungere il campo **Coordinatore del progetto** all&#39;intestazione del progetto nel modello di layout. Il campo viene quindi visualizzato nell’intestazione del progetto.

Per ulteriori informazioni, vedere [Personalizzare le intestazioni degli oggetti utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

Per assegnare un coordinatore di progetto a un progetto:

1. Passare al progetto per il quale si desidera assegnare un coordinatore di progetto.
1. Nell&#39;intestazione del progetto fare clic sul campo **Coordinatore progetto**.
1. Selezionare il coordinatore del progetto che si desidera assegnare.

   Nella finestra viene visualizzata una descrizione del coordinatore di progetto selezionato, nonché le azioni eseguite dal coordinatore di progetto.
1. Fai clic su **Applica**.

## Esegui il coordinatore del progetto menzionandolo

Oltre agli aggiornamenti pianificati, puoi attivare il coordinatore del progetto in qualsiasi momento @mentioning in un aggiornamento del progetto. Il coordinatore del progetto viene eseguito non appena menzionato, anche se non è pianificato per l’esecuzione in tale momento.

Per citare il coordinatore del progetto:

1. Vai al progetto a cui è assegnato il coordinatore del progetto.
1. Apri l&#39;area **Aggiornamenti** del progetto.
1. Nel campo di aggiornamento, digitare **@** e selezionare il coordinatore del progetto.
1. Aggiungi il messaggio, quindi pubblica l’aggiornamento.

   Il coordinatore del progetto esegue e pubblica la sua risposta.

>[!NOTE]
>
>Il coordinatore del progetto deve essere assegnato al progetto prima che tu possa attivarlo con un @mention.

## Configurare il coordinatore del progetto

Per istruzioni sulla configurazione di Project Coordinator, vedere [Configurare Project Coordinator](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) nell&#39;articolo Configurare i collaboratori AI.
