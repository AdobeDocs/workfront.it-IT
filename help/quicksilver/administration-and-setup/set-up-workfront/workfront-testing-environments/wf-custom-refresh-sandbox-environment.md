---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: La [!DNL Adobe Workfront] Ambiente Sandbox di aggiornamento personalizzato
description: La Sandbox di aggiornamento personalizzato è un ambiente in cui puoi eseguire il test e lavorare utilizzando i dati dell’ambiente di produzione. È ideale anche per l'esecuzione di corsi di formazione e la determinazione delle funzionalità di configurazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 0%

---

# La [!DNL Adobe Workfront] Ambiente Sandbox di aggiornamento personalizzato

La Sandbox di aggiornamento personalizzato è un ambiente in cui puoi eseguire il test e lavorare utilizzando i dati dell’ambiente di produzione. È ideale anche per l&#39;esecuzione di corsi di formazione e la determinazione delle funzionalità di configurazione.

>[!NOTE]
>
>Si tratta di un ambiente diverso dalla Sandbox di anteprima, che è anche un ambiente di test che replica il tuo [!DNL Workfront] ambiente di produzione.
>
>* Le nuove funzioni vengono introdotte nella Sandbox Anteprima prima che siano disponibili in Produzione.
>* Le nuove funzioni non vengono introdotte nella Sandbox di aggiornamento personalizzato prima che siano disponibili in Produzione.
>
>  Inoltre, esiste un costo aggiuntivo per ottenere la Sandbox di aggiornamento personalizzato non necessaria per la Sandbox di anteprima.
>
>  Per ulteriori informazioni sulla Sandbox di anteprima, consulta [La [!DNL Adobe Workfront] Ambiente sandbox di anteprima](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] piano</td> 
   <td> <p>[!UICONTROL Business] o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licenza</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Devi essere un [!DNL Workfront] amministratore. Per informazioni su [!DNL Workfront] amministratori, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente pieno accesso amministrativo</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pacchetto di supporto</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] o [!UICONTROL Enterprise]</p> <p>Il pacchetto di supporto standard non ha accesso alla Sandbox di aggiornamento personalizzato, ma ha accesso alla Sandbox di anteprima.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aggiornamento della Sandbox di aggiornamento personalizzata

La Sandbox di aggiornamento personalizzato contiene i dati di produzione effettivi e non viene aggiornata finché non lo pianifichi. È possibile pianificare un aggiornamento in qualsiasi momento è conveniente, con la frequenza di una volta alla settimana.

>[!NOTE]
>
>* Non è possibile pianificare un aggiornamento per il giorno corrente. Ad esempio, se oggi è il 1° giugno, il primo giorno in cui è possibile pianificare un aggiornamento è il 2 giugno.
>* La Sandbox di aggiornamento personalizzato ha sempre le stesse funzionalità di prodotto dell&#39;ambiente di produzione. Tuttavia, quando aggiorni la Sandbox di aggiornamento personalizzato, conserva il branding solo per il colore di sfondo della schermata di accesso. I loghi della schermata di accesso e della barra di navigazione vengono reimpostati su [!DNL Workfront] le impostazioni predefinite e le immagini di branding modificate prima dell’aggiornamento non vengono visualizzate.
>




<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Accedere alla Sandbox di aggiornamento personalizzata dall&#39;ambiente di produzione {#access-the-custom-refresh-sandbox-from-your-production-environment}

Come [!DNL Workfront] amministratore, puoi accedere alla Sandbox di aggiornamento personalizzato dall’ambiente di produzione.

>[!NOTE]
>
>Se l&#39;account è nel cluster 4 (cluster EMEA), non è possibile accedere alla Sandbox di aggiornamento personalizzato dall&#39;ambiente di produzione. Per ulteriori informazioni su come accedere alla Sandbox di aggiornamento personalizzato quando si dispone di un account sul cluster 4, vedere [Accedere alla Sandbox di aggiornamento personalizzato per gli account nel cluster 4 (account EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Accedere alla Sandbox di aggiornamento personalizzato per gli account nel cluster 4 (account EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Per accedere alla Sandbox di aggiornamento personalizzata:

1. Fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![](assets/main-menu-icon.png) nell&#39;angolo superiore destro di [!DNL Adobe Workfront], quindi fai clic su **[!UICONTROL Configurazione]** ![](assets/gear-icon-settings.png).

1. Fai clic su **[!UICONTROL Sistema]** >**[!UICONTROL Preferenze]**.

1. In **[!UICONTROL Ambiente di test]** sezione, fai clic su **[!UICONTROL Sandbox 1]** o **[!UICONTROL Sandbox 2]**.

   Il pacchetto di supporto specifica se si dispone dell&#39;accesso a una o due sandbox di aggiornamento personalizzate.

1. Accedi utilizzando le tue credenziali Sandbox di aggiornamento personalizzate.

   Le credenziali della Sandbox di aggiornamento personalizzato sono uguali alle credenziali di produzione, a meno che non siano state modificate le credenziali di produzione dall’ultimo aggiornamento della Sandbox di aggiornamento personalizzato. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non si sincronizzano automaticamente.

   La Sandbox di aggiornamento personalizzato mostra la versione e la data dell’ultimo aggiornamento nel banner nella parte superiore dello schermo. Tutte le informazioni provenienti dalla produzione sono disponibili e sono pronte per essere utilizzate al termine di un aggiornamento.

## Accedere alla Sandbox di aggiornamento personalizzata utilizzando un URL {#access-the-custom-refresh-sandbox-using-a-url}

Qualsiasi utente può accedere alla Sandbox di aggiornamento personalizzata utilizzando un URL.

* [Accedere alla Sandbox di aggiornamento personalizzato per gli account su cluster 1,2,3 e 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Accedere alla Sandbox di aggiornamento personalizzato per gli account nel cluster 4 (account EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Accedere alla Sandbox di aggiornamento personalizzato per gli account su cluster 1,2,3 e 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

A seconda del pacchetto di supporto, dovresti avere accesso a una o due sandbox di aggiornamento personalizzate.

Per accedere alla Sandbox di aggiornamento personalizzata utilizzando un URL:

1. Passa a questo URL se disponi di una sola Sandbox di aggiornamento personalizzato:

   https://companyname.sb01.workfront.com (URL vecchio:https:/cr1.attasksandbox.)

   Oppure se disponi di due Sandbox di aggiornamento personalizzato, oltre agli URL di cui sopra, puoi anche andare al seguente URL per accedere alla tua seconda Sandbox di aggiornamento personalizzato:

   https://companyname.sb02.workfront.com (URL vecchio:https:/cr2.attasksandbox)

1. Nella schermata di accesso, accedi utilizzando le tue credenziali Sandbox di aggiornamento personalizzate.
1. Le credenziali della Sandbox di aggiornamento personalizzato sono uguali alle credenziali di produzione, a meno che non siano state modificate le credenziali di produzione dall’ultimo aggiornamento della Sandbox di aggiornamento personalizzato. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non si sincronizzano automaticamente.

### Accedere alla Sandbox di aggiornamento personalizzato per gli account nel cluster 4 (account EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Se [!DNL Workfront] l&#39;account è nel cluster 4 (cluster EMEA), è possibile accedere alla Sandbox di aggiornamento personalizzato solo utilizzando un URL. Per sapere su quale cluster si trova il tuo account, contatta il nostro team di assistenza clienti.

A seconda del pacchetto di supporto, dovresti avere accesso a una o due sandbox di aggiornamento personalizzate.

Per accedere alla Sandbox di aggiornamento personalizzata utilizzando un URL:

1. Passa a questo URL se disponi di una sola Sandbox di aggiornamento personalizzato:

   https://companyname.sb01.workfront.com (URL vecchio:https:/cr3.attasksandbox)

   Oppure

   Passa a uno di questi URL se disponi di due Sandbox di aggiornamento personalizzate:

   https://companyname.sb01.workfront.com (URL vecchio:https:/cr3.attasksandbox)

   https://companyname.sb02.workfront.com (URL vecchio:https:/cr4.attasksandbox)

1. Nella schermata di accesso, accedi utilizzando le tue credenziali Sandbox di aggiornamento personalizzate.

   Le credenziali della Sandbox di aggiornamento personalizzato sono uguali alle credenziali di produzione, a meno che non siano state modificate le credenziali di produzione dall’ultimo aggiornamento della Sandbox di aggiornamento personalizzato. Gli accessi vengono sincronizzati solo quando si verifica un aggiornamento. Non si sincronizzano automaticamente.

## Pianifica un aggiornamento della Sandbox di aggiornamento personalizzato

>[!IMPORTANT]
>
>La durata dell’aggiornamento dipende dalla dimensione dei dati da aggiornare. Durante il processo di aggiornamento, è fondamentale che l’ambiente sandbox di aggiornamento personalizzato non venga utilizzato in alcun modo (incluse le chiamate API e le integrazioni), in quanto ciò impedirà il corretto completamento dell’aggiornamento della sandbox. [!DNL Workfront] disabilita l’ambiente sandbox di aggiornamento personalizzato prima dell’inizio, ma è necessario terminare tutte le sessioni attive per garantire che l’aggiornamento della sandbox abbia esito positivo.

Dopo aver pianificato un aggiornamento della Sandbox di aggiornamento personalizzato, puoi annullarla facendo clic su [!UICONTROL Annulla] nella parte superiore della pagina. Puoi anche riprogrammarlo in un secondo momento.

>[!NOTE]
>
>Non è possibile pianificare aggiornamenti automatici della sandbox.

Per pianificare un aggiornamento della Sandbox di aggiornamento del cliente:

1. Accedi alla tua Sandbox di aggiornamento personalizzata.
1. Fai clic su **[!UICONTROL Pianificazione]** nel banner nella parte superiore dello schermo e seleziona una data dal calendario.
1. Seleziona una data per l&#39;aggiornamento, quindi fai clic su **[!UICONTROL Pianifica aggiornamento]**.

## Passa a Produzione dalla Sandbox di aggiornamento personalizzato

1. Accedi alla tua Sandbox di aggiornamento personalizzata.

   Per ulteriori informazioni sull&#39;accesso alla Sandbox di aggiornamento personalizzato, vedi [Accedere alla Sandbox di aggiornamento personalizzata dall&#39;ambiente di produzione](#access-the-custom-refresh-sandbox-from-your-production-environment) o [Accedere alla Sandbox di aggiornamento personalizzata utilizzando un URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Fai clic su **[!UICONTROL Vai a produzione]** nel banner nella parte superiore dello schermo.

   Ricorda che il lavoro svolto nella sandbox non sarà visibile nella [!UICONTROL produzione] ambiente, poiché il trasferimento di dati è unidirezionale, dalla produzione alla Sandbox di aggiornamento personalizzato, e non al contrario.

## Ricevi e-mail dalla Sandbox di aggiornamento personalizzato

[!DNL Workfront] disabilita tutte le comunicazioni e-mail dall’ambiente Sandbox di aggiornamento personalizzato. Se desideri ricevere notifiche e-mail dall’ambiente Sandbox di aggiornamento personalizzato, devi abilitare questa funzionalità nelle impostazioni utente. Per ulteriori informazioni sull’abilitazione delle notifiche e-mail nell’ambiente Sandbox di aggiornamento personalizzato, consulta [Abilitare la consegna di e-mail dall’ambiente Sandbox di anteprima](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Le notifiche di consegna dei rapporti e push nell’app mobile sono sempre disabilitate per l’ambiente Sandbox di aggiornamento personalizzato. Né tu né il [!DNL Workfront] l’amministratore può abilitare la consegna dei rapporti o le notifiche push per l’app mobile quando accedi all’ambiente Sandbox di aggiornamento personalizzato.\
>Per ulteriori informazioni sulle consegne di rapporti per l’ambiente di produzione, consulta [Panoramica sulla consegna dei rapporti](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Per ulteriori informazioni sulle notifiche push nell’app mobile per l’ambiente di produzione, consulta la sezione in .

## Configurare il Single Sign-On nella Sandbox di aggiornamento personalizzata

Se desideri configurare la Sandbox di aggiornamento personalizzato per l’utilizzo con una soluzione Single Sign-On, puoi farlo configurandola separatamente dall’ambiente di produzione. La configurazione SSO nella Sandbox di aggiornamento personalizzato è indipendente dalla configurazione SSO nell&#39;ambiente di produzione.\
Quando si aggiorna la Sandbox di aggiornamento personalizzato, le informazioni SSO non vengono copiate dall&#39;ambiente di produzione per sovrascrivere la configurazione Sandbox di aggiornamento personalizzato.

I passaggi per la configurazione del single sign-on nella Sandbox di aggiornamento personalizzato sono simili a quelli per la configurazione nell’ambiente di produzione.\
Per ulteriori informazioni sulla configurazione [!DNL Workfront] con SSO, vedi [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Questa opzione non è disponibile se l’ [!DNL Workfront] L’istanza è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.

## Uso e disponibilità previsti

[!DNL Workfront] Gli ambienti Sandbox di aggiornamento personalizzati non sono destinati a test delle prestazioni o del carico. Utilizza piuttosto questi ambienti per convalidare la funzionalità con i flussi di lavoro esistenti della tua organizzazione.

[!DNL Workfront] Gli ambienti Sandbox di aggiornamento personalizzati sono sempre disponibili. Qualsiasi interruzione in un ambiente Sandbox di aggiornamento personalizzato di Workfront durante le normali ore di lavoro sarà una priorità assoluta immediatamente dopo la risoluzione di eventuali problemi di produzione, se presenti. Qualsiasi interruzione in un ambiente Sandbox di aggiornamento personalizzato di Workfront nei fine settimana (sabato e domenica) sarà risolta in modo che l&#39;ambiente sia in esecuzione per le ore di lavoro del lunedì.
