---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: L'ambiente Sandbox  [!DNL Adobe Workfront] Anteprima
description: L’ambiente Sandbox di anteprima è un ambiente di test che funge da replica dell’ambiente live. Viene aggiornato ogni fine settimana da Workfront. I dati aggiunti all’ambiente live il venerdì vengono visualizzati nella Sandbox di anteprima entro il lunedì successivo. Tutti i pacchetti di supporto hanno accesso a questa sandbox.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 6aa0aa5b8ffd088e3d79e7d1be66373a7f753f99
workflow-type: tm+mt
source-wordcount: '1310'
ht-degree: 0%

---

# L&#39;ambiente Sandbox di anteprima [!DNL Adobe Workfront]

<!-- Audited: 12/2023 -->

Esistono due ambienti di test per [!DNL Workfront] che sono repliche dell&#39;ambiente di produzione [!DNL Workfront]:

* Sandbox di anteprima

  L&#39;ambiente Sandbox di anteprima è un ambiente di test che funge da replica dell&#39;ambiente live ed è aggiornato ogni fine settimana da [!DNL Workfront]. I dati aggiunti all’ambiente live il venerdì vengono visualizzati nella Sandbox di anteprima entro il lunedì successivo.

  Tutti i pacchetti di supporto hanno accesso alla Sandbox di anteprima.

* Sandbox di aggiornamento personalizzata

  La sandbox di aggiornamento personalizzata è un ambiente di test separato che viene aggiornato manualmente dall’utente. Per ottenere la Sandbox di aggiornamento personalizzata è necessario un costo aggiuntivo. Per ulteriori informazioni su questo ambiente, vedere [L&#39;ambiente Sandbox di aggiornamento personalizzato [!DNL Adobe Workfront] ](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p>Pacchetto di supporto <strong>[!UICONTROL Standard]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus], [!UICONTROL Preferred] e [!UICONTROL Enterprise] pacchetti di supporto</strong> </p> </th> 
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

I dati scorrono in modo unidirezionale, dalla produzione all’anteprima e non viceversa. Un aggiornamento dell&#39;ambiente di anteprima viene sempre pianificato da [!DNL Workfront] ogni fine settimana.

L&#39;anteprima della sandbox consente inoltre a [!DNL Workfront] di distribuire nuove funzioni in un ambiente sicuro prima che siano pronte per essere distribuite in produzione. Puoi testare le nuove funzioni e fornire a [!DNL Workfront] feedback sulle loro funzionalità accedendo alla Sandbox di anteprima. Per questo motivo, il codice della sandbox di anteprima è sempre precedente al codice di produzione, anche se i dati vengono aggiornati settimanalmente.

L’ambiente di anteprima è ideale per l’esecuzione di corsi di formazione, il test di nuove funzioni e la determinazione delle funzionalità di configurazione.

>[!NOTE]
>
>Quando accedi all’anteprima sandbox, osserva il banner blu nella parte superiore dello schermo. Impossibile rimuovere il banner mentre si lavora in questo ambiente.
>
>Sul banner vengono visualizzati il nome dell’ambiente a cui stai effettuando l’accesso (Anteprima) e la versione di rilascio del codice. Fare clic su **[!UICONTROL Visualizza le novità]** per ulteriori informazioni sulla versione.
>
>![Anteprima banner](assets/preview-banner-nwe-350x161.png)

## Accesso alla sandbox di anteprima

Per impostazione predefinita, in qualità di amministratore [!DNL Workfront], hai accesso all&#39;ambiente sandbox [!UICONTROL Anteprima]. Se non riesci ad accedere all&#39;ambiente sandbox [!UICONTROL Anteprima] come descritto in questa sezione, contatta l&#39;amministratore di [!DNL Workfront] o il nostro team di assistenza clienti.


### Accesso alla sandbox di anteprima dall&#39;interfaccia [!DNL Workfront] {#accessing-the-preview-sandbox-from-the-workfront-interface}

In qualità di amministratore [!DNL Workfront], puoi accedere alla Sandbox di anteprima tramite l&#39;interfaccia [!DNL Workfront].

Per accedere alla sandbox di anteprima:

{{step-1-to-setup}}

1. Fare clic su **[!UICONTROL Sistema]** > **[!UICONTROL Preferenze]**.

1. Nella sezione **[!UICONTROL Ambienti di test]**, fai clic su **[!UICONTROL Anteprima sandbox]**.

1. Accedi con le credenziali di anteprima.

   Devono essere uguali alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non vengono sincronizzati automaticamente.

### Accesso alla sandbox di anteprima tramite un URL {#accessing-the-preview-sandbox-using-a-url}

Puoi accedere alla sandbox di anteprima utilizzando un URL.

#### Accesso alla sandbox di anteprima per gli account nei cluster 1, 2, 3 e 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

URL della sandbox di anteprima: `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Se hai dei segnalibri che si collegano al vecchio URL per la Sandbox di anteprima, prendi nota di questa modifica e aggiorna l’URL nei tuoi segnalibri.

Per accedere alla sandbox di anteprima utilizzando un URL:

1. Passare a questo URL: `https://companyname.preview.workfront.com/`.

   Se sei un cliente EMEA e il tuo account si trova nel cluster 4, consulta la sezione Accesso alla sandbox di anteprima per gli account nel cluster 4 (account EMEA) di seguito.

1. Accedi utilizzando le credenziali di anteprima.

   >[!TIP]
   >
   >Le credenziali di anteprima devono essere uguali alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non vengono sincronizzati automaticamente.


#### Accesso alla sandbox di anteprima per gli account sul cluster 4 (account EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Per accedere alla sandbox di anteprima utilizzando un URL:

1. Passare a questo URL: `https://companyname.preview.workfront.com/`.

   Puoi anche accedere alla sandbox di anteprima da [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Accedi utilizzando le credenziali di anteprima.

   Le credenziali di anteprima devono essere uguali alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non vengono sincronizzati automaticamente.

## Ricezione di e-mail dalla sandbox di anteprima

Workfront disabilita tutte le comunicazioni e-mail dall’ambiente Sandbox di anteprima. Se desideri ricevere notifiche e-mail dall’ambiente Sandbox di anteprima, devi abilitare questa funzionalità nelle impostazioni utente. Per ulteriori informazioni sull&#39;abilitazione delle notifiche e-mail nell&#39;ambiente Sandbox di anteprima, vedere [Abilitare la consegna di e-mail dall&#39;ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>La consegna dei rapporti e le notifiche push nell’app mobile sono sempre disabilitate per l’ambiente Sandbox di anteprima. Né l&#39;utente né l&#39;amministratore [!DNL Workfront] possono abilitare la consegna dei rapporti o le notifiche push per l&#39;app mobile quando si accede all&#39;ambiente Sandbox di anteprima.
>
>Per ulteriori informazioni sulle consegne di report per l&#39;ambiente di produzione, vedere [Panoramica sulla consegna dei report](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Single Sign-On (SSO)

Se utilizzi l&#39;SSO, collabora con il nostro team di Assistenza clienti per assicurarti che sia configurato correttamente in modo da poter utilizzare le credenziali SSO per accedere alla sandbox [!UICONTROL Anteprima]. Se l&#39;accesso iniziale non riesce, contattare il supporto tecnico o l&#39;amministratore [!DNL Workfront].

Per ulteriori informazioni sul Single Sign-On, vedere [Panoramica del Single Sign-On in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configurazione del Single Sign-On nella sandbox di anteprima

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state caricate in [!DNL Adobe Admin Console]. Se la tua organizzazione è stata integrata in [!DNL Adobe Admin Console], non è necessaria alcuna azione.
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata in [!DNL Adobe Admin Console], vedere [Differenze di amministrazione basate su Platform ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Se desideri configurare la sandbox di anteprima in modo che funzioni con una soluzione Single Sign-On, puoi farlo configurandola separatamente dall’ambiente di produzione. La configurazione SSO nella Sandbox di anteprima è indipendente dalla configurazione SSO nell’ambiente di produzione.

Quando la Sandbox di anteprima viene aggiornata (ogni fine settimana), le informazioni SSO non vengono copiate dall’ambiente di produzione per sovrascrivere la configurazione Sandbox di anteprima.

I passaggi per configurare il single sign-on nella Sandbox di anteprima sono simili a quelli per la configurazione nell’ambiente di produzione.

Per ulteriori informazioni sulla configurazione di [!DNL Workfront] con SSO, vedere [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Ricalcolo automatico delle sequenze temporali del progetto

Il ricalcolo delle sequenze temporali consente ai responsabili di vedere in che modo forze esterne al progetto influiscono sulla sequenza temporale del progetto. La sequenza temporale di un progetto si riferisce alle date pianificate e previste per il progetto.

In qualità di amministratore di Workfront, puoi configurare quando Workfront ricalcola automaticamente le timeline dei progetti. Workfront può ricalcolare le sequenze temporali del progetto ogni notte o quando l’ambito del progetto cambia, oppure entrambe.

Per informazioni, vedere [Configurare i ricalcoli della sequenza temporale per i progetti](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Per l’ambiente di anteprima, il ricalcolo notturno è disattivato e le timeline del progetto non vengono ricalcolate automaticamente. È necessario ricalcolare manualmente la timeline del progetto per l’ambiente di anteprima. Per informazioni, vedere [Ricalcolare i timeline del progetto](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Anteprima delle prestazioni e della disponibilità dell’ambiente

* Gli ambienti di anteprima [!DNL Workfront] non sono destinati a test delle prestazioni o del carico. Piuttosto, utilizza questi ambienti per convalidare le funzionalità con i flussi di lavoro esistenti della tua organizzazione.

* I flussi di lavoro che coinvolgono i documenti devono concentrarsi sul processo e non sul test di carico. I file di grandi dimensioni non sono supportati negli ambienti Sandbox.

* Gli ambienti di anteprima [!DNL Workfront] devono essere sempre disponibili.

* Qualsiasi interruzione in un ambiente di anteprima [!DNL Workfront] durante il normale orario di lavoro sarà una priorità assoluta subito dopo la risoluzione di eventuali problemi di produzione.

* Eventuali interruzioni di un ambiente di anteprima [!DNL Workfront] nei fine settimana (sabato e domenica) verranno risolte in modo che l&#39;ambiente sia in esecuzione per l&#39;orario di lavoro di lunedì.

* La bozza non è disponibile nell’ambiente di anteprima.
