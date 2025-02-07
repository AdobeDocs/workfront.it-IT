---
title: Personalizza la tua istanza Adobe Workfront
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: In qualità di amministratore di Workfront, puoi inserire i logo di Workfront nella schermata di accesso, nell’area di navigazione superiore e nel menu principale. È inoltre possibile modificare l'immagine di sfondo e il colore della schermata di accesso.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 94603393-bdea-4673-9256-08da14f6916e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 1%

---

# Assegnare un brand all’istanza Adobe Workfront

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state caricate in [!DNL Adobe Experience Cloud].
>
> Se per la tua organizzazione è stato eseguito l&#39;onboarding in [!DNL Adobe Experience Cloud], il branding non è disponibile.

In qualità di amministratore di Workfront, puoi aggiungere i logo di Workfront nelle seguenti posizioni:

* Schermata di accesso

  ![Marchio nella schermata di accesso](assets/brand-login-screen-nwe-adobe.jpg)

* Area di navigazione superiore

  ![Marchio nella navigazione superiore](assets/brand-top-nav-area-nwe-adobe.jpg)

* Menu principale

  ![Marchio nel menu principale](assets/brand-main-menu-adobe.jpg)

È inoltre possibile modificare l&#39;immagine di sfondo e il colore della schermata di accesso:

![Banner nella schermata di accesso](assets/wf_banner_on_login_screen-adobe.png)

>[!NOTE]
>
>* La modifica dell&#39;immagine e del colore di sfondo per l&#39;accesso non è disponibile se l&#39;istanza Workfront dell&#39;organizzazione utilizza un portale SSO personalizzato. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.
><!--
>or is enabled with Adobe IMS  >
>  >
>-->
>
>* Un amministratore di Workfront o un amministratore di gruppo può anche inserire un marchio Workfront per determinati gruppi e utenti utilizzando un modello di layout. Il branding in un modello di layout sostituisce il branding a livello di sistema illustrato in questo articolo. Per istruzioni sul branding in un modello di layout, consulta [Brand Adobe Workfront utilizzando un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p>
       <p>Oppure</p>
       <p>Corrente: Piano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizzare la schermata di accesso

{{step-1-to-setup}}

1. Fai clic su **Sistema** > **Marchio**.

1. Per personalizzare Workfront con le immagini di branding, effettuare una delle seguenti modifiche.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Contrassegna l'icona Home <span style="font-weight: normal;"> (viene visualizzata all'estrema sinistra dell'area di navigazione superiore)</span></p> </td> 
      <td> <p>Nella sezione <strong>Area di navigazione superiore</strong>, in <strong>Icona Home</strong>, fai clic in un punto qualsiasi della casella, quindi individua e seleziona l'immagine del logo. Oppure trascina un’immagine nella casella.</p> <p>Per ritagliare l'immagine, utilizzare i controlli di scorrimento e trascinare l'immagine nella posizione desiderata all'interno dello spazio prescritto.</p> <p>Si consiglia un'immagine 120 x 120. Può essere in uno dei seguenti formati: GIF, JPG, PNG, SVG.</p> <p>Questa icona viene visualizzata anche nei report, elenchi, dashboard e report consegnati che gli utenti esportano come file PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Marchio il logo del menu principale <img src="assets/main-menu-icon.png"> <span style="font-weight: normal;">(viene visualizzato nell'angolo superiore destro del menu principale)</span></p> </td> 
      <td> <p>Nella sezione <strong>Area di navigazione superiore</strong>, in <strong>Logo menu principale</strong>, fai clic in un punto qualsiasi della casella, quindi individua e seleziona l'immagine del tuo logo. Oppure trascina un’immagine nella casella.</p> <p>Per ritagliare l'immagine, utilizzare i controlli di scorrimento e trascinare l'immagine nella posizione desiderata all'interno dello spazio prescritto.</p> <p>Si consiglia un'immagine di 300 x 120 pixel. Può essere in uno dei seguenti formati: GIF, JPG, PNG, SVG.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Imposta il logo della schermata di accesso <span style="font-weight: normal;"> (viene visualizzato in alto a sinistra nella casella in cui gli utenti digitano le credenziali di accesso)</span></td> 
      <td> <p>In <strong>Schermata di accesso</strong>, fai clic in un punto qualsiasi della casella, quindi individua e seleziona l'immagine del logo. Per ritagliare l'immagine, utilizzare i controlli di scorrimento e trascinare l'immagine nella posizione desiderata all'interno dello spazio prescritto.</p> <p>Si consiglia un'immagine di 300 x 120 pixel. Può essere in uno dei seguenti formati: GIF, JPG, PNG, SVG.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Contrassegna il colore di sfondo della schermata di accesso <span style="font-weight: normal;"> (viene visualizzato dietro la casella in cui gli utenti digitano le credenziali di accesso)</span></td> 
      <td> <p>In <strong>Schermata di accesso</strong>, impostare un <strong>Colore di sfondo</strong>. </p> <p>È possibile utilizzare codici colore RGB o HEX.</p> <p>Il colore di sfondo è visibile solo se lo sfondo della schermata di accesso è più grande dell'immagine di sfondo della schermata di accesso (vedere la riga successiva in questa tabella) o se l'immagine è trasparente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Imposta il marchio per l'immagine di sfondo della schermata di accesso <span style="font-weight: normal;">(viene visualizzata dietro la casella in cui gli utenti digitano le credenziali di accesso)</span></td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1"> <p> Nell'area <strong>Schermata di accesso</strong>, in <strong>Immagine di sfondo</strong>, fai clic sulla casella, quindi individua e seleziona l'immagine o le immagini JPG/PNG (fino a 20 ). </p> <p>Più immagini di sfondo vengono visualizzate in ordine casuale, cambiando ogni volta che gli utenti aggiornano la pagina di accesso. Si consiglia di usare immagini non superiori a 2 MB.</p> </li> 
        <li value="2"> <p>Passa il puntatore del mouse su ciascuna immagine di sfondo caricata, fai clic sull’icona Impostazioni (ingranaggio) e utilizza una delle seguenti opzioni per specificare dove e come visualizzare l’immagine nello sfondo della schermata di accesso:</p> 
         <ul> 
          <li> <p><strong>Schermata di riempimento</strong>: adatta l'immagine allo sfondo della schermata di accesso, che potrebbe ingrandirla. Utilizzare un'immagine ad alta risoluzione (fino a 2 MB) per ottenere risultati ottimali.</p> <p>Quando si utilizza questa opzione, il banner Workfront, che non è personalizzabile, nasconde parte dell’immagine.</p> </li> 
          <li> <p><strong>Sezione</strong>: affianca l'immagine nell'area di sfondo della schermata di accesso, nelle dimensioni originali. Questa opzione è utile per creare una serie. Selezionate un'opzione di allineamento blu per avviare l'affiancamento dall'angolo superiore sinistro, dall'alto centrale o dall'alto destro dell'area di sfondo.</p> </li> 
          <li> <p><strong>Posizione</strong>: inserisce l'immagine nelle dimensioni originali nella posizione scelta utilizzando una delle opzioni di allineamento blu: in alto a sinistra, in alto al centro o in alto a destra nell'area di sfondo della schermata di accesso.</p> <p>Il colore di sfondo riempie il resto dell'area di sfondo della schermata di accesso. Per ulteriori informazioni sul colore di sfondo, vedere la riga precedente in questa tabella.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ripristina il marchio predefinito</td> 
      <td> <p>Se si ripristina il marchio predefinito, verranno eliminate tutte le foto e le immagini caricate.</p> <p>Fai clic su <strong>Reimposta tutto il branding sui valori predefiniti di Workfront</strong> nell'angolo inferiore destro dello schermo, quindi fai clic su <strong>Sì</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Questa opzione non è disponibile se l’istanza Workfront dell’organizzazione utilizza un portale SSO personalizzato.
   ><!--   >
   >or is enabled with Adobe IMS   >
   >   >
   >-->
   >
   >Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

1. Fai clic su **Salva**.
