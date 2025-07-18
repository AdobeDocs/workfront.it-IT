---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 'L''ambiente sandbox di aggiornamento personalizzato  [!DNL Adobe Workfront] '
description: La sandbox di aggiornamento personalizzata è un ambiente in cui puoi testare e lavorare utilizzando i dati dell’ambiente di produzione. È ideale anche per l’esecuzione di corsi di formazione e per determinare le funzionalità di configurazione.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 7549c9699a86b6f87e5562efd7e586be282c5619
workflow-type: tm+mt
source-wordcount: '1763'
ht-degree: 0%

---

# L&#39;ambiente Sandbox di aggiornamento personalizzato [!DNL Adobe Workfront]

La sandbox di aggiornamento personalizzata è un ambiente in cui puoi testare e lavorare utilizzando i dati dell’ambiente di produzione. È ideale anche per l’esecuzione di corsi di formazione e per determinare le funzionalità di configurazione.

>[!NOTE]
>
>Si tratta di un ambiente diverso da Sandbox anteprima, che è anche un ambiente di test che replica l&#39;ambiente di produzione [!DNL Workfront].
>
>* Verranno introdotte nuove funzioni nell’anteprima sandbox, prima che siano disponibili in produzione.
>* Le nuove funzioni non vengono introdotte nella Sandbox di aggiornamento personalizzata prima di diventare disponibili in produzione.
>
>  Inoltre, esiste un costo aggiuntivo per ottenere la sandbox di aggiornamento personalizzata che non è necessaria per la sandbox di anteprima.
>
>  Per ulteriori informazioni sulla Sandbox di anteprima, vedi [L&#39;ambiente Sandbox di anteprima [!DNL Adobe Workfront] ](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] piano</td> 
   <td> <p>[!UICONTROL Business] o versione successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licenza</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Devi essere un amministratore [!DNL Workfront]. Per informazioni sugli amministratori di [!DNL Workfront], vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pacchetto di supporto</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] o [!UICONTROL Enterprise]</p> <p>Il pacchetto di supporto standard non ha accesso alla sandbox di aggiornamento personalizzata, ma alla sandbox di anteprima.</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aggiornamento della sandbox di aggiornamento personalizzata

La sandbox di aggiornamento personalizzata contiene i dati di produzione effettivi e non viene aggiornata finché non li pianifichi. È possibile pianificare un aggiornamento in qualsiasi momento e con una frequenza settimanale.

>[!NOTE]
>
>* Impossibile pianificare un aggiornamento per il giorno corrente. Ad esempio, se oggi è il 1° giugno, il primo giorno in cui puoi pianificare un aggiornamento è il 2 giugno.
>* L’aggiornamento pianificato viene eseguito durante la notte, in base al cluster dell’utente (i cluster degli Stati Uniti aggiornano durante la notte negli Stati Uniti). L’ora specifica è imprevedibile a causa della presenza di altri clienti in coda e della quantità di dati aggiornati. Se la coda include molti clienti di grandi dimensioni, l&#39;aggiornamento potrebbe essere eseguito solo più tardi nello stesso giorno o il giorno successivo.
>* La sandbox di aggiornamento personalizzata presenta sempre le stesse funzioni di prodotto dell’ambiente di produzione. Tuttavia, quando aggiorni la Sandbox di aggiornamento personalizzata, il marchio viene mantenuto solo per il colore di sfondo della schermata di accesso. La schermata di accesso e i logo della barra di navigazione sono reimpostati sui valori predefiniti di [!DNL Workfront] e le immagini di branding modificate prima dell&#39;aggiornamento non vengono visualizzate.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Accedere alla sandbox di aggiornamento personalizzata dall’ambiente di produzione {#access-the-custom-refresh-sandbox-from-your-production-environment}

In qualità di amministratore [!DNL Workfront], puoi accedere alla Sandbox di aggiornamento personalizzata dal tuo ambiente di produzione.

>[!NOTE]
>
>Se il tuo account si trova nel cluster 4 (cluster EMEA), non puoi accedere alla Sandbox di aggiornamento personalizzata dall’ambiente di produzione. Per ulteriori informazioni su come accedere alla sandbox di aggiornamento personalizzata quando si dispone di un account nel cluster 4, vedere [Accedere alla sandbox di aggiornamento personalizzata per gli account nel cluster 4 (account EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Accedere alla sandbox di aggiornamento personalizzata per gli account nel cluster 4 (account EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Per accedere alla sandbox di aggiornamento personalizzata:

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).

1. Fare clic su **[!UICONTROL Sistema]** >**[!UICONTROL Preferenze]**.

1. Nella sezione **[!UICONTROL Ambiente di prova]**, fare clic su **[!UICONTROL Sandbox 1]** o **[!UICONTROL Sandbox 2]**.

   Il pacchetto di supporto specifica se è possibile accedere a una o due sandbox di aggiornamento personalizzate.

1. Accedi utilizzando le credenziali Sandbox di aggiornamento personalizzate.

   Le credenziali Sandbox di aggiornamento personalizzate sono uguali alle credenziali di produzione, a meno che non siano state modificate dopo l’ultimo aggiornamento della Sandbox di aggiornamento personalizzata. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non vengono sincronizzati automaticamente.

   La Sandbox di aggiornamento personalizzata mostra la versione e la data dell’ultimo aggiornamento nel banner nella parte superiore dello schermo. Tutte le informazioni di produzione sono disponibili e pronte per essere utilizzate al termine di un aggiornamento.

## Accedere alla sandbox di aggiornamento personalizzata utilizzando un URL {#access-the-custom-refresh-sandbox-using-a-url}

Qualsiasi utente può accedere alla sandbox di aggiornamento personalizzata utilizzando un URL.

* [Accedere alla Sandbox di aggiornamento personalizzata per gli account nei cluster 1, 2, 3 e 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Accedere alla Sandbox di aggiornamento personalizzata per gli account sul cluster 4 (account EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Accedere alla Sandbox di aggiornamento personalizzata per gli account nei cluster 1, 2, 3 e 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

A seconda del pacchetto di supporto, è necessario avere accesso a una o due Sandbox di aggiornamento personalizzate.

Per accedere alla sandbox di aggiornamento personalizzata utilizzando un URL:

1. Passa a questo URL se disponi di una sola sandbox di aggiornamento personalizzata:

   `https://companyname.sb01.workfront.com` (URL precedente:`https://cr1.attasksandbox.com/`.)

   Oppure, se disponi di due sandbox di aggiornamento personalizzate, oltre agli URL indicati sopra, puoi passare al seguente URL per accedere alla seconda sandbox di aggiornamento personalizzata:

   `https://companyname.sb02.workfront.com` (URL precedente:`https://cr2.attasksandbox.com/`)

1. Nella schermata di accesso, effettua l’accesso utilizzando le credenziali Sandbox di aggiornamento personalizzate.
1. Le credenziali Sandbox di aggiornamento personalizzate sono uguali alle credenziali di produzione, a meno che tu non abbia modificato le credenziali di produzione dall’ultimo aggiornamento della Sandbox di aggiornamento personalizzata. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non vengono sincronizzati automaticamente.

### Accedere alla Sandbox di aggiornamento personalizzata per gli account sul cluster 4 (account EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Se l&#39;account [!DNL Workfront] si trova nel cluster 4 (cluster EMEA), è possibile accedere alla sandbox di aggiornamento personalizzata solo utilizzando un URL. Per individuare il cluster su cui si trova l’account, contatta il team di assistenza clienti.

A seconda del pacchetto di supporto, è necessario avere accesso a una o due Sandbox di aggiornamento personalizzate.

Per accedere alla sandbox di aggiornamento personalizzata utilizzando un URL:

1. Passa a questo URL se disponi di una sola sandbox di aggiornamento personalizzata:

   `https://companyname.sb01.workfront.com` (URL precedente:`https://cr3.attasksandbox.com`)

   Oppure

   Se disponi di due sandbox di aggiornamento personalizzate, accedi a uno di questi URL:

   `https://companyname.sb01.workfront.com` (URL precedente:`https://cr3.attasksandbox.com`)

   `https://companyname.sb02.workfront.com` (URL precedente:`https://cr4.attasksandbox.com`)

1. Nella schermata di accesso, effettua l’accesso utilizzando le credenziali Sandbox di aggiornamento personalizzate.

   Le credenziali Sandbox di aggiornamento personalizzate sono uguali alle credenziali di produzione, a meno che tu non abbia modificato le credenziali di produzione dall’ultimo aggiornamento della Sandbox di aggiornamento personalizzata. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non vengono sincronizzati automaticamente.

## Pianificare l’aggiornamento della sandbox di aggiornamento personalizzata

>[!IMPORTANT]
>
>La durata dell&#39;aggiornamento dipende dalle dimensioni dei dati da aggiornare. Durante il processo di aggiornamento, è fondamentale che l’ambiente sandbox di aggiornamento personalizzato non venga utilizzato in alcun modo (incluse le chiamate e le integrazioni API), in quanto ciò impedirà il corretto completamento dell’aggiornamento della sandbox. [!DNL Workfront] disabiliterà l&#39;ambiente sandbox di aggiornamento personalizzato prima dell&#39;inizio, ma è necessario terminare tutte le sessioni attive per garantire che l&#39;aggiornamento della sandbox abbia esito positivo.

Dopo aver pianificato un aggiornamento della Sandbox di aggiornamento personalizzata, puoi annullarlo facendo clic su [!UICONTROL Annulla] nella parte superiore della pagina. Puoi anche riprogrammarlo per un momento successivo.

>[!NOTE]
>
>Non è possibile pianificare aggiornamenti automatici della sandbox.

Per pianificare l’aggiornamento della sandbox di aggiornamento del cliente:

1. Accedi alla tua Sandbox di aggiornamento personalizzata.
1. Fai clic su **[!UICONTROL Pianifica]** nel banner nella parte superiore dello schermo e seleziona una data dal calendario.
1. Seleziona una data per l&#39;aggiornamento, quindi fai clic su **[!UICONTROL Pianifica aggiornamento]**.

## Passa alla produzione dalla sandbox di aggiornamento personalizzata

1. Accedi alla tua Sandbox di aggiornamento personalizzata.

   Per ulteriori informazioni sull&#39;accesso alla sandbox di aggiornamento personalizzata, vedere [Accedere alla sandbox di aggiornamento personalizzata dall&#39;ambiente di produzione](#access-the-custom-refresh-sandbox-from-your-production-environment) o [Accedere alla sandbox di aggiornamento personalizzata utilizzando un URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Fai clic su **[!UICONTROL Vai alla produzione]** nel banner nella parte superiore dello schermo.

   Ricorda che il lavoro svolto nella sandbox non sarà visibile nell&#39;ambiente [!UICONTROL production], in quanto il trasferimento dei dati è unidirezionale, dalla produzione alla sandbox di aggiornamento personalizzata e non viceversa.

## Ricevi e-mail dalla Sandbox di aggiornamento personalizzata

[!DNL Workfront] disabilita tutte le comunicazioni e-mail dall&#39;ambiente Sandbox di aggiornamento personalizzato. Se desideri ricevere notifiche e-mail dall’ambiente Sandbox di aggiornamento personalizzato, devi abilitare questa funzionalità nelle impostazioni utente. Per ulteriori informazioni sull&#39;abilitazione delle notifiche e-mail nell&#39;ambiente Sandbox di aggiornamento personalizzato, vedere [Abilitare la consegna di e-mail dall&#39;ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>La consegna dei rapporti e le notifiche push nell’app mobile sono sempre disabilitate per l’ambiente Sandbox di aggiornamento personalizzato. Né l&#39;utente né l&#39;amministratore [!DNL Workfront] possono abilitare la consegna dei report o le notifiche push per l&#39;app mobile quando si accede all&#39;ambiente Sandbox di aggiornamento personalizzato.\
>Per ulteriori informazioni sulle consegne di report per l&#39;ambiente di produzione, vedi [Panoramica sulla consegna dei report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Per ulteriori informazioni sulle notifiche push nell&#39;app mobile per l&#39;ambiente di produzione, vedi la sezione in .

## Configurare il Single Sign-On nella sandbox di aggiornamento personalizzata

Se desideri configurare la sandbox di aggiornamento personalizzata in modo che funzioni con una soluzione Single Sign-On, puoi farlo configurandola separatamente dall’ambiente di produzione. La configurazione SSO nella Sandbox di aggiornamento personalizzata è indipendente dalla configurazione SSO nell’ambiente di produzione.\
Quando aggiorni la Sandbox di aggiornamento personalizzata, le informazioni SSO non vengono copiate dall’ambiente di produzione per sovrascrivere la configurazione Sandbox di aggiornamento personalizzata.

I passaggi per configurare il single sign-on nella Sandbox di aggiornamento personalizzata sono simili a quelli per la configurazione nell’ambiente di produzione.\
Per ulteriori informazioni sulla configurazione di [!DNL Workfront] con SSO, vedere [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Non è disponibile se l&#39;istanza [!DNL Workfront] dell&#39;organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

## Ricalcolo automatico delle sequenze temporali del progetto

Il ricalcolo delle sequenze temporali consente ai responsabili di vedere in che modo forze esterne al progetto influiscono sulla sequenza temporale del progetto. La sequenza temporale di un progetto si riferisce alle date pianificate e previste per il progetto.

In qualità di amministratore di Workfront, puoi configurare quando Workfront ricalcola automaticamente le timeline dei progetti. Workfront può ricalcolare le sequenze temporali del progetto ogni notte o quando l’ambito del progetto cambia, oppure entrambe.

Per informazioni, vedere [Configurare i ricalcoli della sequenza temporale per i progetti](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Per l’ambiente Sandbox di aggiornamento personalizzato, il ricalcolo notturno è disattivato e le timeline del progetto non vengono ricalcolate automaticamente. È necessario ricalcolare manualmente la timeline del progetto per l’ambiente Sandbox di aggiornamento personalizzato. Per informazioni, vedere [Ricalcolare i timeline del progetto](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Uso previsto e disponibilità

* Gli ambienti sandbox di aggiornamento personalizzati di [!DNL Workfront] non sono destinati a test delle prestazioni o del carico. Piuttosto, utilizza questi ambienti per convalidare le funzionalità con i flussi di lavoro esistenti della tua organizzazione.

* I flussi di lavoro che coinvolgono i documenti devono concentrarsi sul processo e non sul test di carico. I file di grandi dimensioni non sono supportati negli ambienti Sandbox.

* Gli ambienti sandbox di aggiornamento personalizzati di [!DNL Workfront] devono essere sempre disponibili. Qualsiasi interruzione in un ambiente Sandbox di aggiornamento personalizzato Workfront durante il normale orario di lavoro sarà una priorità assoluta subito dopo la risoluzione di eventuali problemi di produzione. In caso di interruzione di un ambiente Sandbox di aggiornamento personalizzato di Workfront nei fine settimana (sabato e domenica), verrà risolto il problema in modo che l’ambiente sia in esecuzione per l’orario di lavoro di lunedì.

* La verifica non è disponibile negli ambienti Sandbox di aggiornamento personalizzati.
