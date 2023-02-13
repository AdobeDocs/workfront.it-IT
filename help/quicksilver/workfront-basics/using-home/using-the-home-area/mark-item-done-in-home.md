---
product-area: projects
navigation-topic: use-the-home-area
title: Contrassegna un elemento come Fatto nell'area Home
description: È possibile contrassegnare un'attività o un problema come Fatto se si è l'attività o il problema assegnatario. Quando si contrassegna un'attività o un problema come Fine, lo stato dell'attività o del problema viene modificato in Completa.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# Contrassegna elemento come [!UICONTROL Fine] in [!UICONTROL Pagina principale] area

È possibile contrassegnare un&#39;attività o un problema come Fatto se si è l&#39;attività o il problema assegnatario. Quando contrassegni un’attività o un problema come [!UICONTROL Fine], lo stato dell’attività o del problema viene modificato in [!UICONTROL Completa].

>[!NOTE]
>
>Non viene visualizzata la [!UICONTROL Fine] a meno che tu non sia una delle risorse assegnate all&#39;attività o al problema.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licenza*</strong></td> 
   <td> <p>[!UICONTROL Work] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso*</strong></td> 
   <td> <p>Accesso a attività e problemi con [!UICONTROL Edit]</p> <p>Nota: Se non hai ancora accesso, chiedi [!DNL Workfront] amministratore se imposta ulteriori restrizioni nel livello di accesso. Per informazioni su come [!DNL Workfront] l'amministratore può modificare il livello di accesso, vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorizzazioni oggetto</strong></td> 
   <td> <p>Autorizzazioni di Contribute o superiori alle attività e ai problemi su cui lavorare</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Contrassegnare un&#39;attività o un problema come [!UICONTROL Fine]

Solo l’utente assegnato all’attività o al problema può contrassegnarlo come [!UICONTROL Fine].

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** ![](assets/main-menu-icon.png) nell&#39;angolo in alto a destra, quindi fai clic su **[!UICONTROL Pagina principale]**.
1. In **[!UICONTROL Elenco lavori]**, individua uno degli elementi su cui lavorare.
1. Effettua una delle seguenti operazioni:

* Fai clic su **[!UICONTROL Fine]** sull&#39;elemento di lavoro.\
   Vedi [Comprendere le opzioni del [!UICONTROL Fine] pulsante](#understand-the-options-of-the-done-button) per informazioni più dettagliate su come potrebbe essere visualizzato questo pulsante.

* Seleziona l&#39;elemento da contrassegnare come completato, quindi fai clic su nel pannello di destra **[!UICONTROL Aggiorna stato]**, quindi cambia lo stato dell&#39;elemento in uno stato che corrisponde a [!UICONTROL Completa] o [!UICONTROL Chiuso].

## Comprendere le opzioni del [!UICONTROL Fine] pulsante

Per impostazione predefinita, fai clic sul pulsante [!UICONTROL Fine] il pulsante su un elemento di lavoro cambia lo stato di tale elemento in [!UICONTROL Completa] (per compiti) o [!UICONTROL Risolto] (per questioni).

Le [!DNL Adobe Workfront] l&#39;amministratore può personalizzare gli stati associati al [!UICONTROL Fine] e applicare tali personalizzazioni al team principale.

A seconda del numero di stati associati al [!UICONTROL Fine] o quante risorse sono assegnate all&#39;attività o al problema, l&#39;aspetto della [!UICONTROL Fine] può cambiare.

* [[!UICONTROL Fine] pulsante associato a uno stato](#done-button-associated-with-one-status)
* [[!UICONTROL Fine] pulsante associato a più stati](#done-button-associated-with-multiple-statuses)
* [[!UICONTROL Fine] pulsante per gli elementi assegnati a più risorse](#done-button-for-items-assigned-to-multiple-resources)

### [!UICONTROL Fine] pulsante associato a uno stato

Quando il [!UICONTROL Fine] il pulsante è associato a uno stato e l&#39;elemento di lavoro è assegnato solo a te, il pulsante legge **[!UICONTROL Fine]**. Quando fai clic su di esso, lo stato dell’attività o del problema viene modificato in quello associato al [!UICONTROL Fine] pulsante .

![Pulsante Fine](assets/Done.png)

Per capire quale stato è associato al [!UICONTROL Fine] controlla il pulsante [!UICONTROL Impostazioni team] della tua Home Team per [!UICONTROL Pulsante Fine] come descritto in [Modificare le impostazioni del team](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

Se non sei assegnato a un team principale, quando fai clic su viene selezionato lo stato predefinito [!UICONTROL Fine], come descritto in precedenza in [Comprendere le opzioni del [!UICONTROL Fine] pulsante](#understand-the-options-of-the-done-button).

### [!UICONTROL Fine] pulsante associato a più stati

Quando il [!UICONTROL Fine] il pulsante è associato a più di uno stato; il pulsante mostra la parola **[!UICONTROL Fine]** seguita da un menu a discesa. In questo scenario, non puoi semplicemente fare clic su [!UICONTROL Fine]. È necessario selezionare uno stato dal menu a discesa. Selezionare lo stato più adatto al completamento dell&#39;elemento di lavoro. In questo modo si cambia lo stato dell&#39;elemento di lavoro.

Per comprendere come associare più stati a [!UICONTROL Fine] pulsante vedi [Configura le [!UICONTROL Fine] pulsante per le attività](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) e [Configura le [!UICONTROL Fine] pulsante per problemi](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### [!UICONTROL Fine] pulsante per gli elementi assegnati a più risorse

Quando l’attività o il problema viene assegnato a più di una risorsa, il pulsante mostra la parola **[!UICONTROL Fine]** seguita da un menu a discesa. Nel menu a discesa, puoi scegliere tra **[!UICONTROL Fatto con la mia parte]** (che consente ai membri del team di sapere che la parte dell’attività è completa) o lo stato associato al [!UICONTROL Fine] pulsante (che completa l’elemento). Dopo aver selezionato **[!UICONTROL Fatto con la mia parte]**, l’elemento di lavoro viene rimosso dall’elenco di lavoro, ma rimane nell’elenco di lavoro di quelli ancora assegnati all’elemento di lavoro.\
Se il pulsante Fine è associato a più stati, sono elencati in **Fatto con la mia parte**.

>[!NOTE]
>
>In un&#39;attività o in un problema con più assegnatari, ogni utente è responsabile di indicare che la propria assegnazione sull&#39;attività o sul problema è stata effettivamente completata. Per questo motivo, ogni assegnatario deve fare clic su [!UICONTROL Fine] per mostrare di aver completato il lavoro assegnato loro sull&#39;elemento.

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
