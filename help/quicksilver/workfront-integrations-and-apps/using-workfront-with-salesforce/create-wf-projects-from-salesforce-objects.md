---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti
description: Dopo l'installazione [!DNL Adobe Workfront] per Salesforce, puoi definire i trigger che creano [!DNL Workfront] progetti quando sono soddisfatti determinati criteri [!DNL Salesforce] Opportunità e account.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '1507'
ht-degree: 3%

---

# Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti

Dopo l&#39;installazione [!DNL Adobe Workfront] per Salesforce, puoi definire i trigger che creano [!DNL Workfront] progetti quando sono soddisfatti determinati criteri [!DNL Salesforce] [!UICONTROL Opportunità] e [!UICONTROL Account].

## Requisiti di accesso

Per utilizzare la funzionalità descritta in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td> <p>[!UICONTROL Pro] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## Prerequisiti

Per inviare un [!DNL Workfront] richiesta di [!DNL Salesforce] [!UICONTROL Opportunità] oppure l&#39;account di assicurarti di avere quanto segue nel tuo ambiente:

* Le [!DNL Workfront] amministratore installato [!DNL Workfront for Salesforce].\
   Per ulteriori informazioni sull’installazione [!DNL Workfront for Salesforce], vedi [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Le [!DNL Workfront] l&#39;amministratore ha aggiunto [!DNL Workfront] alla sezione [!UICONTROL Opportunità] e Layout delle pagine dell&#39;account.\
   Per ulteriori informazioni sull’aggiunta di [!DNL Workfront] al layout di una pagina, vedi [Configura le [!DNL Adobe Workfront] sezione per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Hai un [!DNL Workfront] e puoi accedere a da [!DNL Workfront] all&#39;interno della sezione [!UICONTROL Opportunità] o Account .

## Configurazione della creazione di [!DNL Workfront] Progetti da [!DNL Salesforce]

* [Informazioni sulla creazione automatica di progetti](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Configurazione di Triggers](#configuring-triggers-configuring-triggers)
* [Informazioni sui nomi dei progetti](#understanding-project-names-understanding-project-names)

### Informazioni sulla creazione automatica di progetti {#understanding-the-automatic-creation-of-projects}

Come [!DNL Salesforce] amministratore di sistema, puoi definire i trigger che possono creare automaticamente i progetti in [!DNL Workfront] quando accade quanto segue in [!DNL Salesforce]:

* La [!UICONTROL Stage] di [!UICONTROL Opportunità] è aggiornato.
* La [!UICONTROL Tipo] di un account viene aggiornato.

Triggers può essere configurato solo dopo l&#39;installazione [!DNL Workfront for Salesforce].  \
Per informazioni sull’installazione [!DNL Workfront for Salesforce], vedi [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Quando configuri i trigger per la creazione automatica, considera quanto segue [!DNL Workfront] quando [!DNL Salesforce] gli elementi vengono creati o aggiornati:

* Devi essere un [!DNL Salesforce] e [!DNL Workfront] amministratore di sistema per configurare i trigger.
* Dopo aver configurato i trigger, chiunque aggiorni i [!UICONTROL Stage] di [!UICONTROL Opportunità] o [!UICONTROL Tipo] di un account può attivare la creazione di un [!DNL Workfront] progetto. Ciò include [!DNL Salesforce] utenti che non hanno un [!DNL Workfront] conto.
* Non esiste alcun limite al numero di attivatori disponibili.
* Non è possibile creare più attivatori in base alle stesse condizioni. I trigger sono univoci per impostazione predefinita.
* Una volta creato, il progetto viene automaticamente collegato all’opportunità o all’account in cui è stato generato. Una volta stabilito, questo collegamento non può essere interrotto.
* Un’opportunità o un account può essere collegato a più progetti in [!DNL Workfront] quando una condizione attivata è stata soddisfatta più volte nella vita dell&#39;opportunità o dell&#39;account.

   Ad esempio, se definisci più di un [!UICONTROL Stage] per [!UICONTROL Opportunità] per attivare un progetto, viene creato un progetto per ogni fase definita raggiunta dall’opportunità, per la durata di tale opportunità. Inoltre, se aggiorni il [!UICONTROL Stage] di [!UICONTROL Opportunità] da un passaggio definito a un altro e quindi aggiornarlo nuovamente allo stadio definito, viene creato un secondo progetto per la seconda volta che si aggiorna il [!UICONTROL Stage] allo stesso stadio definito.

* Un progetto in [!DNL Workfront] può essere collegato solo a un&#39;opportunità o a un account in [!DNL Salesforce] in qualsiasi momento, ma non a entrambi allo stesso tempo.

### Configurazione di Triggers {#configuring-triggers}

Una volta configurati i trigger, il processo di creazione [!DNL Workfront] i progetti sono abilitati per entrambi [!UICONTROL Salesforce Classic] o [!DNL Lightning Experience] framework.

Per configurare i trigger in [!UICONTROL Salesforce]:

1. Accedi a [!DNL Salesforce] come amministratore di sistema.
1. (Condizionale) Ingresso [!DNL Salesforce Classic], fai clic su **[!UICONTROL Configurazione]** e sotto **[!UICONTROL Crea]** sezione, espandi **[!UICONTROL Bullone]**.

   Oppure

   In [!DNL Salesforce] Esperienza fulmine, fai clic sul pulsante **[!UICONTROL Configurazione] icona**, quindi **[!UICONTROL Configurazione]** e **[!UICONTROL STRUMENTI DI PIATTAFORMA]** espandi **[!UICONTROL App]**.

1. Fai clic su **[!UICONTROL Pacchetti installati]**.

   Tieni presente che **[!DNL Workfront]** il pacchetto è stato installato.

1. Fai clic su **[!UICONTROL Configura]** accanto a **[!DNL Workfront]**.

1. Accedi a [!DNL Workfront] come amministratore di sistema.

   La **[!UICONTROL Triggers]** viene visualizzata la pagina .

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Fai clic su **[!UICONTROL Nuovo trigger]**.
1. Da **[!UICONTROL [!DNL Salesforce]Oggetto]** menu a discesa, seleziona **[!UICONTROL Opportunità]**.

   Questo è un campo obbligatorio.

1. (Condizionale) Specifica quanto segue:

   1. Da **[!UICONTROL Stage]** menu a discesa, seleziona un **[!UICONTROL Stage]**.\

      Quando un’opportunità raggiunge il [!UICONTROL Stage] qui specificato, viene creato un progetto in [!DNL Workfront]. Questo è un campo obbligatorio.

   1. In **[!UICONTROL Portfolio o programma]** inizia a digitare il nome di un Portfolio o di un programma in cui desideri inserire il progetto [!DNL Workfront], quindi selezionalo quando viene visualizzato nell&#39;elenco.\

      Se non si specifica un Portfolio o un programma, il nuovo progetto viene creato e aggiunto al [!UICONTROL Progetti di proprietà] elenco dell’utente che ha effettuato l’accesso a [!DNL Workfront] durante la configurazione dei trigger. L’utente è anche il proprietario del progetto per il nuovo progetto.

   1. Inizia a digitare il nome di un modello da associare al nuovo [!DNL Workfront] quindi selezionalo quando viene visualizzato nell&#39;elenco.\

      Questo è un campo obbligatorio.


      >[!NOTE]
      >
      >Se nel modello che si intende utilizzare per questa integrazione è stato specificato un proprietario del modello, questo diventerà il proprietario del progetto del nuovo progetto. I nuovi progetti compaiono nel [!UICONTROL Progetti di proprietà] elenco dell’utente proprietario del nuovo progetto, in base al modello.

   1. (Facoltativo) Seleziona la **[!UICONTROL Crea un nuovo progetto per ogni tipo di prodotto venduto] field**, se desideri creare un nuovo progetto per ogni tipo di prodotto venduto con una sola opportunità.
   1. (Condizionale) Seleziona un **[!UICONTROL Prodotto]** in **[!UICONTROL Prodotto]** menu a discesa.

      Questo è un campo obbligatorio.

   1. (Condizionale) Inizia a digitare il nome di un **[!UICONTROL Modello]** che si desidera associare al nuovo [!DNL Workfront] se il prodotto specificato si trova nel [!UICONTROL Opportunità]. Selezionalo quando viene visualizzato nell’elenco.

      Questo è un campo obbligatorio.

      Il progetto creato quando viene aggiunto un nuovo prodotto al [!DNL Salesforce] l’opportunità viene collocata nello stesso Portfolio o programma selezionato per l’opportunità.

      >[!IMPORTANT]
      >
      >Il progetto viene creato solo quando lo stage viene aggiornato nel [!UICONTROL Opportunità]. Viene creato un progetto univoco per ogni prodotto specificato al momento dell’aggiornamento del campo Stage e non quando i prodotti vengono aggiunti a [!UICONTROL Opportunità].

1. (Facoltativo) Fai clic su **[!UICONTROL Nuovo trigger]**.
1. (Facoltativo) Dal **[!UICONTROL [!DNL Salesforce]Oggetto]** menu a discesa, seleziona **Account **.

   Questo è un campo obbligatorio.
1. (Condizionale) Specifica quanto segue:

   1. Seleziona una **[!UICONTROL Tipo]** dal **[!UICONTROL Tipo]** menu a discesa.

      Quando un **Account ** è designato come **[!UICONTROL Tipo]** qui [!DNL Salesforce], **[!UICONTROL Progetto]** viene creato in [!DNL Workfront].

      Questo è un campo obbligatorio.

   1. (Facoltativo) Inizia a digitare il nome di un **[!UICONTROL Portfolio]** o **[!UICONTROL Programma]** in cui desideri inserire il progetto [!DNL Workfront] in **[!UICONTROL Portfolio o programma]** , quindi selezionalo quando viene visualizzato nell’elenco.

      Se non si specifica un Portfolio o un programma, il nuovo progetto viene creato e aggiunto al **[!UICONTROL Progetti di proprietà]** elenco dell’utente che ha effettuato l’accesso a [!DNL Workfront] da [!DNL Salesforce]. L’utente è anche il proprietario del progetto per il nuovo progetto.

   1. Inizia a digitare il nome di un **[!UICONTROL Modello]** che si desidera associare al nuovo [!DNL Workfront] , quindi selezionalo quando viene visualizzato nell’elenco.

      Questo è un campo obbligatorio.

      >[!NOTE]
      >
      >Se nel modello che si intende utilizzare per questa integrazione è stato specificato un proprietario del modello, questo diventerà il proprietario del progetto del nuovo progetto. I nuovi progetti compaiono nel **[!UICONTROL Progetti di proprietà]** elenco dell’utente proprietario del nuovo progetto, in base al modello.
   ![salesforce_triggers_page_with_clean_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Fai clic su **[!UICONTROL Salva]**.

   [!DNL Workfront] ora vengono generati ogni volta che viene soddisfatto uno dei trigger.

### Informazioni sui nomi dei progetti {#understanding-project-names}

A seconda dell’attivatore che ha generato i progetti, i nomi dei progetti in [!DNL Workfront] potrebbe seguire uno dei seguenti pattern:

* Se il progetto viene creato in base a un&#39;opportunità o a un trigger di account, il nome del progetto è: *`<Salesforce object name>`: `<Project template name>` (tramite [!DNL Salesforce])*.
* Se il progetto viene creato in base a un trigger di opportunità che include anche l’aggiunta di un nuovo prodotto, il nome del progetto è: *`<Salesforce object name>`: `<Salesforce product name>` (tramite [!DNL Salesforce])*.

## Visualizza [!DNL Workfront] progetti

Se [!DNL Workfront] l&#39;amministratore ha aggiunto [!DNL Workfront] alla sezione [!UICONTROL Opportunità] Per il layout della pagina Account , puoi vedere i progetti creati automaticamente nel [!UICONTROL Progetti] scheda di questa sezione.\
Per ulteriori informazioni sull’aggiunta di [!DNL Workfront] al layout di pagina di un [!UICONTROL Opportunità] o Account , consulta [Configura le [!DNL Adobe Workfront] sezione per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Devi avere un [!DNL Workfront] e aver effettuato l&#39;accesso a [!DNL Workfront] per visualizzare [!UICONTROL Progetti] scheda .

Per visualizzare i progetti creati da un [!UICONTROL Opportunità] o Account :

1. Vai a un [!UICONTROL Opportunità] o Account .
1. Vai a **[!DNL Workfront]** sezione .

   >[!NOTE]
   >
   >A seconda di come [!DNL Workfront] amministratore ha configurato questa sezione, potrebbe avere un nome diverso.

1. Seleziona la **[!UICONTROL Progetti]** scheda .

   Tutti i progetti creati da attivatori definiti sono elencati in questa scheda. Qualsiasi utente in [!DNL Salesforce] che ha anche [!DNL Workfront] e che potrebbero disporre delle autorizzazioni per visualizzare questi progetti in [!DNL Workfront] possono anche visualizzarle [!DNL Salesforce] per [!UICONTROL Opportunità] o l&#39;account che li ha generati.

   ![[!DNL salesforce_projects_tab_with_projects_listed].png](assets/salesforce-projects-tab-with-projects-listed-350x150.png)

   Puoi visualizzare le seguenti informazioni sui progetti creati dall’integrazione:

   * Nome progetto
   * Numero di riferimento
   * Data inserimento
   * Nome del proprietario
   * Stato
   * Condizione
   * Data di completamento Pianificata
   * Percentuale completato

      Quando queste informazioni vengono aggiornate in [!DNL Workfront], puoi visualizzare i campi aggiornati in questo elenco.

1. (Facoltativo) Fai clic sul nome di un progetto per aprirlo in Workfront.
1. (Facoltativo) Fai clic su [!UICONTROL **[!UICONTROL Vai a Salesforce]**] in [!UICONTROL Dettagli progetto] per accedere all’area o all’intestazione del progetto [!UICONTROL Opportunità] o l&#39;account di origine del progetto. L&#39;amministratore di sistema o di gruppo deve aggiungere [!UICONTROL Integrazioni] al modello di layout per trovarlo nell&#39;intestazione del progetto.

   >[!NOTE]
   >
   >La [!UICONTROL Vai a Salesforce] link è visibile a tutti [!DNL Workfront] utenti che possono visualizzare il progetto. Devi avere un [!DNL Salesforce] per poter accedere al [!DNL Salesforce] Opportunità o account da cui è stato generato il progetto.
