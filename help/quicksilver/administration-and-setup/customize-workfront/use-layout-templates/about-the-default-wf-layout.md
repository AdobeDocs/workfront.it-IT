---
title: Informazioni sul layout predefinito di Adobe Workfront
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Il layout predefinito è la disposizione del menu principale , del pannello sinistro e delle viste, dei raggruppamenti e dei filtri prima che un amministratore Adobe Workfront apporti modifiche utilizzando un modello di layout.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: bd1ebbedecff63fcc9165bd6e409ca1b3b632b3d
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 6%

---

# Informazioni sul layout predefinito di Adobe Workfront

Il layout predefinito è la disposizione del menu principale ![](assets/main-menu-icon.png), del pannello sinistro e delle visualizzazioni, dei raggruppamenti e dei filtri prima che un amministratore Adobe Workfront apporti modifiche utilizzando un modello di layout.

Per informazioni su come un amministratore di Workfront può modificare il layout predefinito di un utente assegnandogli un modello di layout, vedere [Assegnare utenti a un modello di layout](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

>[!NOTE]
>
>Gli utenti possono modificare il proprio layout modificando le preferenze del profilo utente. Per ulteriori informazioni, vedere la sezione [Preferenze](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences) in [Configura impostazioni personali](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Layout predefiniti per ogni livello di accesso

Il layout predefinito di ogni utente dipende dal relativo livello di accesso. Alcuni utenti potrebbero non visualizzare determinate aree nel menu principale o alcune voci del pannello sinistro, a seconda del livello di accesso loro assegnato.

La tabella seguente mostra gli elementi del pannello sinistro visualizzati per impostazione predefinita per ogni livello di accesso. Viene inoltre indicata l’area di destinazione predefinita per ciascun livello di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area</th> 
   <th> Elementi del pannello sinistro </th> 
   <th> <p>Amministratore di Sistema</p> </th> 
   <th> <p>Pianificatore</p> </th> 
   <th>Collaboratore</th> 
   <th>Revisore</th> 
   <th>Richiedente</th> 
   <th>Utente esterno</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2"><strong>Progetti</strong> </td> 
   <td><strong>Progetti</strong> </td> 
   <td>✔ <br>(area di destinazione predefinita)</td> 
   <td><span style="font-weight: 400;"> ✔</span> <br>(area di destinazione predefinita)</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Portfolio</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Reporting</strong> </td> 
   <td><strong>Rapporti</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dashboard</strong> </p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Calendari</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="5"><strong>Persone</strong> (rinominato in <strong>Team</strong> per gli utenti con una licenza Lavoro)</td> 
   <td><strong>Team</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Persone</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> <!--
   <tr> 
    <td><strong>Legacy Resource Planning</strong> </td> 
    <td>✔ </td> 
    <td>✔ </td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
    <td>&nbsp;</td> 
   </tr>
  --> 
  <tr> 
   <td><strong>Pianificazione</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Pianificazione</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Richieste</strong> </td> 
   <td><strong>Nuova richiesta</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td><strong>Richieste inviate</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ <br>(area di destinazione predefinita)</td> 
   <td>✔ <br>(area di destinazione predefinita)</td> 
  </tr> 
  <tr> 
   <td><strong>Tutte le richieste</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Scheda orario</strong> </td> 
   <td><strong>Le mie schede orario</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Schede orario approvate</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Tutte le schede orario</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Documenti</strong> </td> 
   <td> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurazione</strong> </td> 
   <td> </td> 
   <td>✔ </td> 
   <td>Funzionalità limitata</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
