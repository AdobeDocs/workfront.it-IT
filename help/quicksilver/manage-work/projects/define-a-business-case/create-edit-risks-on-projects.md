---
product-area: projects
navigation-topic: business-case-and-scorecards
title: Creare e modificare i rischi relativi ai progetti
description: I rischi sono possibili eventi o fattori che impediscono il completamento di un progetto nei tempi e nel budget previsti. I rischi possono essere registrati come parte della creazione del Business Case di un progetto o utilizzando la scheda Rischi. I rischi vengono creati solo su un progetto. Non è possibile associare i rischi a attività o problemi.
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: 8611c7bf8be6405f8ec8462ff2fd0f5998e8a995
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# Creare e modificare i rischi relativi ai progetti

I rischi sono possibili eventi o fattori che impediscono il completamento di un progetto nei tempi e nel budget previsti. I rischi possono essere registrati come parte della creazione del Business Case di un progetto o utilizzando la scheda Rischi. I rischi vengono creati solo su un progetto. Non è possibile associare i rischi a attività o problemi.

I rischi possono essere associati al costo, ma il costo effettivo del rischio non influisce sul costo effettivo del progetto.

>[!NOTE]
>
>Questo articolo definisce i rischi associati al progetto quando vengono definiti nel Business Case del progetto o come aggiunti nella scheda Rischi del progetto. Per informazioni sul campo Rischio disponibile durante la modifica di un progetto, consulta [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l’accesso a progetti e dati finanziari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p> Gestisci le autorizzazioni che includono Gestione finanziaria per il progetto per il quale desideri creare o modificare i rischi </p> <p>Per ulteriori informazioni sulle autorizzazioni del progetto, consulta l’articolo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Condivisione di un progetto in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Creare e modificare i rischi nel Business Case

È possibile creare rischi nell’ambito della pianificazione del Business Case di un progetto. In seguito è possibile modificarli nel Business Case, quando si verificano cambiamenti alla loro probabilità, al piano di mitigazione o al loro costo, ad esempio. Per informazioni sulla creazione di un Business Case, vedere [Creare un business case per un progetto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

L&#39;amministratore di Workfront o l&#39;amministratore del gruppo deve abilitare **Rischi** nella sezione Business case nell&#39;area Preferenze progetto prima di visualizzarla a livello di progetto nella sezione Business case. Per informazioni sull&#39;impostazione delle preferenze del progetto, consulta [Configurare le preferenze del progetto a livello di sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Creare e modificare i rischi nel Business Case è identico.

Per creare o modificare un rischio nel Business Case:

1. Passa al progetto per il quale desideri creare rischi.
1. Fai clic su **Business case** nel pannello a sinistra.
1. In **Rischi** sezione, fai clic su **Modifica rischi**.
1. Immetti o modifica le seguenti informazioni:

   * **Descrizione:** descrivere il rischio.

   * **Costo potenziale**: indicare il costo stimato in caso di rischio.

   * **Probabilità**: indicare la probabilità che il rischio si verifichi come valore percentuale.

   * **Tipo:** indicare la categoria in cui rientra il rischio.
   * **Piano di attenuazione**: aggiornare la descrizione del piano per attenuare il rischio.

   * **Costi di mitigazione**: indicare il costo del piano di mitigazione che è necessario mettere in atto per evitare che il rischio si verifichi.

   ![](assets/crp1-350x117.png)

1. (Facoltativo) Fai clic su **Aggiungi un altro rischio** aggiungere rischi aggiuntivi.
1. Fai clic su **Salva**.

## Creare e modificare i rischi nell&#39;area Rischi

Oltre a creare e modificare i rischi nel Business Case, è possibile utilizzare il **Rischi** di un progetto.

* [Creare rischi nell&#39;area dei rischi](#create-risks-in-the-risks-area)
* [Modificare i rischi nell&#39;area Rischi](#edit-risks-in-the-risks-area)

### Creare rischi nell&#39;area dei rischi {#create-risks-in-the-risks-area}

1. Passa al progetto per il quale desideri creare dei rischi.
1. Fai clic su **Rischi** nel pannello a sinistra.

   ![Sezione dei rischi dell&#39;attività](assets/risks-section-on-project-2022.png)

1. Fai clic su **Iniziare ad aggiungere rischi** e creare rischi modificando le informazioni in linea.

   Oppure

   Fai clic su **Nuovo rischio**. La **Nuovo rischio** viene visualizzata la finestra di dialogo.

1. Immetti le seguenti informazioni:

   * **Descrizione**: descrivere il rischio.
   * **Tipo di rischio**: indicare la categoria in cui rientra il rischio.\
      L’amministratore di Workfront definisce i tipi di rischio disponibili nell’ambiente. Per informazioni sulla definizione dei tipi di rischio, consulta l’articolo [Modificare e creare tipi di rischio](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Probabilità**: indicare la probabilità che il rischio si verifichi come valore percentuale.
   * **Costo potenziale**: indicare il costo stimato in caso di rischio.
   * **Costi di mitigazione**: indicare il costo del piano di mitigazione che è necessario mettere in atto per evitare che il rischio si verifichi.
   * **Costo effettivo**: indicare il costo effettivo del rischio se si è verificato il rischio.
   * **Piano di attenuazione**: aggiornare la descrizione del piano per attenuare il rischio.

1. (Condizionale) Fai clic su **Invio** se si sta creando il rischio in linea.

   Oppure

   Fai clic su **Salva** se stai modificando le informazioni nel **Nuovo rischio** finestra di dialogo.

1. (Facoltativo) Seleziona un diverso **Stato** per il rischio, **Stato** menu a discesa, quando si applica il **Standard** visualizzazione dell&#39;elenco dei rischi.

   Per impostazione predefinita, lo stato di un rischio è **Identificato**.

### Modificare i rischi nell&#39;area Rischi {#edit-risks-in-the-risks-area}

È possibile modificare i rischi durante la vita di un progetto, ad esempio quando si verificano cambiamenti nella probabilità, nel costo potenziale o nello stato.

È possibile modificare un rischio alla volta oppure modificare più rischi in blocco.

Per modificare i rischi:

1. Passa a un progetto per il quale desideri modificare i rischi esistenti.
1. Fai clic su **Rischi** nel pannello a sinistra.
1. Inizia la modifica in linea dei campi per i rischi visualizzati nell’elenco per modificare un rischio alla volta.

   Oppure

   Seleziona uno o più rischi, quindi fai clic su **Modifica** modificare contemporaneamente più rischi.

   >[!NOTE]
   >
   >Quando modifichi più rischi contemporaneamente, applichi le stesse informazioni a tutti i rischi selezionati. Le informazioni associate a ogni rischio prima delle modifiche vengono sovrascritte in una modifica collettiva.

1. Se hai fatto clic su **Modifica**, **Modifica rischio** viene visualizzata la finestra di dialogo.

   È consigliabile modificare i campi seguenti:

   * **Descrizione**: modificare la descrizione del rischio.
   * **Tipo di rischio**: indicare la categoria in cui rientra il rischio.
   * **Probabilità**: indicare la probabilità che il rischio si verifichi come valore percentuale.
   * **Costo potenziale**: indicare il costo stimato in caso di rischio.
   * **Costi di mitigazione**: indicare il costo del piano di mitigazione che è necessario mettere in atto per evitare che il rischio si verifichi.
   * **Costo effettivo**: indicare il costo effettivo del rischio se si è verificato il rischio.
   * **Piano di attenuazione**: aggiornare la descrizione del piano per attenuare il rischio.

1. Fai clic su **Salva modifiche**.
1. (Facoltativo) Modifica il **Stato** per un rischio, **Stato** menu a discesa, quando si applica il **Standard** visualizzazione dell&#39;elenco dei rischi.

   >[!NOTE]
   >
   >Non è possibile modificare il **Stato** dei rischi **Modifica rischio** finestra di dialogo. È possibile farlo solo in una modifica in linea.
