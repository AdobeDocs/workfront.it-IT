---
title: Condividere un modulo personalizzato
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile configurare l'accesso per un modulo personalizzato in modo da controllare chi, persona, ruolo, gruppo, team, azienda, può visualizzarlo, condividerlo e modificarlo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 6ddbe56dd187d62489c41ff721d0f071202e54e4
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 1%

---

# Condividere un modulo personalizzato

{{highlighted-preview}}

È possibile configurare l&#39;accesso per un modulo personalizzato in modo da controllare chi, persona, ruolo, gruppo, team, azienda, può visualizzarlo, condividerlo e modificarlo.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>piano Adobe Workfront</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Nuovo: Standard</p>
   <p>oppure</p>
   <p>Corrente: Piano</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Accesso ai moduli personalizzati {#access-to-custom-forms}

Per impostazione predefinita, quando si crea un nuovo modulo personalizzato e qualcuno lo allega a un oggetto, qualsiasi utente assegnato all’oggetto può visualizzare e compilare il modulo. Ciò include gli utenti con licenze di richiesta e gli utenti esterni.

Tuttavia, in un oggetto in cui il modulo personalizzato non è già allegato, un utente (anche se dispone di un livello di accesso Planner) non può allegarlo dal menu a discesa Forms personalizzato a meno che non si verifichi una delle seguenti condizioni:

* Qualcuno ha condiviso il modulo personalizzato con l’utente o con il suo team, mansione, gruppo o società, concedendo almeno l’autorizzazione Visualizzazione con l’opzione Allega a dati personalizzati selezionata
* L’utente dispone di una licenza Pianificazione e il suo livello di accesso consente l’accesso amministrativo ai moduli personalizzati

## Condividere un modulo personalizzato dall’elenco dei moduli

Anziché lasciare un modulo personalizzato nello stato di condivisione predefinito (come descritto in [Accesso ai moduli personalizzati](#access-to-custom-forms) in questo articolo), puoi configurare livelli specifici di accesso al modulo per determinati utenti, ruoli, gruppi, team e aziende.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Seleziona il modulo personalizzato, quindi fai clic su ![Icona Condividi](assets/share-icon.png).
1. Nella casella visualizzata, sotto **Concedi accesso al modulo personalizzato a**, inizia a digitare il nome dell’utente, del team, della mansione, del gruppo o dell’azienda con cui vuoi condividere il modulo personalizzato, quindi premi **Invio** quando viene visualizzato il nome.
1. Per regolare l’accesso per l’utente, il team, la mansione, il gruppo o la società appena aggiunti, fai clic sul menu a discesa a destra del nome, quindi configura una delle seguenti opzioni disponibili e le relative impostazioni avanzate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizzare</td> 
      <td> <p>Possibilità di visualizzare e compilare il modulo personalizzato sugli oggetti.</p> <p><b>NOTA</b>: per gli utenti con licenze Light e Contributor (o Licenze Lavoro, Revisione e Richiesta), questa è l’opzione più alta disponibile.</p> <p>Clic <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire quanto segue:</p> 
       <ul> 
        <li><strong>Allega a dati personalizzati</strong>: possibilità di allegare il modulo personalizzato a progetti, attività e problemi per i quali dispongono dell’accesso di gestione</li> 
        <li> <p><strong>Condividi</strong>: possibilità di condividere il modulo personalizzato con altri nel sistema</p> <p>Gli utenti con una licenza Light o Contributor (o Licenza Lavoro, Revisione o Richiesta) possono condividere un modulo personalizzato solo tramite l’API o un rapporto di moduli personalizzati.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gestire</td> 
      <td> <p>Disponibile solo per gli utenti con una licenza Standard o Plan. </p> <p>Oltre a poter aggiungere il modulo agli oggetti a cui hanno accesso per la modifica, gli utenti possono anche modificare completamente il modulo personalizzato, incluse le operazioni di aggiunta, modifica ed eliminazione dei campi.</p> <p>Clic <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire quanto segue:</p> 
       <ul> 
        <li> <p><strong>Allega a dati personalizzati</strong>: possibilità di allegare il modulo personalizzato a progetti, attività e problemi per i quali dispongono dell’accesso di gestione</p> </li> 
        <li><strong>Elimina</strong>: elimina il modulo personalizzato dal sistema</li> 
        <li><strong>Condividi</strong>: condividi il modulo personalizzato con altri nel sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti i passaggi 4-5 per aggiungere altri nomi all’elenco e configurarne le opzioni.
1. (Facoltativo) Se desideri limitare l’accesso al modulo personalizzato (sugli oggetti a cui è allegato) a quelli specificati nei passaggi precedenti, fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings-with-dn-arrow.jpg) nell&#39;angolo superiore destro della casella condivisione, quindi fare clic su **Rimuovi l&#39;accesso a livello di sistema**.

   Se cambi idea, puoi fare clic su **Rendi visibile a livello di sistema** (opzione predefinita).

   >[!NOTE]
   >
   >* Quando si rende visibile un modulo personalizzato a livello di sistema, è possibile consentire agli utenti di visualizzarlo e compilarlo solo sugli oggetti a cui sono assegnati, non di allegarlo ad altri oggetti. È possibile concedere la possibilità di allegare il modulo personalizzato agli oggetti utilizzando l&#39;opzione &quot;Allega a dati personalizzati&quot; descritta nel passaggio 5.
   >* La maggior parte delle organizzazioni desidera assicurarsi che tutti gli utenti del sistema possano compilare un modulo personalizzato quando è allegato agli oggetti su cui lavorano e visualizzarne i dati nei rapporti. Se questo è vero per la tua organizzazione, ti consigliamo di utilizzare **Rendi visibile a livello di sistema**. Se l&#39;opzione è configurata in questo modo, nella finestra di dialogo viene visualizzato &quot;Visibile a livello di sistema&quot;:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Se sei preoccupato di un modulo personalizzato in cui gli utenti potrebbero immettere dati sensibili quando è allegato a determinati oggetti, limitane la condivisione *oggetti* potrebbe essere preferibile a limitare l’accesso al modulo stesso.

1. Fai clic su **Salva**.

<div class="preview">

## Condividere un modulo personalizzato dal progettista del modulo

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Aprire un modulo personalizzato o crearne uno nuovo.
1. Clic **Condividi** in alto a destra nel progettista del modulo quando si è pronti per la condivisione del modulo.
1. Nella casella visualizzata, sotto **Concedere l’accesso al modulo personalizzato a**, inizia a digitare il nome dell’utente, del team, della mansione, del gruppo o dell’azienda con cui vuoi condividere il modulo personalizzato, quindi premi **Invio** quando viene visualizzato il nome.
1. Per regolare l’accesso per l’utente, il team, la mansione, il gruppo o la società appena aggiunti, fai clic sul menu a discesa a destra del nome, quindi configura una delle seguenti opzioni disponibili e le relative impostazioni avanzate:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizzare</td> 
      <td> <p>Possibilità di visualizzare e compilare il modulo personalizzato sugli oggetti.</p> <p><b>NOTA</b>: per gli utenti con licenze Light e Contributor (o Licenze Lavoro, Revisione e Richiesta), questa è l’opzione più alta disponibile.</p> <p>Clic <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire quanto segue:</p> 
       <ul> 
        <li><strong>Allega a dati personalizzati</strong>: possibilità di allegare il modulo personalizzato a progetti, attività e problemi per i quali dispongono dell’accesso di gestione</li> 
        <li> <p><strong>Condividi</strong>: possibilità di condividere il modulo personalizzato con altri nel sistema</p> <p>Gli utenti con una licenza Light o Contributor (o Licenza Lavoro, Revisione o Richiesta) possono condividere un modulo personalizzato solo tramite l’API o un rapporto di moduli personalizzati.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gestire</td> 
      <td> <p>Disponibile solo per gli utenti con una licenza Standard o Plan. </p> <p>Oltre a poter aggiungere il modulo agli oggetti a cui hanno accesso per la modifica, gli utenti possono anche modificare completamente il modulo personalizzato, incluse le operazioni di aggiunta, modifica ed eliminazione dei campi.</p> <p>Clic <strong>Impostazioni avanzate</strong> per specificare se si desidera consentire quanto segue:</p> 
       <ul> 
        <li> <p><strong>Allega a dati personalizzati</strong>: possibilità di allegare il modulo personalizzato a progetti, attività e problemi per i quali dispongono dell’accesso di gestione</p> </li> 
        <li><strong>Elimina</strong>: elimina il modulo personalizzato dal sistema</li> 
        <li><strong>Condividi</strong>: condividi il modulo personalizzato con altri nel sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Ripeti i passaggi 5-6 per aggiungere altri nomi all’elenco e configurarne le opzioni.
1. (Facoltativo) Se si desidera limitare l&#39;accesso al modulo personalizzato (sugli oggetti a cui è associato) a quelli specificati nei passaggi precedenti, fare clic sulla freccia a discesa sotto **Chi ha accesso**, quindi seleziona **Solo gli invitati possono accedere**.

   Se cambi idea, puoi selezionare **Tutti gli utenti del sistema possono visualizzare**.

   >[!NOTE]
   >
   >* Quando si rende visibile un modulo personalizzato a livello di sistema, è possibile consentire agli utenti di visualizzarlo e compilarlo solo sugli oggetti a cui sono assegnati, non di allegarlo ad altri oggetti. È possibile concedere la possibilità di allegare il modulo personalizzato agli oggetti utilizzando l&#39;opzione &quot;Allega a dati personalizzati&quot; descritta nel passaggio 6.
   >* La maggior parte delle organizzazioni desidera assicurarsi che tutti gli utenti del sistema possano compilare un modulo personalizzato quando è allegato agli oggetti su cui lavorano e visualizzarne i dati nei rapporti. Se questo è vero per la tua organizzazione, ti consigliamo di utilizzare **Tutti gli utenti del sistema possono visualizzare**. Se l&#39;opzione è configurata in questo modo, nella finestra di dialogo viene visualizzato &quot;Visibile a livello di sistema&quot;:
   >   
   >![Condividi modulo personalizzato](assets/share-custom-form-in-designer.png)
   >   
   >Se sei preoccupato di un modulo personalizzato in cui gli utenti potrebbero immettere dati sensibili quando è allegato a determinati oggetti, limitane la condivisione *oggetti* potrebbe essere preferibile a limitare l’accesso al modulo stesso.

1. Fai clic su **Salva**.

</div>

## Rimuovere l’accesso a un modulo personalizzato dall’elenco dei moduli

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Forms personalizzato**.
1. Seleziona il modulo personalizzato, quindi fai clic su ![Icona Condividi](assets/share-icon.png).
1. Nella casella visualizzata fare clic sulla X a destra del nome dell&#39;utente, del team, della mansione, del gruppo o della società a cui non si desidera più avere accesso speciale al modulo.
1. (Facoltativo) Ripeti il passaggio precedente a per altri nomi da rimuovere.
1. Fai clic su **Salva**.
