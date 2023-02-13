---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configurare l’accesso per la correzione di un utente
description: In qualità di amministratore Adobe Workfront o amministratore di Workfront Proof, puoi configurare l’accesso di un utente per creare e visualizzare le bozze in Workfront e Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# Configurare l’accesso per la correzione di un utente

In qualità di amministratore Adobe Workfront o amministratore di Workfront Proof, puoi configurare l’accesso di un utente per creare e visualizzare le bozze in Workfront e Workfront Proof.

Per informazioni sulle funzionalità di correzione disponibili per le prove di base e integrate, consulta [Accesso alle funzionalità di correzione in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un amministratore di Workfront o un amministratore di Workfront Proof. Per informazioni sugli amministratori di Workfront, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Abilitare e disabilitare la correzione per un utente (solo per i piani legacy) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Se la tua organizzazione utilizza un piano legacy Select o Premium Workfront, come amministratore di Workfront, puoi abilitare e disabilitare la funzionalità di correzione per l’utente.

Quando si abilita la correzione per un utente, Workfront consente la generazione automatica delle bozze dell’utente.

Sebbene sia possibile abilitare un utente come utente di correzione, deve disporre delle autorizzazioni di amministratore per accedere direttamente all’interfaccia di prova di Workfront dal menu principale di Workfront. Per informazioni su come abilitare questa opzione per tutti gli utenti di correzione nel sistema Workfront, consulta [Configurare l’accesso a prova di Workfront tramite il menu principale di Workfront per tutti gli utenti](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. In **Menu principale**, seleziona **Utenti**.

1. Seleziona un utente, quindi fai clic sul pulsante **Modifica** icona.
1. In **Accesso** sezione , seleziona o deseleziona **L’utente può generare delle bozze**.

## Configurare il profilo di autorizzazione per la bozza di un utente

Il profilo di autorizzazione selezionato viene concesso agli utenti per ogni bozza esistente all’interno della tua organizzazione.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Utenti** ![](assets/users-icon-in-main-menu.png).
1. Seleziona uno o più utenti, quindi fai clic su **Modifica**.

1. In **Accesso** , fai clic su una delle seguenti opzioni di autorizzazione di Workfront Proof nel **Profilo di autorizzazione della bozza** menu a discesa:

   >[!NOTE]
   >
   >Se utilizzi un piano Workfront legacy, assicurati che la **L’utente può generare delle bozze** è abilitata, come spiegato in precedenza nella sezione . [Abilitare e disabilitare la correzione per un utente (solo per i piani legacy)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisore</strong> </td> 
      <td>Gli utenti possono gestire e visualizzare tutte le bozze create sull’account dell’organizzazione. Possono anche modificare i revisori aggiunti a queste bozze. Gli utenti con questo profilo di autorizzazione non possono gestire gli utenti o modificare le impostazioni di Workfront Proof.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Gli utenti possono gestire e visualizzare le bozze create o di proprietà sull’account dell’organizzazione. Possono visualizzare le bozze di altri utenti solo quando vengono aggiunte come revisore. Questa è un'impostazione predefinita. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Amministratore</strong> </td> 
      <td> Gli utenti dispongono delle autorizzazioni di amministratore in Workfront Proof e possono modificare le impostazioni dell’account. Gli utenti possono gestire e visualizzare tutte le bozze create sull’account dell’organizzazione. Ciò include l'aggiunta e la rimozione di revisori, bozze e commenti.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Customizzato</strong> </td> 
      <td> <p>Disponibile solo se hai configurato un profilo di autorizzazione personalizzato all’interno di Workfront Proof.</p> <p><b>NOTA</b>:  <p>Assicurati che il profilo di autorizzazione che concedi qui non fornisca un accesso più elevato dell'impostazione del livello di accesso dell'utente in Workfront (vedi <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>). Se fornisce un accesso più elevato, l’utente può accedere alle bozze all’interno di Workfront Proof alle quali non può accedere in Workfront.</p> <p>Questo è particolarmente importante se intendi consentire a tutti gli utenti Workfront di accedere direttamente a Workfront Proof dal Workfront come descritto in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Accedere a Workfront Proof da Adobe Workfront</a>.</p> <p>Per impostazione predefinita, solo gli amministratori di Workfront possono accedere a un collegamento diretto al sito Workfront Proof dalla barra di navigazione globale di Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Il profilo di autorizzazione selezionato viene concesso agli utenti per ogni bozza esistente all’interno della tua organizzazione.

1. Fai clic su **Salva modifiche** per completare l&#39;aggiornamento delle impostazioni utente.

   >[!NOTE]
   >
   >Quando crei o aggiorni un utente in Workfront e l&#39;indirizzo e-mail dell&#39;utente Workfront corrisponde a quello di un utente con licenza Workfront Proof, il sistema abilita la correzione per l&#39;utente in Workfront. Per ulteriori informazioni, consulta [Sincronizzazione degli utenti tra Adobe Workfront e Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerazioni

Quando imposti le autorizzazioni, considera le seguenti informazioni:

* Se modifichi il profilo delle autorizzazioni di un utente in un profilo con meno autorizzazioni, l’utente potrebbe perdere la visibilità delle bozze esistenti all’interno di Workfront. Ciò può verificarsi quando un utente condivide un&#39;attività con un utente in Workfront, ma non condivide la bozza associata all&#39;attività (vedi [Condividere una bozza in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Condividere una bozza in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Puoi impostare le autorizzazioni Workfront Proof da Workfront solo se l’ambiente Workfront è integrato con un account Workfront Proof Premium. Se non è possibile utilizzare le bozze come descritto in questa sezione, contatta l’amministratore Workfront.
* Almeno un utente nell’ambiente Workfront deve disporre delle autorizzazioni di amministratore per le prove. Viene visualizzato un messaggio di errore se si tenta di rimuovere le autorizzazioni di amministratore per la correzione da tutti gli utenti.
* Quando si modifica il livello Workfront Access di un utente a un livello diverso da System Administrator, il profilo di autorizzazione Workfront Proof dell&#39;utente viene impostato automaticamente su Manager.

* Quando si modifica il livello Workfront Access in Amministratore di sistema, il profilo Autorizzazione bozza diventa Amministratore.

## Configurare l’accesso a prova di Workfront tramite il menu principale di Workfront per tutti gli utenti {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Per impostazione predefinita, solo gli utenti con diritti amministrativi all’interno di Workfront possono accedere a Workfront Proof come descritto  [Accedere a Workfront Proof da Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

È possibile concedere a tutti gli utenti l’accesso al pulsante Workfront Proof nel menu principale di Workfront contattando il supporto Workfront e inviando una richiesta.

>[!IMPORTANT]
>
> Se prevedi di consentire a tutti gli utenti di Workfront di accedere a Workfront Proof direttamente dalla barra di navigazione globale di Workfront, assicurati che il profilo delle autorizzazioni per ogni utente non fornisca più accesso del livello di accesso dell&#39;utente all&#39;interno di Workfront. Questo impedisce agli utenti di accedere alle bozze all’interno di Workfront Proof alle quali non possono accedere in Workfront. Per ulteriori informazioni, consulta [Abilitare e disabilitare la correzione per un utente (solo per i piani legacy)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configurare l’accesso utente al visualizzatore di correzione desktop

Se gli utenti dell’organizzazione preferiscono utilizzare il visualizzatore per correzione desktop anziché il visualizzatore per correzione web per rivedere i contenuti interattivi, è possibile configurare il visualizzatore per correzione desktop affinché venga avviato automaticamente quando gli utenti aprono bozze di contenuto interattivo. Per informazioni su questo visualizzatore per correzione desktop e sulle differenze tra il visualizzatore per correzione Web, vedere [Comprendere il visualizzatore di correzione del desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) e [Panoramica sulle differenze tra il visualizzatore per correzione web e il visualizzatore per correzione desktop](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. In Workfront, fai clic sull’icona Workfront Proof nella barra di navigazione globale per accedere a Workfront Proof.

   ![](assets/proof-access-proofhq-350x39.png)

1. Fai clic su **Impostazioni account** nell&#39;angolo in alto a destra di Workfront Proof, quindi fai clic sul pulsante **Impostazioni** scheda .

1. Sotto **Valori predefiniti di prova**, alla fine del **Visualizzatore di correzione desktop per correzione interattiva** riga, fai clic su **Configurazione**.

1. Modificare le impostazioni del visualizzatore di correzione desktop, come descritto in [Visualizzatore di correzione del desktop](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) nell&#39;articolo [Configurare le impostazioni di bozza per l’organizzazione](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Fai clic su **Salva**.

## Configurare dispositivi personalizzati per le bozze interattive

È possibile aggiungere al sistema qualsiasi dispositivo personalizzato, consentendo agli utenti di rivedere il contenuto interattivo e simulare l’aspetto del contenuto su un dispositivo specifico quando utilizzano il visualizzatore di correzione desktop. (Questa funzionalità non è disponibile nel visualizzatore per correzione web, in cui gli utenti possono rivedere i contenuti interattivi, ma solo come appare in varie risoluzioni, non su vari dispositivi.)

Per ulteriori informazioni, consulta [Modificare la risoluzione della bozza interattiva nel visualizzatore di correzione](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Da Workfront, accedi all’interfaccia Workfront Proof , come descritto in [Accedere a Workfront Proof da Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modificare le impostazioni del visualizzatore di correzione desktop, come descritto in [Configurare dispositivi personalizzati per le bozze](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) nell&#39;articolo [Configurare le impostazioni di bozza per l’organizzazione](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
