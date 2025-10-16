---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Disattivare o riattivare un’azienda
description: Puoi disattivare una società che non utilizzi più conservando tutti i dati storici associati. Se disattivi un’azienda già in uso da qualche parte nel sistema, questa continua a funzionare esattamente come sempre. Non viene rimosso o bloccato.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 8fb17d1008b00bc0701ce6e2f06c59d020510e90
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 1%

---

# Disattivare o riattivare un’azienda

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

Puoi disattivare una società che non utilizzi più conservando tutti i dati storici associati. Se disattivi un’azienda già in uso da qualche parte nel sistema, questa continua a funzionare esattamente come sempre. Non viene rimosso o bloccato.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] pacchetto</p> </td> 
   <td><p>Qualsiasi</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licenza</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
  <td> <p>È necessario disporre di uno dei seguenti elementi:</p> 
    <ul> 
     <li> <p>Il livello di accesso [!UICONTROL Amministratore di sistema], che consente di modificare qualsiasi società del sistema.</p> </li> 
     <li> <p>Accesso amministrativo per gestire le società, che consente di modificare qualsiasi società nel sistema.</p> </li> 
    </ul> <p><b>NOTA</b>:
     <ul> 
      <li> <p>Puoi anche gestire le aziende associate a qualsiasi gruppo a cui sei assegnato come amministratore di gruppo.</p> </li> 
      <li> <p>Per aggiungere e rimuovere utenti dal sistema [!DNL Workfront], è necessario disporre di uno dei seguenti elementi:</p> 
       <ul> 
        <li> <p>Livello di accesso [!UICONTROL System Administrator]. </p> </li> 
        <li> <p>Impostazione di <b>[!UICONTROL Utenti]</b> nel livello di accesso configurato per l'accesso <b>[!UICONTROL Modifica]</b>, con <b>[!UICONTROL Crea]</b> e almeno una delle due opzioni di <b>[!UICONTROL Amministratore utenti]</b> abilitate in <b>[!UICONTROL Ottimizza le impostazioni]</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Di queste due opzioni, se <b>[!UICONTROL User Admin (Group Users)]</b> è abilitato, è necessario essere un amministratore di gruppo di un gruppo di cui l'utente è membro.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Disattivare o riattivare un’azienda

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic sull&#39;icona **[!UICONTROL Aziende]** ![Aziende](assets/companies-icon-left-panel.png).

1. Seleziona una o più società da disattivare o riattivare.
1. Fai clic su **[!UICONTROL Modifica]**.<!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>-->
1. Per una singola azienda, disabilitare l&#39;opzione **[!UICONTROL È attivo]** per disattivarla o abilitare l&#39;opzione per attivarla. <!--ADD TO THE FRONT OF THIS SENTENCE In the Production environment, -->

   Oppure

   Per più società, seleziona **[!UICONTROL No]** dal menu a discesa **[!UICONTROL È attivo]** per disattivarle, oppure **[!UICONTROL Sì]** per attivarle.

1. Fai clic su **[!UICONTROL Salva modifiche]**.
