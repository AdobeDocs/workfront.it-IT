---
title: Configura [!DNL Workfront] con [!DNL Adobe Experience Manager] connettore legacy
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Come [!DNL Adobe Workfront] amministratore, puoi integrare [!DNL Workfront] con Adobe Experience Manager (AEM) Assets e fornire alla tua organizzazione una soluzione completa per la gestione dei contenuti per la creazione, la condivisione e la manutenzione delle risorse all’interno del tuo flusso di lavoro.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '1893'
ht-degree: 0%

---

# Configura [!DNL Workfront] con [!DNL Adobe Experience Manager] connettore legacy

Come [!DNL Adobe Workfront] amministratore, puoi integrare [!DNL Workfront] con [!UICONTROL Risorse Adobe Experience Manager (AEM)] e offre alla tua organizzazione una soluzione completa per la gestione dei contenuti per la creazione, la condivisione e la manutenzione delle risorse all’interno del flusso di lavoro.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

## [!DNL Workfront for AEM Assets]

La [!DNL Workfront for AEM Assets connector] consente alla tua organizzazione di effettuare le seguenti operazioni:

* Collabora e gestisci i contenuti creativi collegando AEM risorse e cartelle a progetti, attività, problemi e richieste in [!DNL Workfront].

   Per ulteriori informazioni sulla configurazione delle integrazioni di documentazione con applicazioni di terze parti, consulta  [Configurare le integrazioni di documenti](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integra con il [!DNL AEM Digital Asset Managemen]archivio t (DAM), che consente di utilizzare [!DNL Workfront] per gestire e condividere le risorse digitali memorizzate nel DAM.

   Per ulteriori informazioni sul collegamento di documenti e cartelle di risorse, consulta   [Collegamento di documenti da applicazioni esterne](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Combinare e applicare metadati da entrambe le applicazioni a una risorsa.
* Visualizza un flusso di comunicazione completo per una risorsa. Aggiornamenti e commenti effettuati a una risorsa in [!DNL Workfront] o [!UICONTROL AEM Assets] sono sincronizzati con l&#39;altra applicazione, stabilendo una cronologia completa delle comunicazioni effettuate al bene.

   Per ulteriori informazioni su come effettuare commenti in [!DNL Workfront], vedi [Aggiungere un aggiornamento a un documento](../../documents/managing-documents/add-update-documents.md).

## Prerequisiti per l’installazione di [!DNL AEM Assets] connettore

Prima di installare [!DNL Workfront] connettore per [!UICONTROL AEM Assets], assicurati che siano soddisfatti i seguenti prerequisiti:

* [!UICONTROL AEM Assets] installato e configurato, versione 6.5 o successiva. Per informazioni sull’installazione [!UICONTROL AEM Assets], vedi [[!DNL Adobe Experience Manager] documentazione](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Condizionale) Se le regole del firewall non consentono il traffico come previsto, aggiungi l’indirizzo IP e/o il dominio del cluster al tuo inserire nell&#39;elenco Consentiti. Per ulteriori informazioni, consulta [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Installa il [!DNL Workfront for AEM Assets] pacchetto di connettori {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>Le seguenti istruzioni sono per un [!DNL Workfront with AEM Assets] connettore legacy sostituito da [[!DNL Workfront for Experience Manager] connettore avanzato](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Per ulteriori informazioni, contatta il rappresentante commerciale di riferimento.

Per installare [!DNL Workfront for AEM Assets] connettore, è necessario importare il connettore in AEM come pacchetto utilizzando [!UICONTROL Gestione pacchetti CRX].

1. Su una workstation in cui hai già installato AEM, scarica il [!DNL Workfront for AEM Assets] File di installazione del connettore.

   È possibile ottenere [!DNL Workfront for AEM Assets] connettore dal [!DNL Workfront] rappresentante.

1. Accedi a AEM utilizzando un account amministratore.
1. Fai clic su **[!UICONTROL Strumenti]** > **[!UICONTROL Distribuzione]** > **[!UICONTROL Pacchetti]**.

   La [!UICONTROL Gestione pacchetti CRX] si apre.

1. Fai clic su **[!UICONTROL Carica pacchetto].**

1. In [!UICONTROL Carica pacchetto] finestra di dialogo, cerca e seleziona [!UICONTROL Connettore Workfront] pacchetto, quindi fai clic su **[!UICONTROL OK]**.\
   Il pacchetto viene visualizzato nel [!UICONTROL Gestione pacchetti CRX].

1. Fai clic su **[!UICONTROL Installa].**

1. Sulla [!UICONTROL Pacchetto] ignora le impostazioni avanzate e fai clic su **[!UICONTROL Installa]**.
1. (Facoltativo) Per confermare che il connettore è stato installato correttamente, verificare che la seguente istruzione sia visualizzata nella [!UICONTROL Registro attività]:

   ```
   Package installed in <time>
   ```

1. Chiudi [!UICONTROL Gestione pacchetti CRX].

   Il connettore è installato ed è ora possibile configurarlo [!DNL AEM Assets] per integrare con [!DNL Workfront].

1. Continua con [Configura [!DNL AEM Assets] per integrare con [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Configura [!DNL AEM Assets] per integrare con [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

Dopo aver installato il connettore, importa il pacchetto del connettore per AEM e configurare AEM per il collegamento con i documenti in [!DNL Workfront].

Per informazioni sull&#39;installazione del connettore, vedi  [Installa il [!DNL Workfront for AEM Assets] pacchetto di connettori](#install-the-workfront-for-aem-assets-connector-package).

* [Prerequisiti](#prerequisites)
* [Integrare AEM con [!DNL Workfront]](#integrate-aem-with-workfront)
* [Configura le [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)

### Prerequisiti {#prerequisites}

Prima di iniziare, è necessario abilitare le autorizzazioni per workfront-service:

1. In AEM, vai a **[!UICONTROL Strumenti]**> **[!UICONTROL Sicurezza]**> **[!UICONTROL Autorizzazioni]**.
1. Nell’angolo in alto a sinistra, scegli **[!UICONTROL Utenti]**&#x200B; nel menu a discesa e immetti *[!UICONTROL servizio anteriore]* in **[!UICONTROL Ricerca]** Campo &#x200B;. Seleziona la [!UICONTROL servizio anteriore] utente.
1. Sul lato destro dello schermo, seleziona **[!UICONTROL Aggiungi ACE]** per creare nuove voci.
1. Nel &#x200B;**[!UICONTROL Aggiungi nuova voce]**&#x200B; finestra, seleziona l’icona della casella di controllo **[!UICONTROL Percorso]**&#x200B; campo e scegli la cartella: */conf*
1. Nel campo Privilegi immetti: *jcr:read*
1. Seleziona **[!UICONTROL Aggiungi]**&#x200B; nell&#39;angolo in alto a destra
1. (Facoltativo) Ripeti i passaggi per creare altre voci.

### Integrare AEM con [!DNL Workfront] {#integrate-aem-with-workfront}

1. Accedi ad AEM Assets come amministratore.
1. Fai clic su **[!UICONTROL Strumenti]** >**[!UICONTROL Cloud Services]**>**[!UICONTROL Configurazione dell’integrazione Workfront]** >**[!UICONTROL Global-Workfront].**&#x200B;**&#x200B;**

1. (Condizionale) Se non lo hai ancora fatto, crea un [!DNL Workfront] file di configurazione cloud.

   1. Fai clic su  **[!UICONTROL Crea]** nell&#39;angolo superiore destro del [!DNL Global-Workfront] pagina.
   1. In **[!UICONTROL URL Workfront]** specifica l’URL per la [!DNL Workfront] istanza.

      Ad esempio: [!DNL https]://`<account>`.my.workfront.com, dove `<account>` è l’account utilizzato per le integrazioni con AEM.

   1. Nel &#x200B;**[!UICONTROL Cartella di base]** , seleziona l’icona della casella di controllo, quindi nel menu a discesa seleziona il percorso in cui sono collegati i documenti [!DNL Workfront] gli oggetti sono memorizzati.
   1. Nel modale AEM visualizzato, seguire il percorso della cartella con i documenti a cui è collegato [!DNL Workfront] oggetti. Scegli la cartella e premi **[!UICONTROL Seleziona]**&#x200B; nell&#39;angolo in alto a destra.

      Puoi collegarti a qualsiasi cartella sotto la radice /content/dam/.

   1. In **[!UICONTROL Chiave API Workfront]** specifica la [!UICONTROL Workfront] Chiave API.

      Per recuperare [!DNL Workfront] Chiave API:

      1. Apri una scheda del browser e accedi al [!DNL Workfront] come account [!DNL Workfront] amministratore.
      1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

      1. Fai clic su **[!UICONTROL Sistema]** >**[!UICONTROL Informazioni cliente]**.

         Se hai già generato una chiave API, la tua [!DNL Workfront] Chiave API viene visualizzata sotto l’etichetta Chiave API dell’utente.

      1. (Condizionale) Se non hai ancora generato una chiave API, devi generarne una:

         1. In **[!UICONTROL Impostazioni chiave API]** la sezione **[!UICONTROL Dopo la creazione, le chiavi API scadono in]** è impostato su Nessuno.

            Se selezioni un periodo di scadenza, il connettore smetterà di funzionare dopo la scadenza della chiave API. Sarà quindi necessario rigenerare una chiave API e aggiornare la [!DNL Workfront] configurazione.

         1. Sotto la **[!UICONTROL Chiave API dell’utente]** etichetta, fai clic su **[!UICONTROL Genera chiave API]**.

            Una chiave API per [!DNL Workfront] genera e visualizza.
      1. Copia la chiave API negli Appunti.
      1. Apri la scheda del browser per AEM Connector e in **[!DNL Workfront API Key]** incolla la chiave API che hai copiato.
   1. (Condizionale) Fai clic sul pulsante **[!UICONTROL Avanzate]** nell’angolo in alto a sinistra del [!UICONTROL [!DNL Workfront] Configurazione dell&#39;integrazione] e, se applicabile, seleziona le seguenti opzioni:

      **[!UICONTROL Consenti esplorazione raccolta]:**&#x200B; Selezionare questa opzione se l’organizzazione consente [!DNL Workfront] utenti a cui collegare le raccolte AEM Assets [!DNL Workfront] oggetti.

      **[!UICONTROL Federated ID utente]:** Seleziona questa opzione se l’organizzazione utilizza Federated ID o Single Sign-On (SSO) al momento dell’accesso a Workfront.

      **[!UICONTROL Ignora dominio e-mail]:** Seleziona questa opzione se gli utenti AEM non utilizzano il nome di dominio nel proprio ID utente.

      **[!UICONTROL Accesso limitato]:** Selezionare questa opzione per specificare il [!DNL Workfront] Indirizzi IP da aggiungere all’inserire nell&#39;elenco Consentiti. Per ulteriori informazioni sull&#39;inserire nell&#39;elenco Consentiti, vedi [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Fai clic sul pulsante **[!UICONTROL Base]** nell’angolo in alto a sinistra della pagina Configurazione integrazione Workfront , quindi fai clic su **[!UICONTROL Connetti]**.

      >[!NOTE]
      >
      >Le modifiche possono richiedere un po&#39; di tempo. Il riavvio del bundle potrebbe accelerare il processo.



1. (Condizionale) Se hai già creato un [!DNL Workfront] file di configurazione cloud, seleziona **[!UICONTROL Globale-[!DNL Workfront]]** nell&#39;angolo in alto a sinistra, fai clic su **[!UICONTROL Proprietà]**.

1. Genera la chiave API AEM facendo clic su **[!UICONTROL Genera chiave],** quindi copia la chiave API AEM negli Appunti.

   In seguito, quando configuri la chiave API AEM sarà necessario [!UICONTROL Workfront] per integrare con [!UICONTROL AEM Assets]. Per ulteriori informazioni, consulta [Configurare Workfront per l’integrazione con le risorse AEM](#configure-workfront-to-integrate-with-aem-assets).

1. Nell’angolo in alto a destra, fai clic su **[!UICONTROL Salva]**.

   La [!UICONTROL Globale-[!DNL Workfront]] viene visualizzata la finestra .

   ![Proprietà.png](assets/properties-350x117.png)

1. (Facoltativo) Sincronizzazione della comunicazione bidirezionale tra AEM e [!DNL Workfront].

   1. Fai clic su **[!UICONTROL Globale-[!DNL Workfront]].**
   1. Nell&#39;angolo in alto a sinistra della finestra, fai clic su **[!UICONTROL Proprietà]**.

      La [!UICONTROL [!DNL Workfront] Configurazione dell&#39;integrazione] viene visualizzata la pagina .

      ![Proprietà2.png](assets/properties2-350x444.png)

   1. (Facoltativo) Per abilitare la sincronizzazione dei commenti tra [!UICONTROL AEM Assets] e [!DNL Workfront], fai clic su **[!UICONTROL Abilita sincronizzazione commenti]**.

      >[!IMPORTANT]
      >
      >È necessario attivare [!UICONTROL Sincronizzazione dei documenti] per sincronizzare le risorse.

   1. (Facoltativo) Per disattivare la sincronizzazione dei commenti, fai clic su **[!UICONTROL Disattiva sincronizzazione commenti].**

      Oppure

      Elimina [!UICONTROL CREA NOTA] iscrizione evento registrata nella tua istanza AEM.

      Per informazioni sugli abbonamenti agli eventi, vedi [API iscrizione agli eventi](../../wf-api/general/event-subs-api.md).

1. Continua con [Configura le [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer).

### Configura le [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

La [!UICONTROL AEM Externalizer] AEM trasmettere gli URL in un formato utilizzabile in [!DNL Workfront]. Se non configurato correttamente, [!DNL Workfront] non può effettuare chiamate all&#39;API AEM e gli URL che collegano AEM documenti in Workfront non funzioneranno.

1. In AEM, fai clic su **[!UICONTROL Strumenti]** > **[!UICONTROL Operazioni]** >**[!UICONTROL Console web]**.

1. Fai clic su **[!UICONTROL OSGI]**, quindi fai clic su **[!UICONTROL Configurazione]** nel menu a discesa .

1. Nell’elenco di configurazione, seleziona &#x200B;**[!UICONTROL Day CQ Link Externalizer].**

   La [!UICONTROL Esternalizzatore] viene visualizzata la pagina .

1. In **[!UICONTROL Domini]** assicurati che il dominio elencato nella sezione [!UICONTROL Autore] è il nome di dominio accessibile esternamente agli utenti AEM.

   Il nome di dominio nel [!UICONTROL autore] Il campo deve corrispondere al dominio elencato nella riga URL dell’istanza AEM.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Condizionale) Se necessario, aggiorna il dominio nel [!UICONTROL Autore] campo .
1. Fai clic su **[!UICONTROL Salva]**.

   [!UICONTROL AEM Assets] è ora configurato per collegare documenti con [!DNL Workfront]

1. Continua con [Configura [!DNL Workfront] per integrare con [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Configura [!DNL Workfront] per integrare con [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

Dopo aver installato [!UICONTROL Workfront per AEM Assets] Connettore (come descritto in [Installa il [!UICONTROL Workfront per AEM Assets] pacchetto di connettori](#install-the-workfront-for-aem-assets-connector-package)) e configura [!UICONTROL AEM Assets] (come descritto in [Configura[!UICONTROL  AEM Assets] per integrare con [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)), è necessario configurare [!DNL Workfront] per collegare documenti tra [!DNL Workfront] e [!DNL AEM Assets].

1. Accedi a [!DNL Workfront] come [!UICONTROL Workfront] amministratore.

   >[!TIP]
   >
   >[!UICONTROL Workfront] consiglia di creare un [!UICONTROL Workfront] amministratore dedicato esclusivamente all’integrazione AEM. Per ulteriori informazioni sull’assegnazione della [!UICONTROL Workfront] livello di accesso dell&#39;amministratore a un utente, vedi [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Documenti]**> **[!UICONTROL Integrazione personalizzata].**

1. Fai clic su **[!UICONTROL Aggiungi integrazione personalizzata]**.
1. In **[!UICONTROL Nome]** Specifica il nome dell’integrazione personalizzata.

   Questo è il nome visualizzato dagli utenti quando si utilizza l’integrazione in [!UICONTROL Workfront]; ad esempio, puoi immettere *&quot;[!DNL AEM Assets]&quot;* nome.

1. In **[!UICONTROL URL API di base]** Specifica l’URL dell’istanza AEM.

   L’URL API di base è costituito dall’URL per l’istanza AEM seguita dal percorso: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. In **[!UICONTROL Tipo di autenticazione]** menu a discesa, seleziona **[!UICONTROL ApiKey].**

1. Nel &#x200B;**[!UICONTROL Chiave API]** incolla la chiave API AEM che hai copiato quando hai configurato [!UICONTROL AEM Assets].
1. Fai clic su **[!UICONTROL Salva]**.
1. (Facoltativo) Assicurati che l&#39;integrazione sia contrassegnata [!UICONTROL Attivo].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] è ora configurato per lavorare con [!DNL AEM Assets].

   Per accedere alle risorse in AEM, ciascuna [!DNL Workfront] l’utente che deve utilizzare il connettore deve essere configurato come utente in AEM. Per informazioni sulla creazione di utenti, consulta  [Configurare gli utenti per l’utilizzo del connettore](#set-up-users-to-use-the-connector).

## Configurare gli utenti per l’utilizzo del connettore {#set-up-users-to-use-the-connector}

Per consentire agli utenti di accedere al connettore, devono avere un profilo utente in AEM e appartenere a un [!DNL Workfront] gruppo con livelli di accesso che includono [!UICONTROL Crea] e [!UICONTROL Elimina] autorizzazioni.

Per ulteriori informazioni [!DNL Workfront] autorizzazioni, vedi [Creare o modificare livelli di accesso personalizzati](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Imposta gli utenti in [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Imposta gli utenti in [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Accedi a [!DNL AEM Assets] come [!DNL Workfront] amministratore.
1. Fai clic su **[!UICONTROL Strumenti]** >**&#x200B;**&#x200B;**[!UICONTROL Sicurezza]** >**[!UICONTROL Utenti]**.

1. (Condizionale) Se l’utente non ha un profilo utente in AEM, crea un profilo utente AEM.

   1. Fai clic su **[!UICONTROL Crea utente].**
   1. Immetti le informazioni personali dell&#39;utente.

      ![64NewUser.png](assets/64newuser-350x524.png)

      L’unico campo obbligatorio è il campo ID. L&#39;ID AEM dell&#39;utente deve corrispondere al [!DNL Workfront] ID, che è l&#39;ID dell&#39;utente [!DNL Workfront] indirizzo e-mail.

      Se hai selezionato la [!UICONTROL Ignora dominio e-mail] quando hai configurato AEM per l’integrazione con [!DNL Workfront], quindi l&#39;ID AEM non corrisponderà al [!DNL Workfront] indirizzo e-mail.

1. (Condizionale) Se l’utente dispone di un profilo AEM, apri il profilo AEM dell’utente.

   1. Fai clic su &#x200B;**[!UICONTROL Utente].**

      La [!UICONTROL Gestione utente] viene visualizzata la pagina .

   1. Fai clic sull’utente da aggiungere, quindi fai clic su **[!UICONTROL Proprietà]**.

      Viene visualizzata la pagina delle impostazioni dell’utente.

1. Fai clic sul pulsante **[!UICONTROL Gruppi]** scheda .

   ![](assets/groupstab.png)

1. Assicurati che l&#39;utente appartenga ad almeno uno [!DNL Workfront] gruppo con livelli di accesso che includono [!UICONTROL Crea] e [!UICONTROL Elimina] autorizzazioni.

   1. Per aggiungere l&#39;utente a un gruppo esistente, inizia a digitare il nome del gruppo nel **[!UICONTROL Nome gruppo di tipi]** selezionare il gruppo quando viene visualizzato nel menu a discesa.

      Oppure

      Per selezionare un gruppo al quale l&#39;utente è membro, selezionare un gruppo nel **[!UICONTROL Gruppi di cui l&#39;utente è membro]** sezione .

1. Fai clic su **[!UICONTROL Salva].**
