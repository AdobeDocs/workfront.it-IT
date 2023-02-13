---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '''Esempio di campo personalizzato calcolato: visualizzare una marca temporale di stato in un modulo personalizzato"'
description: Il seguente campo calcolato visualizza la data in cui lo stato dell’oggetto è contrassegnato come In corso (INP). È possibile utilizzare le stesse informazioni per i campi personalizzati calcolati per problemi, attività o progetti.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Esempio di campo personalizzato calcolato: visualizzare una marca temporale di stato in un modulo personalizzato

Il seguente campo calcolato visualizza la data in cui lo stato dell’oggetto è contrassegnato come In corso (INP). È possibile utilizzare le stesse informazioni per i campi personalizzati calcolati per problemi, attività o progetti.

>[!NOTE]
>
>Se lo stato dell’oggetto cambia in INP, allora cambia in un altro stato, quindi di nuovo in INP, Adobe Workfront acquisisce solo la marca temporale della prima modifica in INP.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Per sapere quale piano, tipo di licenza o accesso si dispone, contattare l'amministratore Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Adobe Workfront*</p> </td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurazioni a livello di accesso*</strong> </td> 
   <td> <p>Modifica l’accesso a Creazione di report, dashboard e calendari</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Consente di gestire le autorizzazioni per l’oggetto a cui è allegato il modulo</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.<br>Per ulteriori informazioni sulle autorizzazioni per le dashboard, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Condividere rapporti, dashboard e calendari </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisito

Per aggiungere a un modulo personalizzato un campo calcolato che visualizzi la cronologia delle modifiche di un campo, è innanzitutto necessario creare il modulo personalizzato.

## Visualizzazione di una marca temporale di stato in un modulo personalizzato

1. Passare a un modulo personalizzato in cui si desidera aggiungere il campo.
1. Fai clic su **Calcolato** per aggiungere al modulo un campo personalizzato calcolato.
1. Tipo a **Etichetta** per il campo personalizzato, ad esempio *Campo personalizzato marca temporale stato*.
1. Fai clic su **Fine**, quindi fai clic su **Salva e chiudi**.
1. Riaprire il modulo personalizzato, quindi selezionare il nuovo **Campo personalizzato marca temporale stato** sul modulo.
1. In **Calcolo** consente di copiare e incollare il calcolo seguente per il campo personalizzato:

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Questo calcolo è identico per tutti gli oggetti e per tutti gli stati. In questo calcolo è sempre necessario utilizzare la chiave a tre lettere e non il nome dello stato per lo stato dell’oggetto.
   >
   >Per ulteriori informazioni sulle chiavi per gli stati, consulta [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Fai clic su **Salva e chiudi**.

   È ora possibile creare rapporti sul campo personalizzato Timestamp di stato o utilizzarlo in altri calcoli, nei rapporti o nei campi personalizzati.
