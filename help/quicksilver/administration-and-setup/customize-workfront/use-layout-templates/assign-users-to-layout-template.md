---
title: Assegnare gli utenti a un modello di layout
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: In qualità di amministratore di Adobe Workfront, puoi assegnare un modello di layout creato a qualsiasi utente, ruolo, team o gruppo che debba utilizzarlo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Assegnare gli utenti a un modello di layout

È possibile assegnare un modello di layout creato a qualsiasi utente, ruolo, team o gruppo che debba utilizzarlo.

Per gli utenti a cui non è assegnato un modello di layout, viene utilizzato il layout predefinito. Per informazioni sul layout predefinito, consulta [Informazioni sul layout predefinito di Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Gli utenti possono anche assegnare un modello di layout a se stessi, come descritto in Modificare le aree Richieste di lavoro e lavoro personali con modelli di layout.

È possibile assegnare più modelli di layout diversi allo stesso nome. Per ulteriori informazioni sul modello di layout attivo per un utente, un ruolo, un gruppo o un team, vedere [Priorità di assegnazione del modello di layout](#layout-template-assignment-priority) più avanti in questo articolo.

Per ulteriori informazioni sui modelli di layout, consulta [Modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Per informazioni sui modelli di layout per gruppi, consulta [Creare e modificare i modelli di layout di un gruppo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisiti di accesso

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Per eseguire questi passaggi a livello di sistema, è necessario disporre del livello di accesso Amministratore di sistema.
Per eseguirle per un gruppo, devi essere un responsabile di quel gruppo.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Assegnare un modello di layout agli utenti

1. Inizia a lavorare su un modello di layout, come descritto in [Creare e gestire modelli di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Quando sei soddisfatto del modello di layout, ti consigliamo di testarlo, come descritto in [Verifica di un nuovo modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Fai clic su **Assegna a** nella sezione superiore della pagina.
1. Nella casella visualizzata, fai clic su **Aggiungere un utente, un ruolo, un team o un gruppo**, inizia a digitare il nome di un utente, un ruolo di lavoro, un team o un gruppo, quindi fai clic sul nome quando viene visualizzato nel menu a discesa.

   I nomi aggiunti di recente vengono visualizzati con sfondo blu. Questa funzione è utile quando si modifica un modello di layout esistente, in quanto è possibile distinguere i nomi appena aggiunti da quelli già presenti nell’elenco.

   Icona Informazioni ![](assets/info-icon.png) viene visualizzato a destra del nome di qualsiasi utente, ruolo, team o gruppo già assegnato a un altro modello di layout. Posizionare il puntatore sull&#39;icona per visualizzare il nome del modello di layout e decidere se si desidera sostituire l&#39;assegnazione esistente.

1. Ripetere i due passaggi precedenti per assegnare il modello di layout ad altri utenti, ruoli di lavoro, team o gruppi, in base alle esigenze.

   Puoi assegnare fino a 100 utenti alla volta.

1. Fai clic su **Fine**, quindi fai clic su **Salva** nell&#39;angolo in basso a sinistra.

   Questo passaggio completa il processo di creazione e assegnazione di un modello di layout.

## Priorità di assegnazione del modello di layout {#layout-template-assignment-priority}

Voi e altri amministratori di Workfront potete assegnare più modelli di layout diversi allo stesso utente in quattro modi diversi:

* Al singolo utente
* A un particolare ruolo di lavoro dell&#39;utente
* Per un certo team l&#39;utente è attivo
* Per un determinato gruppo in cui si trova l&#39;utente

Tuttavia, l’utente può visualizzare un solo modello di layout in un dato momento. Il modello visibile è determinato dalla seguente gerarchia di priorità:

* **Utente singolo**: Il modello di layout assegnato alla persona come singolo utente sostituisce tutti gli altri. È possibile sostituire un&#39;assegnazione precedente creata in modo tale da consentire a un singolo utente di eseguire una nuova assegnazione; quello più recente ha la precedenza.
* **Ruolo di lavoro principale**: Se alla persona non viene assegnato un modello di layout come singolo utente, visualizzerà il modello assegnato per il suo ruolo principale.

   Solo il modello di layout assegnato al ruolo principale di un utente è visibile all’utente. I modelli assegnati a qualsiasi ruolo di lavoro secondario detenuto dall&#39;utente non sono visibili.

* **Gruppo Home**: Se alla persona non viene assegnato un modello di layout come singolo utente o come utente con un ruolo di lavoro principale, visualizzerà il modello assegnato al proprio team principale.

   Solo il modello assegnato al team principale di un utente è visibile all’utente. I modelli assegnati ad altri team in cui un utente è membro non sono visibili.

* **Gruppo Home**: Se alla persona non viene assegnato un modello di layout come singolo utente, come utente con un ruolo principale o come membro di un team principale, visualizzerà il modello assegnato al gruppo home.

   Solo il modello assegnato al gruppo Home di un utente è visibile all’utente. I modelli assegnati a uno qualsiasi degli altri gruppi non sono visibili.

## Numero elevato di utenti assegnati a un modello di layout

Se si modifica un modello di layout assegnato a più di 2000 utenti e si apportano modifiche, verranno mantenuti solo i primi 2000 utenti nel modello di layout e verranno visualizzate le modifiche apportate. Il modello di layout viene rimosso da tutti gli altri.

Se hai più di 2000 utenti da assegnare a un modello di layout, ti consigliamo di effettuare una delle seguenti operazioni:

* Organizza gli utenti in gruppi o team e assegna il modello di layout a tali gruppi o team. Per ulteriori informazioni, consulta [Creare un gruppo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Creare e gestire i team](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Assegnare i ruoli di lavoro agli utenti e assegnare il modello di layout al loro ruolo di lavoro principale. Per ulteriori informazioni, consulta [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
