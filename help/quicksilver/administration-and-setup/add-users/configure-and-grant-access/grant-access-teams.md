---
title: Concedere l’accesso ai team
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai team in Workfront
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 5%

---

# Concedere l’accesso ai team

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l&#39;accesso di un utente ai team in Workfront, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurare l’accesso degli utenti per la modifica degli utenti utilizzando un livello di accesso personalizzato

1. Iniziare a creare o modificare il livello di accesso, come descritto in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull&#39;icona ingranaggio ![](assets/gear-icon-settings.png) sul pulsante **Visualizza** o **Modifica** a destra di Team, quindi seleziona le abilità che desideri concedere in **Ottimizza le impostazioni**.

   * **Visualizza**: se stai configurando il modo in cui gli utenti con una licenza possono visualizzare i team, modifica una delle seguenti opzioni:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Visualizza i team associati ai miei gruppi</td>
         <td>
          <p><b>Abilitato</b>: quando gli utenti cercano i team in un campo di completamento automatico Team, possono visualizzare i team associati ai loro gruppi, indipendentemente dal fatto che siano membri del team. </p>
          <p><b>Disabilitato</b>: quando gli utenti cercano i team in un campo di completamento automatico Team, possono visualizzare i team associati ai loro gruppi solo se sono membri del team</p><p>Questa opzione è attivata per impostazione predefinita.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Visualizza tutti i team</td>
         <td><p>Quando questa opzione è abilitata e gli utenti cercano i team in un campo di completamento automatico Team, gli utenti possono visualizzare e selezionare qualsiasi team.</p><p>Questa opzione è attivata per impostazione predefinita. </p></td>
        </tr>
       </tbody>
      </table>

   * **Modifica**: se stai configurando il modo in cui gli utenti con una licenza Pianificazione e Lavoro possono gestire i team, modifica una delle seguenti opzioni:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Crea</td>
         <td><p>Consente agli utenti con una licenza Pianificazione o Lavoro di creare team.</p><p>Questa opzione è attivata per impostazione predefinita.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Elimina</td>
         <td><p> Consente agli utenti con una licenza Pianificazione di eliminare i team a cui hanno accesso per la modifica (non disponibile per gli utenti con una licenza Lavoro).</p><p>Questa opzione è attivata per impostazione predefinita.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Modifica team nei gruppi che gestisco (solo per amministratori di gruppi)</td>
         <td><p>Consente agli utenti con licenza Pianificazione che sono designati come amministratori di gruppi di modificare i team associati ai gruppi che gestiscono.</p><p>Questa opzione è attivata per impostazione predefinita.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Modifica i team a cui collaboro</td>
         <td><p>Consente agli utenti di pianificare la licenza o la licenza Lavoro per modificare i team di cui sono membri.</p><p>Questa opzione è disabilitata per impostazione predefinita.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Visualizza i team associati ai miei gruppi</td>
         <td>
         <p><b>Abilitato</b> Quando gli utenti cercano i team in un campo di completamento automatico Team, gli utenti possono vedere i team associati ai loro gruppi indipendentemente dal fatto che siano membri del team. </p>
         <p><b>Disabilitato</b>: quando gli utenti cercano i team in un campo di completamento automatico Team, possono visualizzare i team associati ai loro gruppi solo se sono membri del team</p><p>Questa opzione è attivata per impostazione predefinita.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Visualizza tutti i team</td>
         <td><p>Quando questa opzione è abilitata e gli utenti cercano i team in un campo di completamento automatico Team, gli utenti possono visualizzare e selezionare qualsiasi team.</p><p>Questa opzione è attivata per impostazione predefinita. </p></td>
        </tr>
       </tbody>
      </table>

1. Fare clic sulla X per chiudere la casella **Ottimizza impostazioni**.
1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configura l&#39;accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), ad esempio [Concedi l&#39;accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedi l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fare clic su **Salva**.

>[!NOTE]
>
>* Le seguenti condizioni sono vere, indipendentemente dalle impostazioni del livello di accesso:
>
>   * I proprietari dei team possono sempre visualizzare e modificare i propri team
>   * Gli utenti hanno sempre accesso alla visualizzazione dei team a cui appartengono
>
>* La configurazione di qualsiasi opzione disponibile sia per Visualizza che per Modifica (ad esempio &quot;Visualizza team associati ai miei gruppi&quot;) viene mantenuta se si decide di selezionare Visualizza invece di Modifica o Modifica invece di Visualizza in un livello di accesso.
>

## Accesso ai team per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ogni livello di accesso possono eseguire con i problemi, vedere la sezione [Team](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) nell&#39;articolo [Funzionalità disponibile per ogni tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
