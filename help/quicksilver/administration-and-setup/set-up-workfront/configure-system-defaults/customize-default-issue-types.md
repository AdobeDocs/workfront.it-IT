---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Personalizzare i tipi di problemi predefiniti
description: Puoi personalizzare le etichette per ogni tipo di problema predefinito in modo che corrispondano meglio alla terminologia utilizzata nell’organizzazione. I tipi di problema sono utili per personalizzare gli stati dei problemi e creare code di richieste.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Personalizzare i tipi di problemi predefiniti

I tipi di problema sono utili nelle seguenti circostanze:

* Durante la personalizzazione degli stati del problema, come descritto in [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Durante la creazione di una coda di richieste, come descritto in [Creare una coda di richieste](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Puoi personalizzare le etichette per ogni tipo di problema predefinito in modo che corrispondano meglio alla terminologia utilizzata nell’organizzazione.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore [!DNL Workfront].</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di [!DNL Workfront] se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di [!DNL Workfront] può modificare il tuo livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipi di problemi predefiniti

Se disponi dell&#39;accesso [!DNL Adobe Workfront] [!UICONTROL amministratore], puoi configurare e rinominare quattro tipi di problemi predefiniti:

* **[!UICONTROL Rapporto bug]** utilizzato per tenere traccia dei bug segnalati nel sistema.
* **[!UICONTROL Ordine di modifica]** utilizzato per tenere traccia dei problemi che devono essere aggiornati o rivisti.
* **[!UICONTROL Problema]** Oggetto in [!DNL Workfront] che comunica il lavoro non pianificato, un problema che si verifica o un problema che deve essere risolto per continuare un&#39;attività.
* **[!UICONTROL Richiesta]** Un tipo di problema che si applica a una coda di richieste in cui gli utenti effettuano richieste in Workfront.

![](assets/default-issue-types.png)

## Personalizzare un tipo di problema

Considera quanto segue sulla personalizzazione dei tipi di problema:

* È possibile modificare l’etichetta di un tipo di problema, ma non la sua funzione.
* Non è possibile creare altri tipi di problemi.
* Non puoi modificare i valori del filtro per il nome di un tipo di problema. Pertanto, se crei un filtro per un report sui problemi, il valore del filtro (chiave) non riflette il nome personalizzato del tipo di problema.
* A ogni tipo di problema sono associati tre stati predefiniti: [!UICONTROL Nuovo], [!UICONTROL In corso] e [!UICONTROL Chiuso]. Non è possibile eliminare o rimuovere questi stati da un tipo di problema, ma è possibile rinominarli.
* Puoi riordinare le opzioni visualizzate nel menu a discesa per ciascun tipo di problema.

Per personalizzare un tipo di problema:

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Preferenze progetto]** > **[!UICONTROL Stati]**.

1. Fai clic sulla scheda **[!UICONTROL Issues]**.
1. Effettua una delle seguenti operazioni:

   * Passa il puntatore del mouse sul tipo di problema che desideri personalizzare, fai clic sull&#39;icona [!UICONTROL Modifica] ![](assets/edit-icon.png) che appare all&#39;estrema destra, quindi digita un nuovo nome per il tipo di problema.

     ![](assets/customize-issue-type.png)

   * Fai clic su un [!UICONTROL tipo di problema] per elencare i relativi stati associati, quindi trascina gli handle visualizzati al passaggio del mouse su di essi e rilasciali nell&#39;ordine in cui desideri che vengano visualizzati nel menu a discesa dei problemi degli utenti **[!UICONTROL Stato]**.
