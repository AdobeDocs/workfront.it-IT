---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Messaggio di errore: Parametro non valido: valore di conversione"
description: '"Quando si tenta di modificare il formato di un campo personalizzato in un modulo personalizzato esistente, viene visualizzato il seguente messaggio di errore: ''Parametro non valido: valore di conversione `&lt;..&gt;`""'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 1%

---

# Messaggio di errore: Parametro non valido: valore di conversione

## Problema

Quando si tenta di modificare il formato di un campo personalizzato in un modulo personalizzato esistente, viene visualizzato il seguente messaggio di errore: &quot;Parametro non valido: valore di conversione &quot;&lt;...>&quot;&quot;\
![custom_field_format_valid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Causa

Questo messaggio si verifica nel seguente scenario:

Ad esempio, è disponibile un campo personalizzato formattato come Testo .  A questo punto, è necessario modificare il formato del campo personalizzato in Valuta. In un punto della tua istanza di Adobe Workfront, questo campo è già associato a un oggetto e contiene informazioni già specificate. Le informazioni esistenti in almeno un campo di questo tipo sono già formattate come Testo. Pertanto, il formato del campo non può essere modificato in Valuta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">piano Workfront</a>*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica sulle licenze legacy</a>*</p> </td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Livello di accesso*</strong> </td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Creare rapporti, dashboard e calendari</p> </li> 
     <li> <p>Creare filtri, visualizzazioni e gruppi</p> </li> 
    </ul> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Soluzione

Effettua le seguenti operazioni:

1. Creare rapporti per tutti gli oggetti a cui potrebbe essere associato questo campo con il proprio Forms personalizzato.\
   Per informazioni sulla creazione di un rapporto, vedi [Creare un rapporto personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Includi il campo personalizzato che stai tentando di modificare nella visualizzazione del rapporto, in modo da vedere quale oggetto contiene questo campo compilato con un valore di testo.
1. Correggere i valori del campo personalizzato degli oggetti visualizzati in formato testo e assegnare loro un valore formattato come Valuta; quindi provare a modificare nuovamente il campo Formato del modulo personalizzato.\
   Oppure\
   Se nel modulo personalizzato sono già presenti troppi valori di campo con informazioni in formato testo, è consigliabile aggiungere un nuovo campo personalizzato e formattarlo come valuta.
