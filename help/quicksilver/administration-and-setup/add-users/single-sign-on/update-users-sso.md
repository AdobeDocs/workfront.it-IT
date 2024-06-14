---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Aggiornare gli utenti per il Single Sign-On
description: È possibile aggiornare gli utenti per il Single Sign-On in Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 1%

---

# Aggiornare gli utenti per il Single Sign-On

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

Quando l&#39;accesso Single Sign-On (SSO) è abilitato nell&#39;istanza Adobe Workfront, gli utenti possono accedere a Workfront con le credenziali SSO.

Se disponi di un sistema esistente già popolato con utenti associati a credenziali SSO, puoi importare gli ID degli utenti in Workfront importando un file con valori delimitati da virgole (CSV) in Workfront.

Per ulteriori informazioni sull&#39;integrazione di Workfront con un sistema SSO, vedere [Panoramica del single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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
   <td> <p>Devi essere un amministratore di Workfront.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Nomi utenti SSO

A seconda della soluzione SSO utilizzata, il nome utente nell’ambiente SSO può essere chiamato in uno dei seguenti modi:

* Nome utente SSO
* ID federazione
* Nome utente federazione

Indipendentemente dalla chiamata del nome utente nell&#39;ambiente SSO, il valore del campo viene memorizzato nel campo Nome utente SSO dell&#39;oggetto Utente.

Affinché gli utenti possano utilizzare le credenziali SSO per accedere a Workfront, è necessario aggiornare il profilo in modo che includa il nome utente SSO, oltre al nome utente Workfront.

In qualità di amministratore di Workfront, puoi aggiornare in blocco il campo Nome utente SSO per gli utenti di Workfront importando un elenco di nomi utente in Workfront. Tale elenco deve:

* Contengono il GUID (Workfront User ID) e il nome utente SSO corrispondente per ogni utente
* Essere salvato come file CSV o TSV.

Questo processo aggiorna i nomi utente SSO esistenti in Workfront oppure, se ne manca uno per gli utenti, ne aggiunge uno nuovo.

## Preparare il file di importazione {#prepare-the-import-file}

È possibile iniziare a preparare il file di importazione creando un report di tutti gli utenti in Workfront che devono avere i campi Nome utente SSO aggiornati.

1. Creare un rapporto utente in Workfront.

   Per istruzioni sulla creazione di report utente in Workfront, consulta [Creare un rapporto personalizzato](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Seleziona i campi seguenti nel rapporto:

   | Campo | Spiegazione |
   |---|---|
   | Nome | Il nome completo dell’utente di Workfront. |
   | ID | L&#39;ID è il GUID alfanumerico di Workfront. |
   | Nome utente SSO | Aggiunta del campo Nome utente SSO per garantire che non siano presenti nomi utente sovrascritti con l&#39;importazione. Questo campo deve essere vuoto per tutti gli utenti, se gli utenti non sono ancora stati aggiornati per l&#39;SSO. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Salva il rapporto.
1. Clic **Esporta** nella parte superiore del rapporto ed esportarlo in Excel.
1. Aprire il file Excel esportato e aggiungere i nomi utente SSO per ogni utente nel report nella colonna Nome utente SSO.

   >[!IMPORTANT]
   >
   >I nomi utente SSO fanno distinzione tra maiuscole e minuscole.

1. Elimina tutte le colonne nel file di Excel, ad eccezione di **ID** e **Nome utente SSO** colonne.

1. Elimina le intestazioni di colonna e accertati che non vi siano righe vuote nella parte superiore del rapporto.

   Il file che stai utilizzando per aggiornare gli utenti di Workfront con i nomi utente SSO **deve** contiene solo 2 colonne, nell’ordine seguente:

   * Nella prima colonna deve essere visualizzato l&#39;ID utente di Workfront (il GUID utente trovato in Workfront).
   * La seconda colonna deve contenere il nome utente SSO visualizzato nel sistema SSO.
   * Le colonne non devono avere intestazioni e non devono essere presenti righe vuote nella parte superiore dell’elenco dei nomi.

     ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Salva il rapporto come file CSV o TSV sul computer.

## Aggiornare gli utenti per l&#39;SSO {#update-your-users-for-sso}

Il processo di aggiornamento degli utenti per l&#39;SSO aggiunge il campo Nome utente SSO agli utenti di Workfront, se non ne è presente uno, oppure aggiorna il valore in tale campo se è già presente un valore associato agli utenti.

1. Fai clic su **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, oppure (se disponibile) fai clic sul pulsante **[!UICONTROL Menu principale]** icona ![Menu principale](/help/_includes/assets/main-menu-icon-left-nav.png) nell’angolo superiore sinistro, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su, **Sistema** quindi seleziona **Aggiorna utenti per l&#39;SSO**.

1. Clic **Scegli file** per cercare il file preparato.

   Per ulteriori informazioni su come preparare questo file, vedi [Preparare il file di importazione](#prepare-the-import-file).

1. Selezionare il file da cui è stato salvato nel computer, quindi fare clic su **Apri**.

   In questo modo vengono inserite le credenziali SSO in Workfront, consentendo a tutti gli utenti di accedere a Workfront utilizzando le proprie credenziali SSO.

   Il **Consenti solo `<SSO Configuration>` Autenticazione** è attivata per tutti gli utenti inclusi nel file CSV. In questo modo gli utenti devono effettuare l&#39;accesso tramite SSO.

## Verifica l&#39;SSO in base ai nomi utente Workfront degli utenti

Per istruzioni sulla creazione di un report utente contenente informazioni sul nome utente SSO, vedere [Preparare il file di importazione](#prepare-the-import-file).

1. Eseguire un report utente contenente informazioni sul nome utente SSO.

   La colonna Nome utente SSO viene compilata per ogni utente.

1. Verificare che i valori della colonna Nome utente SSO corrispondano al nome utente SSO nel server SSO.
1. Se la colonna Nome utente SSO è vuota, aggiorna i nomi utente SSO degli utenti.

   ![](assets/users-with-sso-field-updated.png)

   Per istruzioni sull&#39;aggiornamento degli utenti per l&#39;accesso SSO, vedere [Aggiornare gli utenti per l&#39;SSO](#update-your-users-for-sso).
