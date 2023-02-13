---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Installare una blueprint
description: Puoi installare una blueprint nell’ambiente di produzione o in un ambiente Sandbox.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Installare una blueprint

Puoi installare una blueprint nell’ambiente di produzione o in un ambiente Sandbox.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] piano</strong></td> 
   <td> <p> Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licenza</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni a livello di accesso</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dove devo installare un modello? {#where-should-i-install-a-blueprint}

Puoi installare il pacchetto in uno dei seguenti ambienti:

<table style="table-layout:auto">
        <tr>
        <td><strong>Produzione</strong></td>
        <td>La produzione è il tuo ambiente live.</td>
    </tr>
    <tr>
        <td><strong>Anteprima Sandbox</strong></td>
        <td>L’anteprima sandbox è un ambiente di test che funge da replica dell’ambiente live e viene aggiornata ogni fine settimana da Workfront. Tutti i pacchetti di supporto hanno accesso all’anteprima Sandbox. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">La [!DNL Adobe Workfront] Ambiente sandbox di anteprima</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 e 2</strong></td>
        <td>La Sandbox di aggiornamento personalizzato è un ambiente di test separato che viene aggiornato manualmente dall’utente. È presente un costo aggiuntivo per ottenere la Sandbox di aggiornamento personalizzato. Per ulteriori informazioni, consulta <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">La [!DNL Adobe Workfront] Ambiente Sandbox di aggiornamento personalizzato</a>.</td>
    </tr>
</table>

>[!TIP]
>
>È consigliabile prima installare la blueprint in un ambiente sandbox. In questo modo, puoi testare il contenuto del blueprint e accertarti che sia adatto alla tua organizzazione senza apportare modifiche ai dati live.

>[!NOTE]
>
>Alcuni blueprint sono disponibili solo per l’installazione nell’ambiente di anteprima a scopo di test. Se accedi al contenuto solo anteprima nell’ambiente di produzione, Sandbox 1 o Sandbox 2, il pulsante di installazione non è attivo e potresti visualizzare un messaggio di avviso.\
>Inoltre, la funzionalità di commutazione dell&#39;ambiente è limitata quando si accede al contenuto di sola anteprima, anche quando si è nell&#39;ambiente di anteprima.

## Installare la blueprint

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Blueprint]**.
1. Trova il modello da installare. È possibile filtrare per caso d’uso, livello di scadenza, stato dell’installazione e digitare sul lato destro.
1. (Facoltativo) Fai clic su **[!UICONTROL Dettagli]** per imparare come funziona il modello.
1. Fai clic su **[!UICONTROL Installa]**.
1. Scegli di eseguire l’installazione nell’ambiente di produzione o in un ambiente sandbox.\
   Per ulteriori informazioni, consulta la sezione [Dove devo installare un modello?](#where-should-i-install-a-blueprint) in questo articolo.
1. Sulla [!UICONTROL Configura] è possibile scegliere di effettuare una delle seguenti operazioni:

   * Installa la blueprint così com&#39;è. Per i tipi di blueprint che non richiedono alcuna configurazione, questa è l’unica opzione. Per i tipi di blueprint che necessitano di configurazione, è possibile scegliere di installare la blueprint ora e configurarla in un secondo momento. Fai clic su **[!UICONTROL Installa così come è]**.
   * Configura la blueprint prima dell’installazione, per i progetti che richiedono la configurazione. Effettua le selezioni di configurazione e fai clic su **[!UICONTROL Installa blueprint]**.\

      Per ulteriori informazioni, consulta [Configurare una blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
Al termine dell’installazione, viene visualizzato un elenco degli oggetti specifici (ad esempio ruoli, team o gruppi) che sono stati installati correttamente con la blueprint ed eventuali oggetti che non sono stati installati.

Dopo l’installazione del modello, potrebbero essere necessarie alcune azioni aggiuntive per distribuirlo completamente. Per informazioni, consulta [Azioni da intraprendere dopo l’installazione di una blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
