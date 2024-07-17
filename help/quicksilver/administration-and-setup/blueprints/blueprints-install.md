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
source-wordcount: '471'
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
   <td role="rowheader"><strong>Licenza Adobe [!DNL Workfront]</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurazioni del livello di accesso</strong></td> 
   <td> <p>[!UICONTROL Amministratore di sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dove devo installare una blueprint? {#where-should-i-install-a-blueprint}

Puoi installare il pacchetto in uno dei seguenti ambienti:

<table style="table-layout:auto">
        <tr>
        <td><strong>Production</strong></td>
        <td>La produzione è il tuo ambiente live.</td>
    </tr>
    <tr>
        <td><strong>Anteprima sandbox</strong></td>
        <td>L’anteprima sandbox è un ambiente di test che funge da replica dell’ambiente live e viene aggiornato ogni fine settimana da Workfront. Tutti i pacchetti di supporto hanno accesso all’anteprima Sandbox. Per ulteriori informazioni, vedere <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">L'ambiente Sandbox di anteprima [!DNL Adobe Workfront]</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 e 2</strong></td>
        <td>La sandbox di aggiornamento personalizzata è un ambiente di test separato che viene aggiornato manualmente dall’utente. Per ottenere la Sandbox di aggiornamento personalizzata è necessario un costo aggiuntivo. Per ulteriori informazioni, vedere <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">L'ambiente Sandbox di aggiornamento personalizzato [!DNL Adobe Workfront]</a>.</td>
    </tr>
</table>

>[!TIP]
>
>È consigliabile innanzitutto installare la blueprint in un ambiente sandbox. In questo modo, puoi testare il contenuto del blueprint e assicurarti che sia adatto alla tua organizzazione senza apportare modifiche ai dati live.

>[!NOTE]
>
>Alcuni blueprint sono disponibili per l’installazione nell’ambiente di anteprima solo a scopo di test. Se accedi a contenuti di sola anteprima nell’ambiente di produzione, Sandbox 1 o Sandbox 2, il pulsante di installazione non è attivo e potresti visualizzare un messaggio di avviso.\
>Inoltre, la funzionalità di cambio dell’ambiente è limitata quando si accede a contenuti di sola anteprima, anche quando ci si trova nell’ambiente di anteprima.

## Installare la blueprint

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **[!UICONTROL menu principale]** nell&#39;angolo superiore destro di [!DNL Adobe] Workfront, quindi fai clic su **[!UICONTROL Blueprint]**.
1. Trova il blueprint da installare. Puoi filtrare per caso d’uso, livello di maturità, stato di installazione e tipo sul lato destro.
1. (Facoltativo) Fai clic su **[!UICONTROL Dettagli]** per scoprire come funziona la blueprint.
1. Fare clic su **[!UICONTROL Installa]**.
1. Scegli di eseguire l’installazione nell’ambiente di produzione o in un ambiente sandbox.\
   Per ulteriori informazioni, vedere [Dove installare una blueprint?](#where-should-i-install-a-blueprint) sezione in questo articolo.
1. Nella pagina [!UICONTROL Configura] è possibile scegliere di eseguire una delle operazioni seguenti:

   * Installa la blueprint così come è. Per i tipi di blueprint che non richiedono alcuna configurazione, questa è l’unica opzione. Per i tipi di blueprint che richiedono la configurazione, puoi facoltativamente scegliere di installare la blueprint ora e configurarla in un secondo momento. Fare clic su **[!UICONTROL Installa come è]**.
   * Configura il blueprint prima dell’installazione, per i blueprint che richiedono la configurazione. Effettuare le selezioni di configurazione e fare clic su **[!UICONTROL Installa blueprint]**.\

     Per ulteriori informazioni, vedere [Configurare una blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
Al termine dell’installazione, un messaggio visualizza un elenco degli oggetti specifici (ad esempio ruoli, team o gruppi) installati correttamente con la blueprint e degli oggetti che non sono stati installati.

Dopo aver installato la blueprint, potrebbero essere necessarie alcune azioni aggiuntive per distribuirla completamente. Per informazioni, vedere [Azioni da eseguire dopo l&#39;installazione di una blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
