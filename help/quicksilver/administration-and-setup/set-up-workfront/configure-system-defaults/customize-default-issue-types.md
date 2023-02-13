---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Personalizzare i tipi di problemi predefiniti
description: Puoi personalizzare le etichette per ogni tipo di problema predefinito in modo che corrispondano meglio alla terminologia utilizzata nell’organizzazione. I tipi di problema sono utili per personalizzare gli stati dei problemi e creare le code di richiesta.
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

I tipi di problemi sono utili nelle seguenti circostanze:

* Quando si personalizzano gli stati dei problemi, come descritto in [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Durante la creazione di una coda di richiesta, come descritto in [Creare una coda di richiesta](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore.</p> <p><b>NOTA</b>: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipi di problemi predefiniti

Se [!DNL Adobe Workfront] [!UICONTROL amministratore] accesso, sono disponibili quattro tipi di problemi predefiniti che è possibile configurare e rinominare:

* **[!UICONTROL Report bug]** Utilizzato per tenere traccia dei bug segnalati nel sistema.
* **[!UICONTROL Cambia ordine]** Utilizzato per tenere traccia dei problemi che devono essere aggiornati o rivisti.
* **[!UICONTROL Problema]** Un oggetto in [!DNL Workfront] che comunica il lavoro non pianificato, un problema che si presenta, o qualcosa che deve essere risolto per continuare un compito.
* **[!UICONTROL Richiesta]** Tipo di problema che si applica a una coda di richiesta in cui gli utenti effettuano richieste in Workfront.

![](assets/default-issue-types.png)

## Personalizzare un tipo di problema

Per personalizzare i tipi di problema, considera quanto segue:

* Puoi modificare l’etichetta per un tipo di problema, ma non puoi modificarne la funzione.
* Non puoi creare altri tipi di problemi.
* Non è possibile modificare i valori del filtro per il nome di un tipo di problema. Quindi, se crei un filtro su un report del problema, il valore del filtro (chiave) non riflette il nome personalizzato del tipo di problema.
* A ogni tipo di problema sono associati tre stati predefiniti: [!UICONTROL Nuovo], [!UICONTROL In corso]e [!UICONTROL Chiuso]. Non è possibile eliminare o rimuovere questi stati da un tipo di problema, ma è possibile rinominarli.
* Puoi riordinare le opzioni visualizzate nel menu a discesa per ogni tipo di problema.

Per personalizzare un tipo di problema:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Preferenze del progetto]** > **[!UICONTROL Stati]**.

1. Fai clic sul pulsante **[!UICONTROL Problemi]** scheda .
1. Effettua una delle seguenti operazioni:

   * Passa il puntatore del mouse sul tipo di problema che desideri personalizzare, fai clic sul pulsante [!UICONTROL Modifica] icona ![](assets/edit-icon.png) all&#39;estrema destra, quindi digita un nuovo nome per il tipo di problema.

      ![](assets/customize-issue-type.png)

   * Fai clic su [!UICONTROL tipo di problema] per elencare gli stati associati, trascina le maniglie visualizzate quando passi il cursore sopra di esse e rilasciale nell’ordine in cui desideri che vengano visualizzate nel problema degli utenti **[!UICONTROL Stato]** menu a discesa.
