---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Esempio di campo personalizzato calcolato: visualizzare una marca temporale di stato in un modulo personalizzato"
description: Nel campo calcolato seguente viene visualizzata la data in cui lo stato dell'oggetto è contrassegnato come In corso (INP.) È possibile utilizzare le stesse informazioni per i campi personalizzati calcolati per problemi, attività o progetti.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Esempio di campo personalizzato calcolato: visualizza una marca temporale di Stato in un modulo personalizzato

Nel campo calcolato seguente viene visualizzata la data in cui lo stato dell&#39;oggetto è contrassegnato come In corso (INP.) È possibile utilizzare le stesse informazioni per i campi personalizzati calcolati per problemi, attività o progetti.

>[!NOTE]
>
>Se lo stato dell&#39;oggetto cambia in INP, lo stato cambia e quindi torna a INP, Adobe Workfront acquisisce solo la marca temporale della prima modifica in INP.

## Requisiti di accesso

Devi avere i seguenti:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Per informazioni sulla pianificazione, il tipo di licenza o l'accesso disponibili, contattare l'amministratore Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Adobe Workfront*</p> </td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurazioni del livello di accesso*</strong> </td> 
   <td> <p>Modificare l’accesso per creare rapporti, dashboard e calendari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorizzazioni oggetto</strong> </p> </td> 
   <td> <p>Gestire le autorizzazioni sull’oggetto a cui è allegato il modulo</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.<br>Per ulteriori informazioni sulle autorizzazioni per le dashboard, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Condividere report, dashboard e calendari </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisito

Per aggiungere a un modulo personalizzato un campo calcolato che visualizzi la cronologia delle modifiche di un campo, è necessario innanzitutto creare il modulo personalizzato.

## Visualizzare un timestamp di stato in un modulo personalizzato

1. Passare a un modulo personalizzato in cui si desidera aggiungere il campo.
1. Fare clic su **Calcolato** per aggiungere al modulo un campo personalizzato calcolato.
1. Digitare un **Etichetta** per il campo personalizzato. Ad esempio, &quot;Campo personalizzato Timestamp stato&quot;.
1. Fai clic su **Salva+Chiudi**.
1. Riapri il modulo personalizzato, quindi seleziona il nuovo campo personalizzato **Timestamp stato** nel modulo.
1. Nella casella **Calcolo**, copia e incolla il seguente calcolo per il campo personalizzato:

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Questo calcolo è identico per tutti gli oggetti e per tutti gli stati. In questo calcolo è sempre necessario utilizzare la chiave a tre lettere e non il nome dello stato dell&#39;oggetto.
   >
   >Per ulteriori informazioni sulle chiavi per gli stati, vedere [Creare o modificare uno stato](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Fai clic su **Salva+Chiudi**.

   È ora possibile creare rapporti sul campo personalizzato Timestamp stato o utilizzarlo in altri calcoli, rapporti o campi personalizzati.
