---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Accesso singolo [!DNL Workfront Proof]: Configurazione di AD FS"'
description: Se si è un amministratore nel server AD, è possibile installare e configurare ADFS.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Accesso singolo [!DNL Workfront Proof]: Configurazione di AD FS

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Se si è un amministratore nel server AD, è possibile installare e configurare ADFS.

## Installazione e configurazione di AD FS

1. Scarica [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) al computer.
1. Aprire il file AdfsSetup.exe scaricato per avviare l&#39;Installazione guidata ADFS (Active Directory Federation Services).
1. Nella schermata Ruolo server selezionare una delle opzioni (è necessario almeno un server federativo).
1. Se non si desidera esporre IIS sul server AD a Internet (porte 80 e 443 per HTTP e HTTPS), è prima possibile impostare un server federativo dietro il firewall, quindi creare un secondo proxy del server federativo che trasmette le richieste attraverso il firewall al server federativo.
1. Una volta completata la configurazione di AD FS, selezionare **[!UICONTROL Avvia lo snap-in Gestione di AD FS 2.0]**, quindi fai clic su **[!UICONTROL Fine]**. Una volta completato, la finestra Gestione AD FS 2.0 deve essere aperta immediatamente. In caso contrario, puoi aprirlo da **[!UICONTROL Inizio]** > **[!UICONTROL Strumenti di amministrazione]** > **[!UICONTROL Gestione di AD FS 2.0]**. Questa è l&#39;applicazione di controllo ADFS principale.

1. Per iniziare, fare clic su Configurazione guidata server federativo ADFS 2.0.
Questo ti aiuterà a configurare AD FS e a connetterlo a Internet tramite IIS e ad AD.
1. Se si sta configurando un nuovo server AD FS, selezionare **[!UICONTROL Crea nuovo servizio federativo]**.
1. Seleziona **[!UICONTROL Server federativo autonomo]** (a fini di test e valutazione).

1. Per un&#39;elevata disponibilità e bilanciamento del carico, fare clic su Nuova server farm federativa.
1. Specifica il nome del servizio federativo.
Per impostazione predefinita, la procedura guidata di configurazione recupera il certificato SSL associato al sito Web predefinito in IIS e utilizzerà il nome del soggetto specificato in questo campo. Se si utilizza un certificato con caratteri jolly, è necessario immettere il nome del servizio federativo.
Se in IIS non è configurato alcun certificato SSL, la procedura guidata di configurazione eseguirà una ricerca nell’archivio certificati del computer locale per individuare eventuali certificati validi. Vengono visualizzati nel menu a discesa del certificato SSL . Se non sono stati trovati certificati, è possibile utilizzare Server Certificate Generator in IIS per crearne uno.

1. Continua con la configurazione e fai clic su **[!UICONTROL Chiudi]** una volta completato.

## Configurazione [!DNL Workfront Proof] Single Sign-On

Se sei un [!DNL Workfront Proof] amministratore, è possibile configurare Single Sign-On nel [!DNL Workfront Proof] lato. Per ulteriori informazioni, consulta [Accesso singolo [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Fai clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**, quindi apri la **[!UICONTROL Single sign-on]** scheda .

1. In **URL SSO** incolla il tuo Entity ID.
Esempio di ID entità: http://*&lt;adfs.your-company.com>*/adfs/services/trust L&#39;ID entità può essere trovato nel file XML dei metadati della federazione.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. I metadati federativi si trovano nella cartella snap-in AD FS 2.0 > Servizio > Endpoint . Nella sezione Metadati individuare quello con il tipo di metadati federativi. Per visualizzare i metadati, incolla questo endpoint nel browser. Puoi anche accedere direttamente a questo link: https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml dopo aver sostituito {adfs.your-company.com} con i tuoi dati.
1. In **[!UICONTROL URL di accesso]** incolla l&#39;accesso SSO.
1. Di seguito è riportato un esempio di accesso SSO:
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Questo collegamento può trovarsi nel file XML dei metadati federativi.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. In **[!UICONTROL URL di disconnessione]** , inserisci il collegamento e salva.
Esempio di URL di disconnessione: https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Vai al tuo AD FS manager > Relazioni di trust > Affidabilità trust party trust - Proprietà ProofHQ.
   1. In Endpoint, fai clic su [!UICONTROL Aggiungi e inserisci] con i seguenti dettagli:

      * Tipo endpoint = Logout SAML
      * Binding = POST
      * URL = https://*&lt;adfs.your-company.com span=&quot;&quot; id=&quot;1&quot; translate=&quot;no&quot; />>/adfs/ls/?wa=wsignout1.0*
      * Questo passaggio può essere completato dopo la configurazione dell&#39;attendibilità del componente (vedi di seguito) in AD FS.
   1. In **[!UICONTROL impronta digitale del certificato]** immettere i dati del certificato.
   1. Passa allo snap-in ADFS 2.0 e passa a Servizio > Certificati > Firma token.
   1. Fai clic con il pulsante destro del mouse su questa voce per visualizzare il certificato.
   1. Da [!UICONTROL Dettagli certificato] copia la miniatura e incollala nel **[!UICONTROL Single Sign-On a prova di Workfront]** scheda di configurazione.

   1. I caratteri dell’impronta digitale possono essere separati da due punti o spazi, ma si consiglia di rimuoverli. In caso di problemi con la configurazione del Single Sign-On, contatta il team di assistenza clienti.


## Aggiunta di un trust tra gruppi

Una volta completata la configurazione, è necessario lavorare nella sezione Affidati del componente in AD FS.

1. Passa a **[!UICONTROL Relazioni di trust]** > **[!UICONTROL Fiducia nel partito]** cartella, quindi fai clic su **[!UICONTROL Aggiungere un trust tra gruppi]** per avviare la configurazione guidata.

1. Seleziona l’origine dati.
Tutti i metadati [!DNL ProofHQ] l&#39;account si trova sotto un link come questo: https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq Questo configurerà la maggior parte del Relying Party Trust.

   >[!NOTE]
   >
   >* In caso di problemi durante l&#39;impostazione della connessione dall&#39;URL, salva i metadati come file e scegli di importare i dati da un file.
   >* Se hai un dominio personalizzato completo (ad esempio, www.your-proofing.com) configurato sul tuo [!DNL ProofHQ] sostituisci l&#39;intera parte &quot;{yoursubdomain}.proofhq.com&quot; con il tuo dominio per creare il tuo [!DNL ProofHQ] collegamento metadati.



## Configurazione delle regole di attestazione

Una volta completata la configurazione dell&#39;attendibilità del componente, puoi configurare le regole di attestazione per completare l&#39;impostazione. Verranno configurate due regole di attestazione per ProofHQ: E-mail e ID nome.

1. Apri **[!UICONTROL Modifica regole di attestazione]** finestra di dialogo.
1. Vai a **[!UICONTROL Trust del gruppo di relazioni con i fornitori di prova]**, quindi fai clic su **[!UICONTROL Modifica regole di attestazione]** (1)\
   Se hai selezionato questa opzione al termine della configurazione dell&#39;attendibilità, la finestra a comparsa deve aprirsi automaticamente.

1. Fai clic su **[!UICONTROL Aggiungi regola]** (2) per aprire la finestra di configurazione dell&#39;attestazione.

   * E-mail (invia attributi LDAP come modello di regola delle attestazioni)
   * NameID (Trasforma un modello di regola attestazione in arrivo)
