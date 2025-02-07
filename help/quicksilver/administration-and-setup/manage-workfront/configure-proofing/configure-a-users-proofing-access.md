---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configurare l’accesso alle bozze di un utente
description: In qualità di amministratore Adobe Workfront o amministratore Workfront Proof, puoi configurare l’accesso di un utente per creare e visualizzare bozze in Workfront e Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 0%

---

# Configurare l’accesso alle verifiche di un utente

In qualità di amministratore Adobe Workfront o amministratore Workfront Proof, puoi configurare l’accesso di un utente per creare e visualizzare bozze in Workfront e Workfront Proof.

Per informazioni sulle funzionalità di verifica disponibili per la verifica di base e integrata, vedere [Accesso alla funzionalità di verifica in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore di Workfront o di Workfront Proof. Per informazioni sugli amministratori di Workfront, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

+++

## Abilitare e disabilitare la verifica per un utente (solo piani legacy) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Se l&#39;organizzazione utilizza un piano Select o Premium Workfront legacy come amministratore di Workfront, è possibile abilitare e disabilitare la funzionalità di verifica per l&#39;utente.

Quando si abilita la verifica per un utente, Workfront abilita l’opzione per la generazione automatica delle bozze dell’utente.

Anche se è possibile abilitare un utente come utente di verifica, per passare direttamente all&#39;interfaccia di Workfront Proof dal menu principale di Workfront è necessario disporre delle autorizzazioni di amministratore. Per informazioni su come abilitare questa opzione per tutti gli utenti di verifica nel sistema Workfront, vedere [Configurare l&#39;accesso a Workfront Proof tramite il menu principale di Workfront per tutti gli utenti](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. Nel **menu principale**, seleziona **Utenti**.

1. Seleziona un utente, quindi fai clic sull&#39;icona **Modifica**.
1. Nella sezione **Accesso**, seleziona o deseleziona **L&#39;utente può generare bozze**.

## Configurare il profilo di autorizzazione di una bozza utente

Il profilo di autorizzazione selezionato viene concesso agli utenti per ogni bozza esistente all’interno dell’organizzazione.

{{step-1-to-users}}

1. Seleziona uno o più utenti, quindi fai clic su **Modifica**.

1. Nella sezione **Accesso**, fai clic su una delle seguenti opzioni di autorizzazione di Workfront Proof nel menu a discesa **Profilo autorizzazione bozza**:

   >[!NOTE]
   >
   >Se utilizzi un piano Workfront legacy, accertati che l&#39;opzione **L&#39;utente può generare bozze** sia abilitata, come spiegato in precedenza nella sezione [Abilitare e disabilitare la verifica per un utente (solo piani legacy)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisore</strong> </td> 
      <td>Gli utenti possono gestire e visualizzare tutte le bozze create sull’account della tua organizzazione. Possono anche modificare i revisori aggiunti a queste bozze. Gli utenti con questo profilo di autorizzazione non possono gestire gli utenti o modificare le impostazioni di Workfront Proof.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Gli utenti possono gestire e visualizzare le bozze create o di proprietà dell’account dell’organizzazione. Possono visualizzare le bozze di altri utenti solo quando vengono aggiunti come revisori. Si tratta di un'impostazione predefinita. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Amministratore</strong> </td> 
      <td> Gli utenti dispongono delle autorizzazioni di amministratore in Workfront Proof e possono modificare le impostazioni dell’account. Gli utenti possono gestire e visualizzare tutte le bozze create sull’account della tua organizzazione. Ciò include l’aggiunta e la rimozione di revisori, bozze e commenti.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personalizzato</strong> </td> 
      <td> <p>Disponibile solo se è stato configurato un profilo di autorizzazione personalizzato in Workfront Proof.</p> <p><b>NOTA</b>:  <p>Assicurati che il profilo di autorizzazione qui concesso non fornisca un accesso maggiore rispetto all'impostazione del Livello di accesso dell'utente in Workfront (vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>). Se fornisce un accesso più elevato, l’utente può accedere alle prove all’interno di Workfront Proof a cui non può accedere in Workfront.</p> <p>Ciò è particolarmente importante se si intende consentire a tutti gli utenti di Workfront di accedere a Workfront Proof direttamente da Workfront come descritto in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Accedere a Workfront Proof da Adobe Workfront</a>.</p> <p>Per impostazione predefinita, solo gli amministratori di Workfront hanno accesso a un collegamento diretto al sito Workfront Proof dalla barra di navigazione globale di Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Il profilo di autorizzazione selezionato viene concesso agli utenti per ogni bozza esistente all’interno dell’organizzazione.

1. Fai clic su **Salva modifiche** per completare l&#39;aggiornamento delle impostazioni utente.

   >[!NOTE]
   >
   >Quando crei o aggiorni un utente in Workfront e l’indirizzo e-mail Workfront dell’utente corrisponde a quello di un utente di Workfront Proof con licenza, il sistema abilita la verifica per l’utente in Workfront. Per ulteriori informazioni, vedere [Sincronizzazione utente tra Adobe Workfront e Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerazioni

Quando si impostano le autorizzazioni, tenere presenti le informazioni seguenti:

* Se modifichi il profilo di autorizzazione di un utente in un profilo con meno autorizzazioni, l’utente potrebbe perdere la visibilità delle bozze esistenti in Workfront. Ciò può verificarsi quando qualcuno condivide un&#39;attività con un utente in Workfront, ma non condivide la bozza allegata all&#39;attività (vedi [Condividi una bozza in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Condividi una bozza in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* È possibile impostare le autorizzazioni Workfront Proof da Workfront solo se l&#39;ambiente Workfront è integrato con un account Workfront Proof Premium. Se non è possibile utilizzare gli strumenti di correzione come descritto in questa sezione, contattare l&#39;amministratore di Workfront.
* Almeno un utente nell’ambiente Workfront deve disporre delle autorizzazioni di amministratore per le verifiche. Se si tenta di rimuovere le autorizzazioni di amministratore per la verifica da tutti gli utenti, viene visualizzato un messaggio di errore.
* Quando si modifica il livello di accesso Workfront di un utente in un livello diverso da Amministratore di sistema, il profilo di autorizzazione Workfront Proof dell&#39;utente viene impostato automaticamente su Manager.

* Quando si modifica il livello di accesso di Workfront in Amministratore di sistema, il profilo Autorizzazione bozza diventa Amministratore.

## Configurare l’accesso a Workfront Proof tramite il menu principale di Workfront per tutti gli utenti {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Per impostazione predefinita, solo gli utenti con diritti amministrativi in Workfront possono accedere a Workfront Proof come descritto [Accedere a Workfront Proof da Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

È possibile concedere a tutti gli utenti l&#39;accesso al pulsante Workfront Proof nel menu principale di Workfront contattando il supporto Workfront e inviando una richiesta.

>[!IMPORTANT]
>
> Se prevedi di consentire a tutti gli utenti di Workfront di accedere a Workfront Proof direttamente dalla barra di navigazione globale di Workfront, accertati che il profilo di autorizzazione per ogni utente non fornisca un accesso maggiore del livello di accesso dell’utente in Workfront. Questo impedisce agli utenti di accedere alle prove all’interno di Workfront Proof a cui non possono accedere in Workfront. Per ulteriori informazioni, vedere [Abilitare e disabilitare la verifica per un utente (solo piani legacy)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configurare l&#39;accesso utente al Visualizzatore bozze desktop

Se gli utenti dell’organizzazione preferiscono utilizzare il Visualizzatore bozze desktop anziché il Visualizzatore bozze web per rivedere il contenuto interattivo, è possibile configurare il Visualizzatore bozze desktop in modo che venga avviato automaticamente quando gli utenti aprono le bozze dei contenuti interattivi. Per informazioni su questo visualizzatore di bozze per il desktop e sulle differenze rispetto al visualizzatore di bozze per il Web, vedere [Comprendere il visualizzatore di bozze per il desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) e [Differenze tra il visualizzatore di bozze per il Web e la panoramica del visualizzatore di bozze per il desktop](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Da Workfront, fai clic sull’icona Workfront Proof nella barra di navigazione globale per accedere a Workfront Proof.

   ![Icona bozza](assets/proof-access-proofhq-350x39.png)

1. Fai clic su **Impostazioni account** nell&#39;angolo superiore destro di Workfront Proof, quindi fai clic sulla scheda **Impostazioni**.

1. In **Proof Defaults**, alla fine della riga **Desktop Proofing Viewer for Interactive proofing**, fare clic su **Setup**.

1. Modificare le impostazioni del Visualizzatore bozze desktop, come descritto in [Visualizzatore bozze desktop](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) nell&#39;articolo [Configurare le impostazioni della bozza per l&#39;organizzazione](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Fai clic su **Salva**.

## Configurare dispositivi personalizzati per le bozze interattive

È possibile aggiungere qualsiasi dispositivo personalizzato al sistema, consentendo agli utenti di esaminare il contenuto interattivo e simulare la modalità di visualizzazione del contenuto su un dispositivo specifico quando utilizzano il Visualizzatore bozze desktop. Questa funzionalità non è disponibile nel visualizzatore bozze web, in cui gli utenti possono esaminare il contenuto interattivo, ma solo come viene visualizzato in varie risoluzioni, non su dispositivi diversi.

Per ulteriori informazioni, vedere [Modificare la risoluzione della bozza interattiva nel visualizzatore di bozze](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Da Workfront, accedere all&#39;interfaccia di Workfront Proof, come descritto in [Accedere a Workfront Proof da Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modificare le impostazioni del Visualizzatore bozze desktop, come descritto in [Configurare dispositivi personalizzati per le bozze](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) nell&#39;articolo [Configurare le impostazioni della bozza per l&#39;organizzazione](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
