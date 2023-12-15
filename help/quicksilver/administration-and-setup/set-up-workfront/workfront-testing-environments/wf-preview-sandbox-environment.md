---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Il [!DNL Adobe Workfront] Anteprima ambiente sandbox
description: L’ambiente Sandbox di anteprima è un ambiente di test che funge da replica dell’ambiente live. Viene aggiornato ogni fine settimana da Workfront. I dati aggiunti all’ambiente live il venerdì vengono visualizzati nella Sandbox di anteprima entro il lunedì successivo. Tutti i pacchetti di supporto hanno accesso a questa sandbox.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

# Il [!DNL Adobe Workfront] Anteprima ambiente sandbox

<!-- Audited: 12/2023 -->

Esistono due ambienti di test per [!DNL Workfront] che sono repliche del tuo [!DNL Workfront] ambiente di produzione:

* Sandbox di anteprima

  L’anteprima sandbox è un ambiente di test che funge da replica dell’ambiente live e viene aggiornato ogni fine settimana da [!DNL Workfront]. I dati aggiunti all’ambiente live il venerdì vengono visualizzati nella Sandbox di anteprima entro il lunedì successivo.

  Tutti i pacchetti di supporto hanno accesso alla Sandbox di anteprima.

* Sandbox di aggiornamento personalizzata

  La sandbox di aggiornamento personalizzata è un ambiente di test separato che viene aggiornato manualmente dall’utente. Per ottenere la Sandbox di aggiornamento personalizzata è necessario un costo aggiuntivo. Per ulteriori informazioni su questo ambiente, consulta [Il [!DNL Adobe Workfront] Ambiente sandbox di aggiornamento personalizzato](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Pacchetto di supporto di [!UICONTROL Standard]</strong> </p> </th> 
   <th> <p><strong>Pacchetti di supporto [!UICONTROL Plus], [!UICONTROL Preferred] e [!UICONTROL Enterprise]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Anteprima Sandbox</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Sandbox di aggiornamento personalizzato</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anteprima Sandbox

L’anteprima sandbox funge da ambiente in cui gli utenti dell’organizzazione possono testare e lavorare in modo sicuro con i dati dell’ambiente di produzione senza influire sull’ambiente di produzione.

La sandbox di anteprima contiene i dati di produzione effettivi; tuttavia, aggiorna ogni fine settimana in modo che i dati possano trovarsi fino a una settimana indietro rispetto all’ambiente di produzione. Gli elementi creati dall’ultimo aggiornamento si trovano nell’ambiente Sandbox di anteprima fino al successivo aggiornamento.

I dati scorrono in modo unidirezionale, dalla produzione all’anteprima e non viceversa. Un aggiornamento dell’ambiente di anteprima viene sempre pianificato da [!DNL Workfront] ogni fine settimana.

L’anteprima della sandbox consente anche di: [!DNL Workfront] per implementare le nuove funzioni in un ambiente sicuro, prima che siano pronte per l’implementazione in produzione. Puoi testare le nuove funzioni e fornire [!DNL Workfront] feedback sulle funzionalità mediante l’accesso alla sandbox di anteprima. Per questo motivo, il codice della sandbox di anteprima è sempre precedente al codice di produzione, anche se i dati vengono aggiornati settimanalmente.

L’ambiente di anteprima è ideale per l’esecuzione di corsi di formazione, il test di nuove funzioni e la determinazione delle funzionalità di configurazione.

>[!NOTE]
>
>Quando accedi all’anteprima sandbox, osserva il banner blu nella parte superiore dello schermo. Impossibile rimuovere il banner mentre si lavora in questo ambiente.
>
>Sul banner vengono visualizzati il nome dell’ambiente a cui stai effettuando l’accesso (Anteprima) e la versione di rilascio del codice. Clic **[!UICONTROL Scopri le novità]** per informazioni su tale versione.
>
>![](assets/preview-banner-nwe-350x161.png)

## Accesso alla sandbox di anteprima

Per impostazione predefinita, come [!DNL Workfront] amministratore, puoi accedere al [!UICONTROL Anteprima] Ambiente sandbox. Se non riesci ad accedere al [!UICONTROL Anteprima] Come descritto in questa sezione, contatta il tuo [!DNL Workfront] o il nostro team di assistenza clienti.


### Accesso alla sandbox di anteprima da [!DNL Workfront] Interfaccia {#accessing-the-preview-sandbox-from-the-workfront-interface}

As a [!DNL Workfront] amministratore, puoi accedere alla Sandbox di anteprima tramite il [!DNL Workfront] di rete.

Per accedere alla sandbox di anteprima:

1. Fai clic su **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Sistema]** > **[!UICONTROL Preferenze]**.

1. In **[!UICONTROL Ambienti di test]** , fare clic su **[!UICONTROL Anteprima sandbox]**.

1. Accedi con le credenziali di anteprima.

   Devono essere uguali alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non vengono sincronizzati automaticamente.

### Accesso alla sandbox di anteprima tramite un URL {#accessing-the-preview-sandbox-using-a-url}

Puoi accedere alla sandbox di anteprima utilizzando un URL.

#### Accesso alla sandbox di anteprima per gli account nei cluster 1, 2, 3 e 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

L’URL per la sandbox di anteprima è: `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Se hai dei segnalibri che si collegano al vecchio URL per la Sandbox di anteprima, prendi nota di questa modifica e aggiorna l’URL nei tuoi segnalibri.

Per accedere alla sandbox di anteprima utilizzando un URL:

1. Passa a questo URL: `https://companyname.preview.workfront.com/`.

   Se sei un cliente EMEA e il tuo account si trova nel cluster 4, consulta la sezione Accesso alla sandbox di anteprima per gli account nel cluster 4 (account EMEA) di seguito.

1. Accedi utilizzando le credenziali di anteprima.

   >[!TIP]
   >
   >Le credenziali di anteprima devono essere uguali alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non vengono sincronizzati automaticamente.


#### Accesso alla sandbox di anteprima per gli account sul cluster 4 (account EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Per accedere alla sandbox di anteprima utilizzando un URL:

1. Passa a questo URL: `https://companyname.preview.workfront.com/`.

   Puoi anche accedere all’anteprima sandbox da [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Accedi utilizzando le credenziali di anteprima.

   Le credenziali di anteprima devono essere uguali alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non vengono sincronizzati automaticamente.

## Ricezione di e-mail dalla sandbox di anteprima

Workfront disabilita tutte le comunicazioni e-mail dall’ambiente Sandbox di anteprima. Se desideri ricevere notifiche e-mail dall’ambiente Sandbox di anteprima, devi abilitare questa funzionalità nelle impostazioni utente. Per ulteriori informazioni sull’abilitazione delle notifiche e-mail nell’ambiente Sandbox di anteprima, consulta [Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>La consegna dei rapporti e le notifiche push nell’app mobile sono sempre disabilitate per l’ambiente Sandbox di anteprima. Né tu né il [!DNL Workfront] L’amministratore può abilitare la consegna dei rapporti o le notifiche push per l’app mobile quando accedi all’ambiente Sandbox di anteprima.
>
>Per ulteriori informazioni sulle consegne di rapporti per l’ambiente di produzione, consulta [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Single Sign-On (SSO)

Se utilizzi l’SSO, collabora con il nostro team di Assistenza clienti per assicurarti che sia configurato correttamente, in modo da poter utilizzare le credenziali SSO per accedere a [!UICONTROL Anteprima] Sandbox. Se l’accesso iniziale non riesce, contatta il regolare contatto di supporto oppure [!DNL Workfront] per assistenza.

Per ulteriori informazioni sul Single Sign-On, vedere [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configurazione del Single Sign-On nella sandbox di anteprima

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state caricate in [!DNL Adobe Admin Console]. Se per la tua organizzazione è stato eseguito l’onboarding in [!DNL Adobe Admin Console], non è necessaria alcuna azione.
>
>Per un elenco di procedure che differiscono in base al fatto che la tua organizzazione sia stata caricata su [!DNL Adobe Admin Console], vedi [Differenze di amministrazione basate sulla piattaforma ([!UICONTROL Adobe Workfront]/[!UICONTROL Piattaforma aziendale Adobe])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Se desideri configurare la sandbox di anteprima in modo che funzioni con una soluzione Single Sign-On, puoi farlo configurandola separatamente dall’ambiente di produzione. La configurazione SSO nella Sandbox di anteprima è indipendente dalla configurazione SSO nell’ambiente di produzione.

Quando la Sandbox di anteprima viene aggiornata (ogni fine settimana), le informazioni SSO non vengono copiate dall’ambiente di produzione per sovrascrivere la configurazione Sandbox di anteprima.

I passaggi per configurare il single sign-on nella Sandbox di anteprima sono simili a quelli per la configurazione nell’ambiente di produzione.

Per ulteriori informazioni sulla configurazione [!DNL Workfront] con SSO, vedi [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Anteprima delle prestazioni e della disponibilità dell’ambiente

[!DNL Workfront] Gli ambienti di anteprima non sono destinati al test delle prestazioni o del carico. Piuttosto, utilizza questi ambienti per convalidare le funzionalità con i flussi di lavoro esistenti della tua organizzazione.

[!DNL Workfront] Gli ambienti di anteprima sono sempre disponibili.

Eventuali interruzioni a un [!DNL Workfront] L’ambiente di anteprima durante il normale orario di lavoro sarà la prima priorità subito dopo la risoluzione di eventuali problemi di produzione.

Eventuali interruzioni a un [!DNL Workfront] L’ambiente di anteprima nei fine settimana (sabato e domenica) verrà gestito in modo che l’ambiente sia in esecuzione per l’orario di lavoro di lunedì.
