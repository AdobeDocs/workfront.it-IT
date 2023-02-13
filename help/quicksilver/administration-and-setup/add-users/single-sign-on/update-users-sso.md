---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Aggiornare gli utenti per il single sign-on
description: È possibile aggiornare gli utenti per il single sign-on in Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# Aggiornare gli utenti per il single sign-on

{{important-admin-console-onboard}}

Quando l&#39;accesso single sign-on (SSO) è abilitato nell&#39;istanza Adobe Workfront, puoi accedere a Workfront con le tue credenziali SSO.

Se disponi di un sistema esistente già popolato con utenti associati a credenziali SSO, puoi importare gli ID degli utenti in Workfront importando un file di valori delimitati da virgole (CSV) in Workfront.

Per ulteriori informazioni sull&#39;integrazione di Workfront con un sistema SSO, vedi [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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

## Nomi utente SSO

A seconda della soluzione SSO utilizzata, il nome utente nel tuo ambiente SSO può essere chiamato uno dei seguenti:

* Nome utente SSO
* ID federazione
* Nome utente federativo

In Workfront, tutti questi nomi sono memorizzati nel campo Username SSO, sull&#39;oggetto utente.

Affinché i tuoi utenti possano utilizzare le loro credenziali SSO per accedere a Workfront, devi aggiornare il loro profilo per includere il loro nome utente SSO, oltre al loro nome utente Workfront.

In qualità di amministratore di Workfront, è possibile aggiornare in massa il campo Nome utente SSO per gli utenti Workfront utilizzando un elenco di nomi utente e importandolo in Workfront. Questo elenco deve contenere l’ID utente Workfront (GUID) e il nome utente SSO corrispondente per ciascun utente e deve essere salvato come file CSV o TSV. Questo processo aggiorna i nomi utente SSO esistenti in Workfront oppure aggiunge un nuovo nome utente SSO, se manca uno per gli utenti.

## Preparare il file di importazione {#prepare-the-import-file}

Puoi iniziare a preparare il file di importazione creando un rapporto di tutti gli utenti in Workfront che deve avere i campi del nome utente SSO aggiornati.

1. Crea un rapporto utente in Workfront.

   Per istruzioni su come creare rapporti sugli utenti in Workfront, vedi [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Seleziona i campi seguenti nel rapporto:

   | Nome | Nome completo dell’utente Workfront. |
   |---|---|
   | ID | L&#39;ID è il GUID alfanumerico Workfront. |
   | Nome utente SSO | Seleziona il campo Nome utente SSO per assicurarti che non ci siano nomi utente che stai sovrascrivendo con l&#39;importazione. Questo campo deve essere vuoto per tutti gli utenti, se gli utenti non sono ancora stati aggiornati per SSO. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Salva il rapporto.
1. Fai clic su **Esporta** nella parte superiore del rapporto ed esporta il rapporto in Excel.
1. Apri il file Excel esportato e inizia ad aggiungere i tuoi nomi utente SSO per ogni utente nel report nella colonna Nome utente SSO.

   >[!IMPORTANT]
   >
   >I nomi utente SSO sono sensibili all&#39;uso di maiuscole e minuscole.

1. Elimina tutte le colonne del file Excel, ad eccezione del **ID** e **Nome utente SSO** colonne.

1. Elimina le intestazioni di colonna e assicurati che non ci siano righe vuote nella parte superiore del rapporto.

   Il file utilizzato per aggiornare gli utenti Workfront con i nomi utente SSO deve contenere solo 2 colonne, in questo ordine:

   * Nella prima colonna deve essere visualizzato l’ID utente di Workfront (il GUID utente trovato in Workfront).
   * La seconda colonna deve contenere il nome utente SSO, così come viene visualizzato nel sistema SSO.
   * Le colonne non devono avere intestazioni e non devono essere presenti righe vuote nella parte superiore dell’elenco dei nomi.

      ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Salva il rapporto come file CSV o TSV sul tuo computer.

## Aggiorna gli utenti per SSO {#update-your-users-for-sso}

Il processo di aggiornamento degli utenti per SSO aggiunge il campo Username SSO agli utenti Workfront se non è presente, oppure aggiorna il valore in quel campo se esiste già un valore associato agli utenti.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** then **Aggiorna utenti per SSO**.

1. Fai clic su **Scegli file** per cercare il file preparato.

   Per ulteriori informazioni su come preparare questo file, vedi [Preparare il file di importazione](#prepare-the-import-file).

1. Selezionare il file in cui è salvato sul computer, quindi fare clic su **Apri**.

   Questo consente a tutti gli utenti di accedere a Workfront utilizzando le proprie credenziali SSO.

   La **Consenti solo `<SSO Configuration>` Autenticazione** è abilitata per tutti gli utenti inclusi nel CSV.

## Verifica SSO i nomi utente Workfront degli utenti

Per istruzioni su come creare un report utente contenente informazioni sul nome utente SSO, vedi [Preparare il file di importazione](#prepare-the-import-file).

1. Esegui un rapporto utente contenente informazioni sul nome utente SSO.

   La colonna Nome utente SSO viene compilata per ogni utente.

1. Assicurati che i valori della colonna Nome utente SSO corrispondano al nome utente SSO sul server SSO.
1. Se la colonna Nome utente SSO è vuota, aggiorna i nomi utente SSO degli utenti.

   ![](assets/users-with-sso-field-updated.png)

   Per istruzioni su come aggiornare gli utenti per SSO, vedi [Aggiorna gli utenti per SSO](#update-your-users-for-sso).
