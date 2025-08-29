---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Impostare i tassi di cambio
description: I tassi di cambio influiscono su tutti gli elementi finanziari di Workfront. La valuta di base è la valuta predefinita per tutti i progetti nel sistema.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc820b4012fec494ce5ebb1baefb4ee0df214916
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 2%

---

# Impostare i tassi di cambio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

In qualità di amministratore di Adobe Workfront, puoi impostare i tassi di cambio in Workfront. Ciò include quanto segue:

* Impostazione della valuta predefinita per il sistema Workfront
* Aggiornamento dei tassi di cambio in Workfront per far corrispondere i tassi di cambio correnti
* La configurazione dei tassi di cambio per più valute (consentendo agli utenti di scegliere una valuta predefinita per i singoli progetti)

I tassi di cambio influiscono su tutti gli elementi finanziari di Workfront. La valuta di base è la valuta predefinita per tutti i progetti nel sistema, a meno che non venga sostituita per un determinato progetto o mansione. La valuta di base o predefinita corrente è indicata dall&#39;icona ![icona valuta predefinita](assets/default-icon.png) nell&#39;elenco. È inoltre possibile scegliere di visualizzare le informazioni finanziarie in valute disponibili nel sistema diverse dalla valuta di base o da quella del progetto quando vengono visualizzate in un report o in un elenco. Per ulteriori informazioni, vedere [Creare report di dati finanziari con tassi di cambio univoci](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Per ulteriori informazioni sull’override della valuta di base in Workfront per progetti e ruoli, vedi i seguenti articoli:

* [Cambia la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

La modalità di impostazione dei tassi di cambio influisce sulla possibilità degli utenti di modificare i tassi di cambio per un determinato progetto.

>[!IMPORTANT]
>
>I tassi di cambio in Workfront non sono dinamici; il valore impostato deve essere aggiornato quando si verificano modifiche nei tassi di cambio.

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

## Impostare i tassi di cambio

{{step-1-to-setup}}

1. Fai clic su **Preferenze progetto** > **Tassi di cambio**.

1. Fare clic su **Aggiungi valuta**.
1. Nella casella **Aggiungi valuta**, iniziare a digitare il nome della valuta, quindi fare clic su di essa quando viene visualizzata nell&#39;elenco a discesa.
1. Nel campo **Tasso di cambio** immettere il tasso per la valuta selezionata, confrontato con la valuta impostata come valuta di base nel sistema.
1. Fai clic su **Aggiungi** per aggiungere la nuova valuta e il relativo tasso di cambio.
1. (Facoltativo) Per modificare la valuta di base (predefinita), effettuare una delle seguenti operazioni:

   * Selezionare la casella di controllo accanto al nome della valuta e selezionare **Rendi predefinito** nella barra delle azioni nella parte inferiore dello schermo.
   * Passa il puntatore del mouse sul nome della valuta e fai clic sul menu **Altro** visualizzato. Quindi, selezionare **Rendi predefinito**.

     La nuova valuta predefinita viene aggiornata con l’icona.

     >[!NOTE]
     >
     >La valuta predefinita viene sempre visualizzata per prima nell&#39;elenco, indipendentemente dall&#39;ordinamento dell&#39;elenco.

1. (Facoltativo) Per eliminare una valuta, seleziona la casella di controllo accanto al nome della valuta e seleziona **Elimina** nella barra delle azioni nella parte inferiore della schermata. Impossibile eliminare la valuta predefinita.

## Consenti agli utenti di modificare la valuta predefinita per un progetto

Gli utenti possono modificare la valuta predefinita per un progetto quando sono soddisfatte le seguenti condizioni:

* L&#39;utente dispone di una licenza Standard o Plan con accesso amministrativo ai tassi di cambio.

  Per ulteriori informazioni, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Nel sistema Workfront è abilitata più di una valuta.

Per informazioni su come gli utenti possono modificare la valuta predefinita in un determinato progetto, vedere [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Consenti agli utenti di modificare la valuta predefinita per una mansione

Gli utenti possono modificare la valuta per una mansione quando sono soddisfatte le seguenti condizioni:

* L’utente dispone di una licenza Standard o Full con accesso amministrativo ai Ruoli.

  Per ulteriori informazioni, vedere [Concedere agli utenti l&#39;accesso amministrativo ad alcune aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Nel sistema Workfront è abilitata più di una valuta.

Per informazioni su come gli utenti possono modificare la valuta predefinita per una determinata mansione, vedere [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).


<!--The default currency is the currency that is used as the default for all projects and reports throughout the system. The current default is indicated with an icon ![Default currency icon](assets/default-icon.png).-->
