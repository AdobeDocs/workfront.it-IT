---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: In qualità di amministratore di Adobe Workfront, puoi impostare i tassi di cambio in Workfront.
description: Imposta i tassi di cambio
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Imposta i tassi di cambio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

In qualità di amministratore di Adobe Workfront, puoi impostare i tassi di cambio in Workfront. Ciò include i seguenti elementi:

* Impostazione della valuta predefinita per il sistema Workfront
* Aggiornamento dei tassi di cambio in Workfront in modo che corrispondano ai tassi di cambio correnti
* Configurazione dei tassi di cambio per più valute (in questo modo gli utenti possono scegliere una valuta predefinita per i singoli progetti)

I tassi di cambio influiscono su tutti gli elementi finanziari in Workfront. La valuta di base è la valuta predefinita per tutti i progetti in tutto il sistema, a meno che non venga sostituita per un determinato progetto o ruolo di lavoro. È inoltre possibile scegliere di visualizzare le informazioni finanziarie nelle valute disponibili nel sistema che sono diverse dalla valuta di base o da quella del progetto quando vengono visualizzate in un report o in un elenco. Per ulteriori informazioni, consulta [Creare rapporti di dati finanziari con tassi di cambio univoci](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Per ulteriori informazioni sull&#39;override della valuta di base in Workfront per progetti e ruoli di lavoro, vedere i seguenti articoli:

* [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

Il modo in cui si impostano i tassi di cambio influisce sulla possibilità per gli utenti di modificare i tassi di cambio di un determinato progetto.

>[!IMPORTANT]
>
>I tassi di cambio in Workfront non sono dinamici; il valore impostato deve essere aggiornato quando si verificano variazioni dei tassi di cambio.

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

## Imposta i tassi di cambio

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Preferenze del progetto** > **Tassi di cambio**

1. Fai clic su **Aggiungi valuta.**
1. Inizia a digitare il nome della valuta, quindi fai clic su di essa quando viene visualizzata nell’elenco a discesa.

1. Nel campo fornito specificare il tasso per la valuta selezionata, in quanto si riferisce alla valuta impostata come valuta di base nel sistema.
1. (Facoltativo) Imposta la valuta come valuta di base (predefinita) per Workfront.

   Si tratta della valuta utilizzata come impostazione predefinita per tutti i progetti e i rapporti in tutto il sistema.

1. Fai clic su **Salva** per salvare le modifiche.

## Consenti agli utenti di modificare la valuta predefinita di un progetto

Gli utenti possono modificare la valuta predefinita di un progetto quando sono soddisfatte le seguenti condizioni:

* L&#39;utente dispone di una licenza Plan con accesso amministrativo a Exchange Rates.

   Per ulteriori informazioni, consulta [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Sul sistema Workfront è abilitata più di una valuta.

Per informazioni su come gli utenti possono modificare la valuta predefinita di un determinato progetto, consulta [Modificare la valuta del progetto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Consenti agli utenti di modificare la valuta predefinita per un ruolo di lavoro

Gli utenti possono modificare la valuta per un ruolo di lavoro quando sono soddisfatte le seguenti condizioni:

* L&#39;utente dispone di una licenza Plan con accesso amministrativo a Ruoli processo.

   Per ulteriori informazioni, consulta [Consentire agli utenti l&#39;accesso amministrativo a determinate aree](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Nel sistema Workfront è abilitata più di una valuta.

Per informazioni su come gli utenti possono modificare la valuta predefinita in un determinato ruolo di lavoro, vedere [Creare e gestire ruoli di lavoro](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
