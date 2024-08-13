---
title: Assegnare utenti a un modello di layout
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: In qualità di amministratore di Adobe Workfront, puoi assegnare un modello di layout creato a qualsiasi utente, mansione, team o gruppo che deve utilizzarlo.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Assegnare utenti a un modello di layout

È possibile assegnare un modello di layout creato a qualsiasi utente, mansione, team o gruppo che deve utilizzarlo.

Per gli utenti a cui non è assegnato un modello di layout, viene utilizzato il layout predefinito. Per informazioni sul layout predefinito, vedere [Informazioni sul layout predefinito di Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Gli utenti possono anche assegnare a se stessi un modello di layout, come descritto in Modificare le aree Il mio lavoro e Richieste di lavoro con modelli di layout.

È possibile assegnare più modelli layout diversi allo stesso nome. Per ulteriori informazioni sul modello di layout attivo per un utente, un ruolo, un gruppo o un team, vedere [Priorità assegnazione modello di layout](#layout-template-assignment-priority) più avanti in questo articolo.

Per ulteriori informazioni sui modelli layout, vedere [Modelli layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Per informazioni sui modelli di layout per i gruppi, vedere [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirli per un gruppo, è necessario essere un manager di tale gruppo.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Assegnare un modello di layout agli utenti

1. Iniziare a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Se si è soddisfatti del modello di layout, si consiglia di verificarlo, come descritto in [Verifica di un nuovo modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Fai clic su **Assegna a** nella sezione superiore della pagina.
1. Nella casella visualizzata, fare clic su **Aggiungi utente, mansione, team o gruppo**, iniziare a digitare il nome di un utente, una mansione, un team o un gruppo, quindi fare clic sul nome quando viene visualizzato nel menu a discesa.

   I nomi aggiunti di recente vengono visualizzati con uno sfondo blu. Questa funzione è utile quando si modifica un modello di layout esistente, in quanto è possibile distinguere i nomi appena aggiunti da quelli già presenti nell&#39;elenco.

   A destra del nome di qualsiasi utente, mansione, team o gruppo già assegnato a un altro modello di layout viene visualizzata l&#39;icona Info ![](assets/info-icon.png). Passa il puntatore del mouse sull&#39;icona per visualizzare il nome del modello di layout e decidere se ignorare l&#39;assegnazione esistente.

1. Ripeti i due passaggi precedenti per assegnare il modello di layout ad altri utenti, ruoli, team o gruppi in base alle esigenze.

   Puoi assegnare fino a 100 utenti alla volta.

1. Fai clic su **Fine**, quindi fai clic su **Salva** nell&#39;angolo in basso a sinistra.

   Questo passaggio completa il processo di creazione e assegnazione di un modello di layout.

## Priorità assegnazione modello di layout {#layout-template-assignment-priority}

L’utente e gli altri amministratori di Workfront possono assegnare più modelli di layout diversi allo stesso utente in quattro modi diversi:

* Per il singolo utente
* A una particolare mansione l’utente ha
* Per un determinato team l&#39;utente è attivo
* A un determinato gruppo l’utente si trova

Tuttavia, l&#39;utente può visualizzare un solo modello di layout alla volta. Il modello visibile è determinato dalla seguente gerarchia di priorità:

* **Utente singolo**: il modello di layout assegnato alla persona come singolo utente sostituisce tutti gli altri. È possibile sovrascrivere un&#39;assegnazione precedente assegnata a un singolo utente effettuando una nuova assegnazione; quella più recente ha la precedenza.
* **Ruolo principale**: se alla persona non viene assegnato un modello di layout come singolo utente, viene visualizzato il modello assegnato per la sua mansione principale.

  Solo il modello di layout assegnato alla mansione principale di un utente è visibile all&#39;utente. I modelli assegnati a qualsiasi mansione secondaria in possesso dell’utente non sono visibili.

* **Team predefinito**: se alla persona non viene assegnato un modello di layout come singolo utente o come utente con una mansione principale, viene visualizzato il modello assegnato al proprio team predefinito.

  Solo il modello assegnato al team principale di un utente è visibile all’utente. I modelli assegnati ad altri team a cui appartiene un utente non sono visibili.

* **Gruppo predefinito**: se alla persona non viene assegnato un modello di layout come singolo utente, utente con una mansione principale o membro di un team predefinito, verrà visualizzato il modello assegnato al proprio gruppo predefinito.

  Solo il modello assegnato al gruppo Predefinito di un utente è visibile all&#39;utente. I modelli assegnati a uno qualsiasi degli altri gruppi non sono visibili.

## Numero elevato di utenti assegnati a un modello di layout

Se si modifica un modello di layout assegnato a più di 2.000 utenti e si apportano modifiche, solo i primi 2.000 utenti verranno mantenuti nel modello e verranno visualizzate le modifiche apportate. Il modello di layout viene rimosso da tutti gli altri.

Se si dispone di più di 2.000 utenti da assegnare a un modello di layout, è consigliabile effettuare una delle seguenti operazioni:

* Organizza gli utenti in gruppi o team e assegna il modello di layout a tali gruppi o team. Per ulteriori informazioni, vedere [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Creare e gestire team](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Assegna ruoli agli utenti e assegna il modello di layout alla loro mansione principale. Per ulteriori informazioni, vedere [Creare e gestire ruoli](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
