---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Single Sign-On in [!DNL Workfront Proof]: configurazione ADFS'
description: Se si è un amministratore del server AD, è possibile installare e configurare ADFS.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Single Sign-On in [!DNL Workfront Proof]: configurazione ADFS

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Se si è un amministratore del server AD, è possibile installare e configurare ADFS.

## Installazione e configurazione di ADFS

1. Scaricare [ADFS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) nel computer.
1. Aprire il file AdfsSetup.exe scaricato per avviare l&#39;Installazione guidata di ADFS (Active Directory Federation Services).
1. Nella schermata Ruolo server selezionare una delle opzioni (è necessario almeno un server federativo).
1. Se non si desidera esporre IIS sul server AD a Internet (porte 80 e 443 per HTTP e HTTPS), è innanzitutto possibile impostare un server federativo dietro il firewall e quindi creare un secondo proxy server federativo che trasmetta le richieste al server federativo attraverso il firewall.
1. Dopo aver completato l&#39;installazione di ADFS, selezionare **[!UICONTROL Avvia lo snap-in Gestione ADFS 2.0]**, quindi fare clic su **[!UICONTROL Fine]**. Al termine dell&#39;operazione, viene visualizzata immediatamente la finestra Gestione ADFS 2.0. In caso contrario, è possibile aprirlo da **[!UICONTROL Start]** > **[!UICONTROL Strumenti di amministrazione]** > **[!UICONTROL Gestione AD FS 2.0]**. Questa è l&#39;applicazione di controllo principale di AD FS.

1. Per iniziare, fare clic su Configurazione guidata server federativo ADFS 2.0.
In questo modo sarà possibile configurare ADFS e collegarlo a Internet tramite IIS e AD.
1. Se si sta configurando un nuovo server AD FS, selezionare **[!UICONTROL Crea nuovo servizio federativo]**.
1. Selezionare **[!UICONTROL Server federativo autonomo]** (a scopo di test e valutazione).

1. Per ottenere un&#39;elevata disponibilità e il bilanciamento del carico, fare clic su Nuova server farm federativa.
1. Specificare il nome del servizio federativo.
Per impostazione predefinita, la configurazione guidata recupera il certificato SSL associato al sito Web predefinito in IIS e utilizzerà il nome del soggetto specificato. Se si utilizza un certificato con caratteri jolly, è necessario immettere il nome del servizio federativo.
Se in IIS non è configurato alcun certificato SSL, la configurazione guidata eseguirà una ricerca di eventuali certificati validi nell&#39;archivio certificati del computer locale. Vengono visualizzati nel menu a discesa del certificato SSL. Se non è stato trovato alcun certificato, è possibile utilizzare il Generatore di certificati del server in IIS per crearne uno.

1. Continua con la configurazione e fai clic su **[!UICONTROL Chiudi]** una volta completata.

## Configurazione di [!DNL Workfront Proof] Single Sign-On

Gli amministratori di [!DNL Workfront Proof] possono configurare il Single Sign-On sul lato [!DNL Workfront Proof]. Per ulteriori informazioni, vedere [Single Sign-On in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Fai clic su **[!UICONTROL Impostazioni]** > **[!UICONTROL Impostazioni account]**, quindi apri la scheda **[!UICONTROL Single Sign-on]**.

1. Nella casella **URL SSO**, incolla l&#39;ID entità.
Di seguito è riportato un esempio di ID entità:
http://*&lt;adfs.your-company.com>*/adfs/services/trust
L&#39;ID entità si trova nel file XML dei metadati federativi.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. I metadati federativi si trovano nello snap-in ADFS 2.0 > Servizio > Endpoint. Nella sezione Metadati individuare quello con il tipo di metadati federativi. Per visualizzare i metadati, incolla questo endpoint nel browser. Puoi anche accedere direttamente a questo collegamento: https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml dopo aver sostituito {adfs.your-company.com} con i tuoi dettagli.
1. Nella casella **[!UICONTROL URL di accesso]**, incolla l&#39;accesso SSO.
1. Di seguito è riportato un esempio di accesso SSO:
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Questo collegamento si trova nel file XML dei metadati federativi.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. Nella casella **[!UICONTROL URL disconnessione]** immettere il collegamento e salvare.
Di seguito è riportato un esempio di URL di disconnessione:
https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Passare a Gestione AD FS > Relazioni di attendibilità > Trust tra componenti - Proprietà ProofHQ.
   1. In Endpoint, fare clic su [!UICONTROL Aggiungi e immetti] con i dettagli seguenti:

      * Tipo endpoint = SAML Logout
      * Binding = POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/?wa=wsignout1.0
      * Questo passaggio può essere completato dopo la configurazione dell&#39;attendibilità del componente (vedere di seguito) in ADFS.
   1. Nella casella **[!UICONTROL Impronta digitale certificato]** immettere i dati del certificato.
   1. Andare allo snap-in ADFS 2.0 Passare a Servizio > Certificati > Firma token.
   1. Fai clic con il pulsante destro del mouse su questa voce per visualizzare il certificato.
   1. Dalla scheda [!UICONTROL Dettagli certificato] copiare l&#39;identificazione personale e incollarla nella scheda di configurazione **[!UICONTROL Workfront Proof Single Sign-On]**.

   1. I caratteri delle impronte digitali possono essere separati da due punti o da spazi, ma si consiglia di rimuoverli. In caso di problemi con la configurazione Single Sign-On, contatta il team di assistenza clienti.


## Aggiunta di un trust componente

Una volta completata la configurazione, è necessario utilizzare la sezione Trust relying party in ADFS.

1. Passa alla cartella **[!UICONTROL Relazioni di trust]** > **[!UICONTROL Trust relying party]**, quindi fai clic su **[!UICONTROL Aggiungi un trust relying party]** per avviare la configurazione guidata.

1. Seleziona l’origine dati.
Tutti i metadati per l&#39;account [!DNL ProofHQ] si trovano in un collegamento simile al seguente:
https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq
In questo modo viene configurata la maggior parte dell&#39;attendibilità del componente.

   >[!NOTE]
   >
   >* In caso di problemi con la connessione dall’URL, salva i metadati come file e scegli di importare i dati da un file.
   >* Se nell&#39;account [!DNL ProofHQ] è configurato un dominio personalizzato completo (ad esempio, www.your-proofing.com), sostituire l&#39;intera parte &quot;{yoursubdomain}.probhq.com&quot; con il proprio dominio per creare il collegamento ai metadati [!DNL ProofHQ].


## Configurazione delle regole di attestazione

Una volta completata la configurazione dell&#39;attendibilità della componente, è possibile configurare le regole di attestazione per completare la configurazione. Per ProofHQ verranno configurate due regole di attestazione: E-mail e ID nome.

1. Aprire la finestra di dialogo **[!UICONTROL Modifica regole attestazione]**.
1. Vai a **[!UICONTROL Attendibilità componente ProofHQ]**, quindi fai clic su **[!UICONTROL Modifica regole attestazione]** (1).\
   Se si seleziona questa opzione al termine della configurazione del trust, il popup dovrebbe aprirsi automaticamente.

1. Fare clic su **[!UICONTROL Aggiungi regola]** (2) per aprire la finestra di configurazione attestazione.

   * E-mail (Invia attributi LDAP come modello di regole attestazioni)
   * NameID (Trasforma un modello di regole di attestazione in ingresso)
