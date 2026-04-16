---
title: Concedere l’accesso alle autorizzazioni del marchio
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: In qualità di amministratore di Adobe Workfront, puoi configurare le autorizzazioni del brand creando un gruppo di utenti in Admin Console e assegnando il profilo di prodotto GenStudio system manager.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 727efbd6-79b4-42c5-bfa2-e5350f30ff23
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 7%

---

# Concedere l’accesso alle autorizzazioni del brand

Gli utenti ricevono le autorizzazioni di creazione, modifica e pubblicazione del brand dei manager di sistema di Adobe GenStudio quando vengono aggiunti a un gruppo di utenti.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza di Adobe Workfront</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni di Admin Console</td> 
   <td> <p>Devi essere un amministratore di sistema in Adobe Admin Console.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisiti

* L&#39;istanza di Workfront deve avere le approvazioni unificate abilitate.

* La tua organizzazione deve disporre di GenStudio Foundation.
   * Il Visualizzatore contenuti di Workfront fornisce le funzionalità disponibili in GenStudio Foundation per i flussi di lavoro di revisione e approvazione delle risorse. Non è necessario accedere direttamente a GenStudio Foundation per completare il lavoro. L’accesso alle funzionalità di GenStudio Foundation tramite Content Reviewer rientra nei termini del contratto Workfront.
* Adobe deve disporre di un accordo Adobe Gen AI firmato su file.
Per ulteriori informazioni sulla firma del contratto, consulta [Firmare il contratto di Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## &#x200B;1. Configurare le autorizzazioni del brand in Admin Console

### Passaggio 1: creare un gruppo di utenti

Crea un nuovo gruppo di utenti in Admin Console per gestire le autorizzazioni per la creazione e la modifica del brand.

### Passaggio 2: assegnare un profilo di prodotto al gruppo di utenti

L’adesione associata al profilo assegnato concede a tutti gli utenti di questo gruppo le autorizzazioni GenStudio Brands (creazione, aggiornamento ed eliminazione di brand).

Per assegnare un profilo:

1. Passa al gruppo di utenti appena creato.
1. Fai clic sulla scheda **Profili di prodotto assegnati**.
1. Fare clic su **Assegna profilo**.
1. Nel popup, seleziona **Adobe GenStudio** dall&#39;elenco dei prodotti, quindi fai clic su **Applica**.
1. Seleziona il profilo **Editor di Adobe GenStudio Foundation**.
1. Fai clic su **Applica**.
1. Fai clic su **Salva**.

### Passaggio 3: aggiungere utenti al gruppo di utenti

Per assegnare agli utenti le autorizzazioni per creare, modificare e pubblicare i brand, aggiungili al gruppo di utenti.

>[!NOTE]
>
>È necessario aggiungere almeno un utente prima di aggiungere il gruppo a un progetto come descritto nel passaggio 4.

Per aggiungere utenti:

1. Vai a **Admin Console** > **Utenti** > **Gruppi di utenti**.
1. Seleziona il gruppo di utenti.
1. Aggiungere gli utenti per nome utente o indirizzo e-mail.
1. Scegli una delle corrispondenze suggerite per gli utenti esistenti.

### Passaggio 4: creare un progetto Brands

Un progetto fornisce una posizione di archiviazione in cui gli utenti possono salvare le risorse del marchio.

Per creare un progetto:

1. Passa alla scheda **Archiviazione** in Admin Console.
1. Fai clic su **Progetti**.
1. Fare clic su **Crea progetto**.
1. Nel popup immettere il nome del progetto: **Marchi Adobe GenStudio**.

   >[!IMPORTANT]
   >
   >Immetti il nome del progetto esattamente come mostrato. Non aggiungere spazi in più e non modificare le maiuscole/minuscole.

1. Fai clic su **Crea**.

### Passaggio 5: invitare il gruppo di utenti al progetto

Aggiungi il gruppo di utenti al progetto Brands per consentire loro di accedere e gestire le risorse.

1. Nel popup **Invita al progetto**, aggiungi il gruppo di utenti creato.
1. Seleziona **Autorizzazioni modificabili**.
1. Fai clic su **Invita**.

### Risultato

Gli utenti del gruppo ora dispongono delle autorizzazioni per creare, modificare e pubblicare risorse per i brand in Workfront.

## &#x200B;2. Concedere l’accesso ai marchi nei livelli di accesso di Workfront

Devi completare tutti i passaggi della sezione precedente prima di concedere l’accesso ai singoli utenti ai Marchi nei livelli di accesso di Workfront.

>[!IMPORTANT]
>
>* Solo gli utenti assegnati al gruppo di utenti con il profilo di prodotto GenStudio system manager in Admin Console possono creare, modificare e pubblicare brand in Workfront, anche se altri utenti hanno accesso ai brand abilitati nelle impostazioni del livello di accesso.
>* Gli utenti aggiunti al livello di accesso con l’accesso Marchi abilitato, ma non aggiunti al gruppo di utenti in Admin Console, possono visualizzare solo i marchi.


Per concedere l’accesso ai Marchi nei livelli di accesso di Workfront:

{{step-1-to-setup}}

1. Fai clic su **Livelli di accesso** nel pannello a sinistra.
1. Individua il livello di accesso da modificare, quindi fai clic sull&#39;icona di modifica ![icona di modifica](assets/edit-icon.png) per modificarlo.

   Oppure

   Fai clic su **Nuovo livello di accesso** per creare un nuovo livello di accesso. Per ulteriori informazioni sulla creazione dei livelli di accesso, vedere [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Scorri verso il basso fino a **Imposta restrizioni aggiuntive**, quindi seleziona **Consenti agli utenti di accedere ai marchi**.
   ![consenti l&#39;accesso alle impostazioni dei brand](assets/access-for-brands.png)
1. Fai clic su **Salva**.

Dopo aver configurato i marchi, puoi creare un revisore dei contenuti per esaminare le risorse in base alle linee guida del marchio nel flusso di lavoro di revisione e approvazione. Per ulteriori informazioni, vedere [Configurare i collaboratori IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).
