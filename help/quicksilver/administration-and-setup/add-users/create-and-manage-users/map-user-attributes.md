---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mappa attributi utente
description: Utilizzando il Single Sign-On (SSO), è possibile passare gli attributi da Active Directory del provider di identità agli utenti di Adobe Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 1%

---

# Mappare gli attributi utente

<!--Audited 2/2024-->

Utilizzando il Single Sign-On (SSO), è possibile passare gli attributi da Active Directory del provider di identità agli utenti di Adobe Workfront.

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
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Nuovo: Standard</p><p>Oppure</p><p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td>
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Suggerimenti per la mappatura degli attributi

Quando mappate gli attributi, tenete presente quanto segue:

* Esegui sempre il test in una sandbox di anteprima o di aggiornamento cliente (CR).
* Eseguire il test con gli account amministratore e non amministratore per verificare che gli attributi vengano mappati correttamente.
* Gli attributi mappati vengono applicati ogni volta che un utente accede tramite single sign-on.

  Esempio: se mappi &quot;cognome&quot; e aggiorni il loro nome in Workfront senza aggiornare il valore nel loro provider di identità, il cognome verrà sovrascritto in modo che corrisponda al valore di qualsiasi elemento presente nel provider di identità alla successiva connessione dell’utente.

## Mappare gli attributi utente per la tua organizzazione

La procedura per la mappatura degli attributi varia a seconda che l’organizzazione sia o meno nell’esperienza unificata di Adobe.

Per determinare se l’organizzazione si trova nell’esperienza unificata di Adobe, esamina l’URL utilizzato per accedere a Workfront.

| URL | Esperienza Adobe |
|---|---|
| (NomeSocietà).my.workfront.com | Esperienza classica |
| experience.adobe.com | Adobe di esperienza unificata |

* [Mappatura degli attributi utente nell’esperienza classica](#map-user-attributes-in-the-classic-experience)
* [Mappare gli attributi utente nell’esperienza unificata di Adobe](#map-user-attributes-in-the-adobe-unified-experience)

### Mappatura degli attributi utente nell’esperienza classica

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fare clic su **Sistema** > **Single Sign-On (SSO)**.

1. Nel menu a discesa **Tipo**, fare clic su **SAML 2.0**.

1. Fare clic su **Mappa attributi utente**.

   ![](assets/map-user-attributes.png)

1. Nella riga di opzioni visualizzata, mappa gli attributi necessari per gli utenti di Workfront.

   Puoi mappare attributi come Indirizzo, Manager, Ruolo, Gruppo predefinito e così via.

   Le mappature degli attributi funzionano con un rapporto 1:1. Ad esempio, non è possibile impostare ogni gruppo a cui appartiene un utente, ma solo uno per utente.

   >[!IMPORTANT]
   >
   >È sconsigliato mappare i livelli di accesso nelle mappature degli attributi. In tal caso, presta attenzione quando imposti il valore predefinito per evitare di rimuovere inavvertitamente Admin Access.

   Nella tabella seguente vengono illustrati i campi che è possibile utilizzare per mappare gli attributi:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Attributo utente Workfront</td> 
      <td>Scegli il nome dell'attributo di cui stai eseguendo la mappatura</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attributo di directory</td> 
      <td>Digitare l'etichetta dell'attributo SSO che si desidera utilizzare.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Valore predefinito</td> 
      <td> <p>Dopo aver scelto un attributo utente di Workfront, se il valore è NULL durante la connessione, questo campo viene compilato con il valore predefinito corrispondente nel sistema. Digita un valore qui solo se intendi applicare le regole di mappatura attributi (vedi passaggio 7). Il valore predefinito funge da eccezione a tali regole.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Fai clic su **Regole** per aggiungere una regola all&#39;attributo.

   1. Nell’elenco a discesa, scegli il modificatore di attributo che desideri utilizzare.
   1. Nei 2 campi a destra, digita il valore dell’attributo della directory e il valore con cui desideri sostituirlo.

      ![](assets/rule-fields.png)

   Puoi fare clic su **Aggiungi regola** per aggiungere altre regole all&#39;attributo.

1. (Facoltativo) Per mappare altri attributi utente, fare clic su **Aggiungi mappatura** e ripetere i passaggi 6-7.
1. Fai clic su **Salva**.

### Mappare gli attributi utente nell’esperienza unificata di Adobe

1. Fai clic sull&#39;icona ![](assets/main-menu-left.png) del **menu principale** nell&#39;angolo superiore sinistro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fare clic su **Sistema** > **Single Sign-On (SSO)**.

1. Selezionare la scheda **Adobe**.

1. (Facoltativo e condizionale) Se nell&#39;esperienza classica è stata configurata la mappatura degli attributi per la tua organizzazione e desideri copiarla nell&#39;esperienza unificata di Adobe, fai clic su **Migra mappature**. Puoi quindi eliminare, eliminare o modificare queste mappature.

   >[!NOTE]
   >
   >È consigliabile eseguire la migrazione delle mappature la prima volta che le si configura nell’esperienza unificata di Adobe. Non c&#39;è alcun danno nel migrarli di nuovo in un secondo momento, ma migrarli più di una volta non è necessario.

1. Per creare un nuovo mapping di attributi, fare clic su **Aggiungi mapping**.

1. Fare clic sulla freccia accanto al nome del campo Workfront e selezionare il campo [!DNL Workfront] che si desidera mappare.

1. (Facoltativo) Se si desidera creare più regole per un determinato campo, fare clic sulla freccia accanto a **Sempre** e selezionare l&#39;operatore che si desidera utilizzare per la regola.

1. (Condizionale) Se hai selezionato un operatore oltre a Sempre, seleziona il campo Workfront e il valore a cui si applica l’operatore.

   >[!NOTE]
   >
   >Gli operatori `Is Truthy` e `Is Falsy` non richiedono valori.

1. Seleziona se desideri applicare il valore di un attributo nel gestore identità al campo Workfront o se desideri applicare un valore costante specifico.

1. Immettere il nome del campo Identity Manager che si desidera applicare oppure immettere il testo del valore costante che si desidera applicare.

1. (Facoltativo) Per aggiungere altre regole per lo stesso campo Workfront, fai clic su **Aggiungi nuova regola** e segui i passaggi 4-9.

   >[!IMPORTANT]
   >
   > * Qualsiasi regola al di sotto di una regola Always verrà ignorata. Se si dispone di una regola Always, è necessario spostarla in fondo all&#39;elenco delle regole. Per spostare le regole nell’elenco, fai clic sul menu a tre punti a destra della regola e spostale verso l’alto o verso il basso.
   > * Per creare una regola al centro dell&#39;elenco, fai clic sul menu a tre punti accanto alla regola che desideri posizionare al di sopra o al di sotto della nuova regola e seleziona **Aggiungi regola al di sopra di** o **Aggiungi regola al di sotto di**.

1. Per eliminare una regola, fare clic sul menu a tre punti accanto alla regola che si desidera eliminare e selezionare **Elimina**.
1. Per eliminare una mappatura, fai clic sull&#39;icona **Elimina** presente nella scheda della mappatura.

1. Per salvare, scorri fino alla parte superiore della pagina e fai clic su **Salva**.


