---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Imposta tassi di cambio
description: In qualità di amministratore di Adobe Workfront, puoi impostare i tassi di cambio in Workfront.
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: b0cf0a5ec6b932267c8714b966638d8da93331b8
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Imposta tassi di cambio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

In qualità di amministratore di Adobe Workfront, puoi impostare i tassi di cambio in Workfront. Ciò include quanto segue:

* Impostazione della valuta predefinita per il sistema Workfront
* Aggiornamento dei tassi di cambio in Workfront per far corrispondere i tassi di cambio correnti
* La configurazione dei tassi di cambio per più valute (consentendo agli utenti di scegliere una valuta predefinita per i singoli progetti)

I tassi di cambio influiscono su tutti gli elementi finanziari di Workfront. La valuta di base è la valuta predefinita per tutti i progetti nel sistema, a meno che non venga sostituita per un determinato progetto o mansione. È inoltre possibile scegliere di visualizzare le informazioni finanziarie in valute disponibili nel sistema diverse dalla valuta di base o da quella del progetto quando vengono visualizzate in un report o in un elenco. Per ulteriori informazioni, consulta [Creazione di report di dati finanziari con tassi di cambio univoci](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Per ulteriori informazioni sull&#39;override della valuta di base in Workfront per i progetti e le mansioni, vedere gli articoli seguenti:

* [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

La modalità di impostazione dei tassi di cambio influisce sulla possibilità degli utenti di modificare i tassi di cambio per un determinato progetto.

>[!IMPORTANT]
>
>I tassi di cambio in Workfront non sono dinamici; il valore impostato deve essere aggiornato quando si verificano modifiche nei tassi di cambio.

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
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Imposta tassi di cambio

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Preferenze progetto** > **Tassi di cambio.**

1. Clic **Aggiungi valuta.**
1. Inizia a digitare il nome della valuta, quindi fai clic su di essa quando viene visualizzato nell’elenco a discesa.

1. Nel campo fornito, specifica il tasso per la valuta selezionata, in quanto si riferisce alla valuta impostata come valuta di base nel sistema.
1. (Facoltativo) Imposta la valuta come valuta di base (predefinita) per Workfront.

   Questa è la valuta utilizzata come predefinita per tutti i progetti e i report in tutto il sistema.

1. Clic **Salva** per salvare le modifiche.

## Consenti agli utenti di modificare la valuta predefinita per un progetto

Gli utenti possono modificare la valuta predefinita per un progetto quando sono soddisfatte le seguenti condizioni:

* L&#39;utente dispone di una licenza Pianificazione con accesso amministrativo a Tassi di cambio.

  Per ulteriori informazioni, consulta [Concedere agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Nel sistema Workfront è abilitata più di una valuta.

Per informazioni su come gli utenti possono modificare la valuta predefinita in un dato progetto, vedi [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Consenti agli utenti di modificare la valuta predefinita per una mansione

Gli utenti possono modificare la valuta per una mansione quando sono soddisfatte le seguenti condizioni:

* L’utente dispone di una licenza Pianificazione con accesso amministrativo ai Ruoli.

  Per ulteriori informazioni, consulta [Concedere agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Nel sistema Workfront è abilitata più di una valuta.

Per informazioni su come gli utenti possono modificare la valuta predefinita per una determinata mansione, vedi [Creare e gestire le mansioni](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
