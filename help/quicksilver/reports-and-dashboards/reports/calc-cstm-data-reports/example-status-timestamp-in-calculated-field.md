---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Esempio di campo personalizzato calcolato: visualizzare un timestamp di stato in un modulo personalizzato'
description: Nel campo calcolato seguente viene visualizzata la data in cui lo stato dell'oggetto è contrassegnato come In corso (INP). È possibile utilizzare le stesse informazioni per i campi personalizzati calcolati per problemi, attività o progetti.
author: Jenny
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Esempio di campo personalizzato calcolato: visualizza una marca temporale di Stato in un modulo personalizzato

Nel campo calcolato seguente viene visualizzata la data in cui lo stato dell&#39;oggetto è contrassegnato come In corso (INP). È possibile utilizzare le stesse informazioni per i campi personalizzati calcolati per problemi, attività o progetti.

>[!NOTE]
>
>Se lo stato dell&#39;oggetto cambia in INP, lo stato cambia e quindi torna a INP, Adobe Workfront acquisisce solo la marca temporale della prima modifica in INP.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Pacchetto Adobe Workfront</p> </td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Adobe Workfront</p> </td> 
   <td>
      <p>Standard</p>
      <p>Piano</p></td>
  </tr> 
  <tr> 
   <td><p>Configurazioni del livello di accesso</p></td> 
   <td> <p>Modificare l’accesso per creare rapporti, dashboard e calendari</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni oggetto</p> </td> 
   <td> <p>Gestire le autorizzazioni sull’oggetto a cui è allegato il modulo</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
