---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mappatura degli attributi utente e provisioning automatico dei nuovi utenti
description: Utilizzando Single Sign-On (SSO), puoi passare gli attributi da Active Directory del provider di identità agli utenti Adobe Workfront. È inoltre possibile aggiungere nuovi utenti a Workfront utilizzando l’opzione di provisioning automatico (denominata anche Just In Time Provisioning o JIT).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 2%

---

# Mappatura degli attributi utente e provisioning automatico dei nuovi utenti

Utilizzando Single Sign-On (SSO), puoi passare gli attributi da Active Directory del provider di identità agli utenti Adobe Workfront. È inoltre possibile aggiungere nuovi utenti a Workfront utilizzando l’opzione di provisioning automatico (denominata anche Just In Time Provisioning o JIT).

>[!NOTE]
>
>Questa opzione non è disponibile se l’organizzazione è stata caricata in Adobe Admin Console. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.


## Requisiti di accesso

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Suggerimenti per la mappatura degli attributi

Quando mappi gli attributi, tieni presente quanto segue:

* Esegui sempre il test in una sandbox Anteprima o in una sandbox Customer Refresh (CR).
* Esegui il test con gli account amministratore e non amministratore per verificare che gli attributi siano mappati correttamente.
* Gli attributi vengono mappati ogni volta che un utente effettua l’accesso a Workfront tramite SSO, non solo durante il provisioning automatico.

## Mappatura degli attributi utente e provisioning automatico dei nuovi utenti

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Single Sign-On (SSO)**.

1. In **Tipo** a discesa, fai clic su **SAML 2.0**.

1. Fai clic su **Attributi utente mappa**.

   ![](assets/map-user-attributes.png)

1. (Facoltativo) Se si desidera che Workfront crei automaticamente nuovi utenti da Active Directory, fare clic su **Utente con provisioning automatico**.

   Questa funzione richiede la mappatura degli attributi.

1. Nella riga delle opzioni visualizzata, mappa gli attributi necessari per gli utenti Workfront.

   È possibile mappare attributi quali Indirizzo, Manager, Ruolo lavoro, Gruppo principale e così via.

   Le mappature degli attributi funzionano con un rapporto 1:1. Ad esempio, non è possibile impostare ogni gruppo a cui appartiene un utente; è possibile impostarne solo uno per utente.

   >[!IMPORTANT]
   >
   >Per ogni utente sono necessari i seguenti attributi:
   >      
   >* Nome
   >* Cognome
   >* Indirizzo Email

   >      
   >Non è consigliabile mappare i livelli di accesso nelle mappature degli attributi. In questo caso, presta attenzione quando imposti il valore predefinito per assicurarti di non rimuovere accidentalmente Admin Access.

   Nella tabella seguente sono descritti i campi che è possibile utilizzare per mappare gli attributi:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Attributo utente Workfront</td> 
      <td>Scegli il nome dell'attributo che stai mappando</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attributo di directory</td> 
      <td>Digitare l'etichetta dell'attributo SSO che si desidera utilizzare./td&gt; 
     </tr> 
     <tr> 
      <td role="rowheader">Valore predefinito</td> 
      <td> <p>Dopo aver scelto un attributo utente Workfront, se il valore è NULL durante la connessione, questo campo si riempie con il valore predefinito corrispondente nel sistema. Digita un valore qui solo se intendi applicare le regole di mappatura attributi (vedi il passaggio 7). Il valore predefinito funge da eccezione per tali regole.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facoltativo) Fai clic su **Regole** per aggiungere una regola all&#39;attributo.

   1. Nel menu a discesa, scegli il modificatore di attributo che desideri utilizzare.
   1. Nei 2 campi a destra, digita il valore dell’attributo di directory e il valore con cui desideri sostituirlo.

      ![](assets/rule-fields.png)
   Puoi fare clic su **Aggiungi regola** per aggiungere più regole all&#39;attributo .

1. (Facoltativo) Per mappare altri attributi utente, fai clic su **Aggiungi mappatura** e ripetere i punti 6-7.
1. Fai clic su **Salva**.
