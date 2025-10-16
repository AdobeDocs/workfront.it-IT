---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti
description: Dopo aver installato  [!DNL Adobe Workfront] per Salesforce, puoi definire i trigger che creano [!DNL Workfront] progetti quando vengono soddisfatti determinati criteri in [!DNL Salesforce] Opportunità e account.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '1573'
ht-degree: 3%

---

# Crea [!DNL Adobe Workfront] progetti da [!DNL Salesforce] oggetti

>[!IMPORTANT]
>
>Per offrire integrazioni più stabili e scalabili, stiamo passando a un approccio di integrazione moderno e flessibile che utilizza l’automazione e l’integrazione di Workfront (Fusion). Come parte di questo processo di transizione, l&#39;integrazione di Workfront for Salesforce non sarà disponibile dopo il **28 febbraio 2026**.
>
>È consigliabile utilizzare l’automazione e l’integrazione di Workfront per le esigenze di integrazione della tua organizzazione con Salesforce.
>
>Per una panoramica dell&#39;automazione e dell&#39;integrazione di Workfront, vedere [Panoramica di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Per informazioni sulle funzionalità specifiche dei moduli di automazione e integrazione di Workfront per Salesforce, vedere [Moduli Salesforce](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Dopo aver installato [!DNL Adobe Workfront] per Salesforce, è possibile definire i trigger che creano [!DNL Workfront] progetti quando vengono soddisfatti determinati criteri in [!DNL Salesforce] [!UICONTROL Opportunità] e [!UICONTROL Account].

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Piano</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti

Per inviare una richiesta [!DNL Workfront] da un [!DNL Salesforce] [!UICONTROL opportunità] o account
assicurati di disporre dei seguenti elementi nell’ambiente:

* L&#39;amministratore di [!DNL Workfront] ha installato [!DNL Workfront for Salesforce].\
   Per ulteriori informazioni sull&#39;installazione di [!DNL Workfront for Salesforce], vedere [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* L&#39;amministratore di [!DNL Workfront] ha aggiunto la sezione [!DNL Workfront] alla [!UICONTROL opportunità] e all&#39;account
layout di pagina.\
   Per ulteriori informazioni sull&#39;aggiunta della sezione [!DNL Workfront] a un layout di pagina, vedere [Configurare la sezione  [!DNL Adobe Workfront] per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Hai un account [!DNL Workfront] e puoi accedervi dalla sezione [!DNL Workfront] all&#39;interno della tua [!UICONTROL opportunità] o account
.

## Configurazione della creazione di [!DNL Workfront] progetti da [!DNL Salesforce]

* [Informazioni sulla creazione automatica dei progetti](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Configurazione di Triggers](#configuring-triggers-configuring-triggers)
* [Informazioni sui nomi dei progetti](#understanding-project-names-understanding-project-names)

### Informazioni sulla creazione automatica dei progetti {#understanding-the-automatic-creation-of-projects}

In qualità di amministratore di sistema [!DNL Salesforce], puoi definire trigger che possono creare automaticamente progetti in [!DNL Workfront] quando si verificano le seguenti situazioni in [!DNL Salesforce]:

* Aggiornamento della [!UICONTROL fase] di un&#39;opportunità [!UICONTROL opportunità] completato.
* Il [!UICONTROL Tipo] di un account
viene aggiornato.

È possibile configurare Triggers solo dopo aver installato [!DNL Workfront for Salesforce].  \
Per informazioni sull&#39;installazione di [!DNL Workfront for Salesforce], vedere [Installa [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Quando si configurano i trigger per creare automaticamente [!DNL Workfront] progetti quando vengono creati o aggiornati [!DNL Salesforce] elementi, tenere presente quanto segue:

* Per configurare i trigger è necessario essere un [!DNL Salesforce] e un amministratore di sistema [!DNL Workfront].
* Dopo aver configurato i trigger, chiunque aggiorni [!UICONTROL Stage] di un&#39;opportunità [!UICONTROL Opportunity] o [!UICONTROL Type] di un account
può attivare la creazione di un progetto [!DNL Workfront]. Sono inclusi [!DNL Salesforce] utenti che non hanno un account [!DNL Workfront].
* Non esiste alcun limite al numero di attivatori che è possibile avere.
* Non è possibile creare più trigger in base alle stesse condizioni. I trigger sono univoci per impostazione predefinita.
* Una volta creato, il progetto viene automaticamente collegato all’opportunità o all’account in cui è stato generato. Una volta stabilito, questo collegamento non può essere interrotto.
* È possibile collegare un&#39;opportunità o un account a più progetti in [!DNL Workfront] se una condizione attivata è stata soddisfatta più volte nel ciclo di vita dell&#39;opportunità o dell&#39;account.

  Ad esempio, se definisci più di una [!UICONTROL Fase] per un [!UICONTROL Opportunità] per attivare un progetto, viene creato un progetto per ogni fase definita raggiunta dall&#39;opportunità, per la durata di tale opportunità. Inoltre, se si aggiorna la [!UICONTROL Fase] di un&#39;opportunità [!UICONTROL Opportunità] da una fase definita a un&#39;altra e quindi la si aggiorna alla fase definita, viene creato un secondo progetto per la seconda volta che si aggiorna il campo [!UICONTROL Fase] alla stessa fase definita.

* Un progetto in [!DNL Workfront] può essere collegato a una sola opportunità o a un account in [!DNL Salesforce] alla volta, ma non a entrambi contemporaneamente.

### Configurazione di Triggers {#configuring-triggers}

Dopo aver configurato i trigger, il processo di creazione di [!DNL Workfront] progetti è abilitato per entrambi i framework [!UICONTROL Salesforce Classic] o [!DNL Lightning Experience].

Per configurare i trigger in [!UICONTROL Salesforce]:

1. Accedere a [!DNL Salesforce] come amministratore di sistema.
1. (Condizionale) In [!DNL Salesforce Classic], fare clic su **[!UICONTROL Configurazione]** e nella sezione **[!UICONTROL Build]** espandere **[!UICONTROL Fulmine]**.

   Oppure

   In [!DNL Salesforce] esperienza di fulmine, fai clic sull&#39;icona **[!UICONTROL Configurazione]**, quindi su **[!UICONTROL Configurazione]** e in **[!UICONTROL STRUMENTI PIATTAFORMA]** espandi **[!UICONTROL App]**.

1. Fare clic su **[!UICONTROL Pacchetti installati]**.

   Il pacchetto **[!DNL Workfront]** è stato installato.

1. Fai clic su **[!UICONTROL Configura]** accanto a **[!DNL Workfront]**.

1. Accedere a [!DNL Workfront] come amministratore di sistema.

   Viene visualizzata la pagina **[!UICONTROL Triggers]**.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Fai clic su **[!UICONTROL Nuovo trigger]**.
1. Dal menu a discesa **[!UICONTROL [!DNL Salesforce]Oggetto]**, selezionare **[!UICONTROL Opportunità]**.

   Questo è un campo obbligatorio.

1. (Condizionale) Specifica quanto segue:

   1. Dal menu a discesa **[!UICONTROL Stage]**, selezionare un **[!UICONTROL Stage]**.\

      Quando un&#39;opportunità raggiunge la [!UICONTROL Fase] specificata qui, viene creato un progetto in [!DNL Workfront]. Questo è un campo obbligatorio.

   1. Nel campo **[!UICONTROL Portfolio o Programma]**, inizia a digitare il nome di un Portfolio o di un programma in cui vuoi inserire il progetto in [!DNL Workfront], quindi selezionalo quando viene visualizzato nell&#39;elenco.\

      Se non si specifica un Portfolio o un Programma, il nuovo progetto verrà creato e aggiunto all&#39;elenco [!UICONTROL Progetti di cui sono Proprietario] dell&#39;utente connesso a [!DNL Workfront] durante la configurazione dei trigger. Tale utente è anche il proprietario del nuovo progetto.

   1. Iniziare a digitare il nome di un modello che si desidera associare al nuovo progetto [!DNL Workfront], quindi selezionarlo quando viene visualizzato nell&#39;elenco.\

      Questo è un campo obbligatorio.


      >[!NOTE]
      >
      >Se hai specificato un Proprietario del modello da utilizzare per questa integrazione, diventa il Proprietario del nuovo progetto. I nuovi progetti vengono visualizzati nell&#39;elenco [!UICONTROL Progetti di mia proprietà] dell&#39;utente proprietario del nuovo progetto, in base al modello.

   1. (Facoltativo) Seleziona **[!UICONTROL Crea un nuovo progetto per ogni tipo di prodotto venduto] campo**, se desideri creare un nuovo progetto per ogni tipo di prodotto venduto in una sola opportunità.
   1. (Condizionale) Seleziona un **[!UICONTROL prodotto]** nel menu a discesa **[!UICONTROL prodotto]**.

      Questo è un campo obbligatorio.

   1. (Condizionale) Iniziare a digitare il nome di un **[!UICONTROL Modello]** che si desidera associare al nuovo progetto [!DNL Workfront] se il prodotto specificato si trova nell&#39;opportunità [!UICONTROL 4&rbrace;. &#x200B;] Selezionala quando viene visualizzata nell’elenco.

      Questo è un campo obbligatorio.

      Il progetto creato quando un nuovo prodotto viene aggiunto all&#39;opportunità [!DNL Salesforce] viene inserito nello stesso Portfolio o nello stesso programma selezionato per l&#39;opportunità.

      >[!IMPORTANT]
      >
      >Il progetto viene creato solo quando lo stage viene aggiornato nell&#39;[!UICONTROL opportunità]. Viene creato un progetto univoco per ogni prodotto specificato al momento dell&#39;aggiornamento del campo Stage e non quando i prodotti vengono aggiunti alle [!UICONTROL opportunità].

1. (Facoltativo) Fai clic su **[!UICONTROL Nuovo trigger]**.
1. (Facoltativo) Dal menu a discesa Oggetto **[!UICONTROL [!DNL Salesforce]]**, selezionare **Account
**.

   Questo è un campo obbligatorio.
1. (Condizionale) Specifica quanto segue:

   1. Selezionare un tipo **[!UICONTROL Type]** dal menu a discesa **[!UICONTROL Type]**.

      Quando un **account
**&#x200B; designato come &#x200B;** [!UICONTROL Tipo] **&#x200B; qui specificato in [!DNL Salesforce], viene creato un &#x200B;** [!UICONTROL Progetto]** in [!DNL Workfront].

      Questo è un campo obbligatorio.

   1. (Facoltativo) Inizia a digitare il nome di un **[!UICONTROL Portfolio]** o di un **[!UICONTROL Programma]** in cui desideri inserire il progetto in [!DNL Workfront] nel campo **[!UICONTROL Portfolio o Programma]**, quindi selezionalo quando viene visualizzato nell&#39;elenco.

      Se non si specifica un Portfolio o un Programma, il nuovo progetto verrà creato e aggiunto all&#39;elenco **[!UICONTROL Progetti di cui sono Proprietario]** dell&#39;utente connesso a [!DNL Workfront] da [!DNL Salesforce]. L’utente è anche il proprietario del nuovo progetto.

   1. Inizia a digitare il nome di un **[!UICONTROL Modello]** che desideri associare al nuovo progetto [!DNL Workfront], quindi selezionalo quando viene visualizzato nell&#39;elenco.

      Questo è un campo obbligatorio.

      >[!NOTE]
      >
      >Se hai specificato un Proprietario del modello da utilizzare per questa integrazione, diventa il Proprietario del nuovo progetto. I nuovi progetti vengono visualizzati nell&#39;elenco **[!UICONTROL Progetti di mia proprietà]** dell&#39;utente proprietario del nuovo progetto, in base al modello.

   ![salesforce_triggers_page_with_cleaned_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Fai clic su **[!UICONTROL Salva]**.

   [!DNL Workfront] progetti vengono ora generati ogni volta che viene soddisfatto uno qualsiasi dei trigger.

### Informazioni sui nomi dei progetti {#understanding-project-names}

A seconda del trigger che ha generato i progetti, i nomi dei progetti in [!DNL Workfront] possono seguire uno dei seguenti modelli:

* Se il progetto viene creato in base a un&#39;opportunità o a un attivatore di account, il nome del progetto è: *`<Salesforce object name>`: `<Project template name>` (tramite [!DNL Salesforce])*.
* Se il progetto viene creato in base a un trigger di opportunità che include anche l&#39;aggiunta di un nuovo prodotto, il nome del progetto è: *`<Salesforce object name>`: `<Salesforce product name>` (tramite [!DNL Salesforce])*.

## Visualizza [!DNL Workfront] progetti

Se l&#39;amministratore di [!DNL Workfront] ha aggiunto la sezione [!DNL Workfront] all&#39;opportunità [!UICONTROL o all&#39;account &#x200B;]
layout di pagina, puoi visualizzare i progetti creati automaticamente nella scheda [!UICONTROL Progetti] di questa sezione.\
Per ulteriori informazioni sull&#39;aggiunta della sezione [!DNL Workfront] al layout di pagina di un&#39;opportunità [!UICONTROL o di un account]
, vedi [Configurare la [!DNL Adobe Workfront] sezione per [!DNL Salesforce] utenti](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

Devi disporre di un account [!DNL Workfront] e aver effettuato l&#39;accesso a [!DNL Workfront] per visualizzare la scheda [!UICONTROL Progetti].

Per visualizzare i progetti creati da un [!UICONTROL opportunità] o account
:

1. Vai a un [!UICONTROL opportunità] o account
.
1. Passare alla sezione **[!DNL Workfront]**.

   >[!NOTE]
   >
   >A seconda del modo in cui l&#39;amministratore di [!DNL Workfront] ha configurato questa sezione, potrebbe avere un nome diverso.

1. Selezionare la scheda **[!UICONTROL Progetti]**.

   Tutti i progetti creati da attivatori definiti sono elencati in questa scheda. Qualsiasi utente in [!DNL Salesforce] che dispone anche di un account [!DNL Workfront] e che potrebbe disporre delle autorizzazioni per visualizzare questi progetti in [!DNL Workfront] può visualizzarli anche in [!DNL Salesforce] per l&#39;opportunità o l&#39;account
che li ha generati.&rbrack;

   Puoi visualizzare le seguenti informazioni sui progetti creati dall’integrazione:

   * Nome progetto
   * Numero di riferimento
   * Data inserimento
   * Nome del proprietario
   * Stato
   * Condizione
   * Data di completamento Pianificata
   * Percentuale completato

     Quando queste informazioni vengono aggiornate in [!DNL Workfront], è possibile visualizzare i campi aggiornati in questo elenco.

1. (Facoltativo) Fai clic sul nome di un progetto per aprirlo in Workfront.
1. (Facoltativo) Fai clic su [!UICONTROL **[!UICONTROL Vai a Salesforce]**] nell&#39;area [!UICONTROL Dettagli progetto] o sull&#39;intestazione del progetto per accedere all&#39;[!UICONTROL opportunità] o all&#39;account
luogo di origine del progetto. L&#39;amministratore del sistema o del gruppo deve aggiungere il campo [!UICONTROL Integrazioni] al modello di layout per individuarlo nell&#39;intestazione del progetto.

   >[!NOTE]
   >
   >Il collegamento [!UICONTROL Vai a Salesforce] è visibile a tutti gli utenti [!DNL Workfront] che possono visualizzare il progetto. Per accedere all&#39;opportunità [!DNL Salesforce] o all&#39;account da cui è stato generato il progetto, è necessario disporre di un account [!DNL Salesforce].
