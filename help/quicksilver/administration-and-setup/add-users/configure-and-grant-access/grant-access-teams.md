---
title: Concedere l’accesso ai team
description: In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai team in Workfront
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 4%

---

# Concedere l’accesso ai team

In qualità di amministratore di Adobe Workfront, puoi utilizzare un livello di accesso per definire l’accesso di un utente ai team in Workfront, come spiegato in [Panoramica dei livelli di accesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare l’accesso degli utenti per modificare gli utenti utilizzando un livello di accesso personalizzato

1. Inizia a creare o modificare il livello di accesso, come spiegato in [Creare o modificare livelli di accesso personalizzati](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Fai clic sull’icona a forma di ingranaggio ![](assets/gear-icon-settings.png) sulla **Visualizza** o **Modifica** pulsante a destra di Team, quindi selezionare le capacità che si desidera concedere in **Ottimizzare le impostazioni**.

   * **Visualizza**: Se stai configurando il modo in cui gli utenti con una licenza possono visualizzare i team, modifica una delle seguenti opzioni:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Visualizza i team associati ai miei gruppi</td>
         <td>
          <p><b>Abilitato</b>: Quando gli utenti cercano i team in un campo di tipo Team-ahead, gli utenti possono vedere i team associati ai loro gruppi, indipendentemente dal fatto che siano membri del gruppo o meno. </p>
          <p><b>Disabilitato</b>: Quando gli utenti cercano team in un campo di tipo Team-ahead, gli utenti possono vedere i team associati ai loro gruppi solo dove sono membri del team</p><p>Questa opzione è attivata per impostazione predefinita.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Visualizza tutti i team</td>
         <td><p>Quando questa opzione è abilitata e gli utenti cercano team in un campo di tipo Team-ahead, gli utenti possono vedere e selezionare qualsiasi team.</p><p>Questa opzione è attivata per impostazione predefinita. </p></td>
        </tr>
       </tbody>
      </table>

   * **Modifica**: Se si sta configurando il modo in cui gli utenti con una licenza Pianifica e una licenza Lavoro possono gestire i team, modificare una delle opzioni seguenti:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Crea</td>
         <td><p>Consente agli utenti con una licenza Pianifica o Lavoro di creare team.</p><p>Questa opzione è attivata per impostazione predefinita.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Elimina</td>
         <td><p> Consente agli utenti con una licenza Plan di eliminare i team a cui hanno accesso per la modifica (non disponibili per gli utenti con una licenza Work).</p><p>Questa opzione è attivata per impostazione predefinita.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Modifica team nei gruppi che gestisco (solo per amministratori di gruppi)</td>
         <td><p>Consente agli utenti con licenza Plan designati come amministratori di gruppo di modificare i team associati ai gruppi gestiti.</p><p>Questa opzione è attivata per impostazione predefinita.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Modifica team in corso</td>
         <td><p>Consente agli utenti di pianificare licenze o licenze di lavoro per modificare i team in cui sono membri.</p><p>Questa opzione è disabilitata per impostazione predefinita.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Visualizza i team associati ai miei gruppi</td>
         <td>
         <p><b>Abilitato</b> Quando gli utenti cercano i team in un campo di tipo Team-ahead, gli utenti possono vedere i team associati ai loro gruppi, indipendentemente dal fatto che siano membri del gruppo o meno. </p>
         <p><b>Disabilitato</b>: Quando gli utenti cercano team in un campo di tipo Team-ahead, gli utenti possono vedere i team associati ai loro gruppi solo dove sono membri del team</p><p>Questa opzione è attivata per impostazione predefinita.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Visualizza tutti i team</td>
         <td><p>Quando questa opzione è abilitata e gli utenti cercano team in un campo di tipo Team-ahead, gli utenti possono vedere e selezionare qualsiasi team.</p><p>Questa opzione è attivata per impostazione predefinita. </p></td>
        </tr>
       </tbody>
      </table>

1. Fai clic sulla X per chiudere la **Ottimizzare le impostazioni** scatola.
1. (Facoltativo) Per configurare le impostazioni di accesso per altri oggetti e aree nel livello di accesso su cui stai lavorando, continua con uno degli articoli elencati in [Configurare l’accesso ad Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), quali [Concedere l’accesso alle attività](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Concedere l’accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Al termine, fai clic su **Salva**.

>[!NOTE]
>
>* Le seguenti affermazioni sono vere, indipendentemente dalle impostazioni del livello di accesso:
   >
   >   * I proprietari del team possono sempre visualizzare e modificare i propri team
   >   * Gli utenti hanno sempre accesso per visualizzare i team in cui si trovano
>
* La configurazione di qualsiasi opzione disponibile sia per Visualizza che per Modifica (ad esempio &quot;Visualizza team associati ai miei gruppi&quot;) viene mantenuta se si decide di selezionare Visualizza invece di Modifica o Modifica anziché Visualizza in un livello di accesso.
>


## Accesso ai team per tipo di licenza

Per informazioni sulle operazioni che gli utenti di ciascun livello di accesso possono eseguire con i problemi, consulta la sezione . [Team](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) nell&#39;articolo [Funzionalità disponibile per ciascun tipo di oggetto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
