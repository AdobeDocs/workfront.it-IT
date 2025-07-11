---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gestisci i Tipi di Ora
description: È possibile associare i tipi di ore alle ore inserite. I tipi di ore sono etichette utilizzate per definire le ore inserite.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 4fafdcea97874e791104260375617e3989af1870
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# Gestire tipi di ora

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>
-->

I tipi di ore sono etichette utilizzate per definire le ore inserite. È possibile associare i tipi di ore alle ore inserite.

Esistono due categorie di tipi di ore:

* **Tipi di lavoro specifici per il progetto**: tempo impiegato per l&#39;accesso a progetti, attività e problemi. I tipi di lavoro specifici del progetto possono essere associati alle ore inserite in qualsiasi punto di [!DNL Adobe Workfront], dove è possibile registrare il tempo per progetti, attività e problemi.

  Quando si registra l&#39;ora in [!DNL Workfront], i tipi di ora specifici del progetto disponibili dipendono dalle opzioni di configurazione impostate a livello di sistema, progetto e utente.

  Sono sempre disponibili i seguenti tipi di lavoro predefiniti specifici per il progetto:

   * Ore di Progetto
   * Ore di Attività
   * Tempo del problema

  L&#39;amministratore [!DNL Workfront] determina quali tipi di ore specifiche del progetto sono rese disponibili, come descritto in [Definire i tipi di ore e la disponibilità](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Se si abilita qualsiasi tipo di ora specifico del progetto nel sistema [!DNL Workfront], è necessario abilitare almeno un tipo di ora specifico del progetto in ogni progetto del sistema. Non è possibile abilitare un tipo di ora specifico per il progetto a livello di sistema e non sono disponibili tipi di ora specifici per il progetto a livello di progetto.

* **Tipi di lavoro generali**: le ore generali non possono essere associate a un progetto, un&#39;attività o un problema e vengono registrate direttamente in una scheda orario.

Per informazioni sulle ore di registrazione e sulla loro associazione ai tipi di ore, vedere [Tempo di registrazione](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Nuovo: Standard</p>
   <p>Oppure</p>
   <p>Corrente: Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Livello di accesso</td> 
   <td>Amministratore di Sistema</td>
  </tr> 
 </tbody> 
</table>

*Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipi di lavoro incorporati

Workfront viene fornito con un set di tipi di ora incorporati. Questi tipi di lavoro non possono essere modificati o nascosti.

I tipi di ore forniti con [!DNL Workfront] sono:

* **[!UICONTROL Malattia]**: tipo di ora generale che non può essere associato alle ore inserite in un progetto, attività o problema. Le ore di malattia non possono essere conteggiate come ricavi.
* **[!UICONTROL Ferie]**: tipo di ora generale che non può essere associato alle ore inserite in un progetto, attività o problema. Il tempo di vacanza non può essere conteggiato come reddito.
* **[!UICONTROL Costi comuni generali]**: un tipo di ora generale che non può essere associato alle ore inserite in un progetto, attività o problema. Può essere conteggiato come ricavo nel processo di pianificazione del progetto.
* **[!UICONTROL Ora progetto]**: tipo di ora generale che può essere associato solo alle ore inserite in un progetto.
* **[!UICONTROL Ora attività]**: tipo di ora generale che può essere associato solo alle ore inserite in un&#39;attività.
* **[!UICONTROL Ora problema]**: tipo di ora generale che può essere associato solo alle ore inserite in un problema.

## Crea tipi di lavoro

In qualità di amministratore [!DNL Workfront], puoi creare tipi di lavoro per la tua organizzazione a livello di sistema e di progetto.

Dopo aver definito i tipi di ore a livello di sistema, gli utenti possono definire quali tipi di ore sono disponibili per progetti specifici o per utenti specifici.

Per ulteriori informazioni, vedere [Definire i tipi di ore e la disponibilità](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Per creare i tipi di lavoro:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Scheda orario e ore**, quindi fai clic su **Tipi di ore**.

1. Nella sezione **Tipi di lavoro** fare clic su **Nuovo tipo di lavoro**.
1. Nella finestra di dialogo **Nuovi tipi di lavoro** specificare le informazioni seguenti:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Immettere un nome di tipo di ora facilmente riconoscibile nel sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrizione]</td> 
      <td>Aggiungi una descrizione per il tipo di ora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ambito]</td> 
      <td> <p>Nel menu a discesa <strong>Ambito</strong>, selezionare se il tipo di ora è generale o specifico del progetto.</p> <p>I tipi di lavoro generali sono visibili solo nelle schede orario e non possono essere associati a progetti, attività o problemi.</p> <p><b>IMPORTANTE</b>: se si dispone di un Tipo di Ora personalizzato che è [!UICONTROL Specifico per Progetto] e si modifica tale tipo in [!UICONTROL Generale], tutte le attività, i problemi e le ore di Progetto esistenti vengono impostate sui relativi tipi predefiniti di sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count As Revenue]</td> 
      <td><p>Selezionare questa opzione se si desidera che la voce relativa alle ore associata a questo tipo di ore influisca sui calcoli dei ricavi.</p>
      <p>Il tempo di malattia e il tempo di vacanza non possono essere conteggiati come ricavi.</p>
      <p><b>NOTA</b></p>
      <p>Quando i tipi di ore generali vengono conteggiati come ricavi, la tariffa di costo associata al profilo dell’utente che registra l’ora viene associata al costo orario.  
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **[!UICONTROL Crea tipo di lavoro].**

   Il tipo di ora viene aggiunto al sistema Workfront e attivato per impostazione predefinita.

## Disattiva i tipi di lavoro

È possibile disattivare i tipi di ore se non si desidera più che gli utenti associno le loro ore. Quando si disattivano i tipi di ore, questi vengono nascosti da qualsiasi punto di [!DNL Workfront] in cui i tipi di ore sono visibili.

>[!NOTE]
>
>* Non è possibile disattivare i tipi di lavoro incorporati.
>* Quando disattivi un Tipo di ora specifico per il progetto, per tutto il tempo registrato per quel tipo viene automaticamente utilizzato il tipo di ora predefinito del progetto. Ad esempio, il tempo registrato per un progetto viene impostato automaticamente sul tipo Ora progetto; il tempo registrato per un&#39;attività viene impostato automaticamente sul tipo Ora attività.
>


Per disattivare un tipo di ora:

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **[!UICONTROL Scheda orario e ore]**, quindi fai clic su **[!UICONTROL Tipi di ore]**.

1. Selezionare il tipo di ora che si desidera disattivare.


1. Fai clic su **Altro**, quindi su **Disattiva**.

   ![Attiva e disattiva collegamenti di tipo ora](assets/activate-and-deactivate-hour-type-links.png)

   Il tipo di ora è disattivato e gli utenti non possono più trovarlo durante la registrazione delle ore.

1. (Facoltativo) Per riattivare un tipo di ora, selezionalo nell&#39;elenco **Tipi di ora**, quindi fai clic su **Altro** > **Attiva**.

