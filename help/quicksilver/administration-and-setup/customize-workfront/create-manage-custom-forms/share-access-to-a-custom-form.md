---
title: Condivisione di un modulo personalizzato
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile configurare l’accesso per un modulo personalizzato per controllare chi (persona, ruolo, gruppo, team, azienda) può visualizzarlo, condividerlo e modificarlo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 1%

---

# Condivisione di un modulo personalizzato

È possibile configurare l’accesso per un modulo personalizzato per controllare chi (persona, ruolo, gruppo, team, azienda) può visualizzarlo, condividerlo e modificarlo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> <p>Per informazioni su come gli amministratori di Workfront concedono questo accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per sapere quale piano, tipo di licenza o configurazioni del livello di accesso si dispone, contattare l&#39;amministratore Workfront.

## Accesso ai moduli personalizzati {#access-to-custom-forms}

Per impostazione predefinita, quando si crea un nuovo modulo personalizzato e lo si allega a un oggetto, qualsiasi utente assegnato all’oggetto può visualizzare e compilare il modulo. Questo include gli utenti con licenze di richiesta e gli utenti esterni.

Tuttavia, su un oggetto in cui il modulo personalizzato non è già allegato, un utente (anche se ha un livello di accesso Planner) non può allegarlo dal menu a discesa Personalizza Forms, a meno che una delle seguenti affermazioni non sia vera:

* Un utente ha condiviso il modulo personalizzato con l’utente o con il proprio team, ruolo, gruppo o società, concedendo almeno l’autorizzazione Visualizza con l’opzione Allega a dati personalizzati selezionata
* L’utente dispone di una licenza Plan e il suo livello di accesso consente l’accesso amministrativo ai moduli personalizzati

## Condivisione di un modulo personalizzato

Anziché lasciare un modulo personalizzato nello stato di condivisione predefinito (descritto in [Accesso ai moduli personalizzati](#access-to-custom-forms) in questo articolo è possibile configurare livelli specifici di accesso al modulo per determinati utenti, ruoli di lavoro, gruppi, team e aziende.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Seleziona il modulo personalizzato, quindi fai clic su **Condividi**.
1. Nella casella visualizzata, sotto **Attribuire l’accesso al modulo personalizzato a**, inizia a digitare il nome dell’utente, del team, del ruolo del lavoro, del gruppo o della società con cui desideri condividere il modulo personalizzato, quindi premi **Invio** quando viene visualizzato il nome.
1. Per regolare l’accesso per l’utente, il team, il ruolo del lavoro, il gruppo o la società appena aggiunto, fai clic sul menu a discesa a destra del nome, quindi configura una delle seguenti opzioni disponibili e una delle relative impostazioni avanzate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizzare</td> 
      <td> <p>Possibilità di visualizzare e compilare il modulo personalizzato sugli oggetti.</p> <p><b>NOTA</b>: Per gli utenti con licenze Work, Review e Request, questa è l'opzione più alta disponibile.</p> <p>Fai clic su <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire quanto segue:</p> 
       <ul> 
        <li><strong>Allega a dati personalizzati</strong>: Possibilità di allegare il modulo personalizzato a progetti, attività e problemi per i quali dispongono dell’accesso Gestione</li> 
        <li> <p><strong>Condividi</strong>: Possibilità di condividere il modulo personalizzato con altri utenti del sistema</p> <p>Gli utenti con una licenza Work, Review o Request possono condividere un modulo personalizzato solo tramite l’API o un rapporto di moduli personalizzati. Per ulteriori informazioni, consulta .</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gestire</td> 
      <td> <p>Disponibile solo per gli utenti con una licenza Plan. </p> <p>Oltre a poter aggiungere il modulo agli oggetti che possono modificare, gli utenti possono anche modificare completamente il modulo personalizzato, ad esempio aggiungere, modificare ed eliminare campi.</p> <p>Fai clic su <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire quanto segue:</p> 
       <ul> 
        <li> <p><strong>Allega a dati personalizzati</strong>: Possibilità di allegare il modulo personalizzato a progetti, attività e problemi per i quali dispongono dell’accesso Gestione</p> </li> 
        <li><strong>Elimina</strong>: Elimina il modulo personalizzato dal sistema</li> 
        <li><strong>Condividi</strong>: Condividere il modulo personalizzato con altri utenti del sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti i passaggi 4-5 per aggiungere altri nomi all’elenco e configurare le relative opzioni.
1. (Facoltativo) Se si desidera limitare l’accesso al modulo personalizzato (su oggetti in cui è allegato) a quelli specificati nei passaggi precedenti, fare clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings-with-dn-arrow.jpg) nell&#39;angolo in alto a destra della casella di condivisione, quindi fai clic su **Rimuovere l&#39;accesso a livello di sistema**.

   Se cambi idea, puoi fare clic su **Rendere visibile il sistema a livello di sistema** (opzione predefinita).

   >[!NOTE]
   >
   >* Quando si rende visibile un modulo personalizzato a livello di sistema, gli utenti possono solo visualizzarlo e compilarlo sugli oggetti a cui sono assegnati, non collegarlo ad altri oggetti. È possibile concedere la possibilità di allegare il modulo personalizzato agli oggetti utilizzando l’opzione &quot;Allega dati personalizzati&quot; descritta al punto 5.
   >* La maggior parte delle organizzazioni desidera garantire che tutti gli utenti del sistema possano compilare un modulo personalizzato quando è associato a oggetti su cui lavorano e visualizzarne i dati nei rapporti. Se questo vale per la tua organizzazione, ti consigliamo di utilizzare &quot;**Rendere visibile il sistema a livello di sistema**.&quot; Quando l’opzione è configurata in questo modo, nella finestra di dialogo viene visualizzato &quot;Visible System-Wide&quot; (Sistema visibile):

   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Se si desidera creare un modulo personalizzato in cui gli utenti potrebbero immettere dati sensibili quando sono collegati a determinati oggetti, la condivisione è limitata *oggetti* potrebbe essere preferibile anziché limitare l’accesso al modulo stesso.

1. Fai clic su **Salva**.

## Rimuovere l’accesso a un modulo personalizzato

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Seleziona il modulo personalizzato, quindi fai clic su **Condividi**.
1. Nella casella visualizzata, fare clic sulla X a destra del nome dell’utente, del team, del ruolo, del gruppo o della società che non si desidera più avere accesso speciale al modulo.
1. (Facoltativo) Ripetete il passaggio precedente su per altri nomi da rimuovere.
1. Fai clic su **Salva**.
