---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: La [!DNL Adobe Workfront] Ambiente sandbox di anteprima
description: La Sandbox di anteprima è un ambiente di test che funge da replica dell’ambiente live. Viene aggiornato ogni fine settimana da Workfront. I dati aggiunti all’ambiente live il venerdì vengono visualizzati nella Sandbox Anteprima entro il lunedì successivo. Tutti i pacchetti di supporto hanno accesso a questa sandbox.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 0%

---

# La [!DNL Adobe Workfront] Ambiente sandbox di anteprima

Esistono due ambienti di test per [!DNL Workfront] che sono repliche del [!DNL Workfront] ambiente di produzione:

* Sandbox di anteprima

   La Sandbox Anteprima è un ambiente di test che funge da replica dell’ambiente live e viene aggiornato ogni fine settimana per [!DNL Workfront]. I dati aggiunti all’ambiente live il venerdì vengono visualizzati nella Sandbox Anteprima entro il lunedì successivo.

   Tutti i pacchetti di supporto hanno accesso alla Sandbox di anteprima.

* Sandbox di aggiornamento personalizzato

   La Sandbox di aggiornamento personalizzato è un ambiente di test separato che viene aggiornato manualmente dall’utente. È presente un costo aggiuntivo per ottenere la Sandbox di aggiornamento personalizzato. Per ulteriori informazioni su questo ambiente, consulta [La [!DNL Adobe Workfront] Ambiente Sandbox di aggiornamento personalizzato](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Pacchetto di supporto [!UICONTROL Standard]</strong> </p> </th> 
   <th> <p><strong>Pacchetti di supporto [!UICONTROL Plus], [!UICONTROL Preferred] e [!UICONTROL Enterprise]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Anteprima sandbox</p> </td> 
   <td scope="col"> <p>↓</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Sandbox di aggiornamento personalizzato</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anteprima sandbox

La Sandbox di anteprima funge da ambiente in cui gli utenti della tua organizzazione possono eseguire in modo sicuro test e lavorare con i dati dell’ambiente di produzione senza influire sull’ambiente di produzione.

La sandbox Anteprima contiene i dati di produzione effettivi; tuttavia, si aggiorna ogni fine settimana in modo che i dati possano essere fino a una settimana dietro l&#39;ambiente di produzione. Gli elementi creati dopo l’ultimo aggiornamento si trovano nell’ambiente Sandbox di anteprima fino al successivo aggiornamento.

I dati scorrono in modo unidirezionale, dalla produzione all’anteprima e non al contrario. Un aggiornamento dell’ambiente di anteprima è sempre pianificato da [!DNL Workfront] ogni fine settimana. Per ulteriori informazioni sul giorno e l&#39;ora specifici dell&#39;aggiornamento, vai a [status.adobe.com](https://status.adobe.com/it/).

La funzione Anteprima sandbox consente inoltre di [!DNL Workfront] per implementare nuove funzionalità in un ambiente sicuro, prima che siano pronte per essere implementate in Produzione. Puoi testare le nuove funzioni e fornire [!DNL Workfront] feedback sulle loro funzionalità accedendo alla Sandbox di anteprima. Per questo motivo, il codice della Sandbox di anteprima è sempre in anticipo rispetto al codice di produzione, anche se i dati vengono aggiornati settimanalmente.

L’ambiente di anteprima è ideale per l’esecuzione di corsi di formazione, il test delle nuove funzioni e la determinazione delle funzionalità di configurazione.

>[!NOTE]
>
>Quando accedi alla Sandbox Anteprima, osserva il banner blu nella parte superiore dello schermo. Impossibile rimuovere il banner mentre si lavora in questo ambiente.
>
>Sul banner vengono visualizzati il nome dell’ambiente a cui si accede (Anteprima) e la versione di rilascio del codice. Fai clic su **[!UICONTROL Scopri le novità]** per informazioni su tale versione.
>
>![](assets/preview-banner-nwe-350x161.png)

## Accesso alla Sandbox di anteprima

Per impostazione predefinita, come [!DNL Workfront] amministratore, puoi accedere al [!UICONTROL Anteprima] Ambiente sandbox. Se non è possibile accedere al [!UICONTROL Anteprima] Ambiente sandbox come descritto in questa sezione, contatta il tuo [!DNL Workfront] amministratore o il nostro team di assistenza clienti.

* [Accesso alla Sandbox di anteprima dalla [!DNL Workfront] Interfaccia](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [Accesso alla Sandbox di anteprima utilizzando un URL](#accessing-the-preview-sandbox-using-a-url)

### Accesso alla Sandbox di anteprima dalla [!DNL Workfront] Interfaccia {#accessing-the-preview-sandbox-from-the-workfront-interface}

Come [!DNL Workfront] amministratore, puoi accedere alla Sandbox di anteprima tramite il [!DNL Workfront] interfaccia.

Per accedere alla Sandbox di anteprima:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Sistema]** > **[!UICONTROL Preferenze]**.

1. In **[!UICONTROL Ambienti di test]** sezione, fai clic su **[!UICONTROL Anteprima sandbox]**.

1. Accedi con le tue credenziali di anteprima.

   Devono corrispondere alle credenziali di produzione, a meno che non le abbiate modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non si sincronizzano automaticamente.

### Accesso alla Sandbox di anteprima utilizzando un URL {#accessing-the-preview-sandbox-using-a-url}

* [Accesso alla Sandbox di anteprima per gli account nel cluster 1, 2, 3 e 5](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [Accesso alla Sandbox di anteprima per gli account nel cluster 4 (account EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### Accesso alla Sandbox di anteprima per gli account nel cluster 1, 2, 3 e 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

Precedentemente, era possibile accedere alla Sandbox di anteprima andando [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg).

Questo URL non è più supportato e non è stato reindirizzato al nuovo URL per l’ambiente Sandbox di anteprima. Il nuovo URL corretto per la Sandbox di anteprima è: [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ).

>[!NOTE]
>
>Se i segnalibri erano collegati al vecchio URL per la Sandbox di anteprima, prendere nota di questa modifica e aggiornare l&#39;URL nei segnalibri.

Per accedere alla Sandbox di anteprima utilizzando un URL:

1. Passa a questo URL: [[!DNL https]://companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)

   Se sei un cliente EMEA e il tuo account è nel cluster 4, consulta la sezione . [Accesso alla Sandbox di anteprima per gli account nel cluster 4 (account EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) in questo articolo.

1. Accedi utilizzando le tue credenziali di anteprima.

   Le credenziali di anteprima devono corrispondere alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non si sincronizzano automaticamente.

#### Accesso alla Sandbox di anteprima per gli account nel cluster 4 (account EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Per accedere alla Sandbox di anteprima utilizzando un URL:

1. Passa a questo URL: `https://companyname.preview.workfront.com/`.

   Per accedere alla Sandbox di anteprima, vai a [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Accedi utilizzando le tue credenziali di anteprima.

   Le credenziali di anteprima devono corrispondere alle credenziali di produzione, a meno che non siano state modificate in Produzione dopo l’aggiornamento dell’anteprima. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non si sincronizzano automaticamente.

## Ricezione di e-mail dalla Sandbox di anteprima

Workfront disabilita tutte le comunicazioni e-mail dall’ambiente Sandbox di anteprima. Se desideri ricevere notifiche e-mail dall’ambiente Sandbox di anteprima, devi abilitare questa funzionalità nelle impostazioni utente. Per ulteriori informazioni sull’abilitazione delle notifiche e-mail nell’ambiente Sandbox di anteprima, consulta [Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Le notifiche di consegna dei rapporti e push nell’app mobile sono sempre disabilitate per l’ambiente Sandbox di anteprima. Né tu né il [!DNL Workfront] L’amministratore può abilitare la consegna dei rapporti o le notifiche push per l’app mobile quando accedi all’ambiente Sandbox di anteprima.
>
>Per ulteriori informazioni sulle consegne di rapporti per l’ambiente di produzione, consulta [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Single Sign-On (SSO)

Se utilizzi SSO, collabora con il nostro team di assistenza clienti per assicurarti che sia configurato correttamente in modo da poter utilizzare le tue credenziali SSO per accedere al [!UICONTROL Anteprima] Sandbox. Se l&#39;accesso iniziale non riesce, contatta il tuo contatto di supporto regolare o [!DNL Workfront] amministratore dell&#39;assistenza.

Per ulteriori informazioni sul Single Sign-On, consulta [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configurazione del Single Sign-On nella Sandbox di anteprima

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate [!DNL Adobe Admin Console]. Se la tua organizzazione è stata integrata nel [!DNL Adobe Admin Console], non è necessaria alcuna azione.
>
>Per un elenco delle procedure che variano a seconda che l&#39;organizzazione sia stata integrata o meno nel [!DNL Adobe Admin Console], vedi [Differenze di amministrazione basate su piattaforma ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Se desideri configurare la Sandbox di anteprima in modo che funzioni con una soluzione Single Sign-On, puoi farlo configurandola separatamente dall’ambiente di produzione. La configurazione SSO nella Sandbox di anteprima è indipendente dalla configurazione SSO nell&#39;ambiente di produzione.

Quando la Sandbox di anteprima viene aggiornata (ogni fine settimana), le informazioni SSO non vengono copiate dal tuo ambiente di produzione per sovrascrivere la configurazione della Sandbox di anteprima.

I passaggi per la configurazione del single sign-on nella Sandbox di anteprima sono simili a quelli per la configurazione nell’ambiente di produzione.

Per ulteriori informazioni sulla configurazione [!DNL Workfront] con SSO, vedi [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Anteprima delle prestazioni e della disponibilità dell&#39;ambiente

[!DNL Workfront] Gli ambienti di anteprima non sono destinati a test delle prestazioni o del carico. Utilizza piuttosto questi ambienti per convalidare la funzionalità con i flussi di lavoro esistenti della tua organizzazione.

[!DNL Workfront] Gli ambienti di anteprima sono sempre disponibili.

Qualsiasi interruzione a un [!DNL Workfront] L&#39;ambiente di anteprima durante l&#39;orario di lavoro regolare sarà una priorità assoluta immediatamente dopo la risoluzione di eventuali problemi di produzione, se presenti.

Qualsiasi interruzione a un [!DNL Workfront] L’ambiente di anteprima nei fine settimana (sabato e domenica) verrà affrontato in modo che l’ambiente sia in esecuzione per le ore lavorative del lunedì.
