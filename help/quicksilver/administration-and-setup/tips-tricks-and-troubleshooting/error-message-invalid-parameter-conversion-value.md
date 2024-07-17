---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Messaggio di errore: parametro non valido: valore di conversione"
description: '"Quando si tenta di modificare il formato di un campo personalizzato in un modulo personalizzato esistente, viene visualizzato il seguente messaggio di errore: "Parametro non valido: valore di conversione "&lt;...&gt;""'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Messaggio di errore: Parametro non valido: valore di conversione

## Problema

Viene visualizzato il seguente messaggio di errore quando si tenta di modificare il formato di un campo personalizzato in un modulo personalizzato esistente: &quot;Parametro non valido: valore di conversione &quot;&lt;...>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Causa

Questo messaggio viene visualizzato nello scenario seguente:

Ad esempio, un campo personalizzato è formattato come testo.  Ora si desidera modificare il formato del campo personalizzato in Valuta. In un punto qualsiasi dell’istanza di Adobe Workfront, questo campo è già associato a un oggetto e contiene informazioni già specificate. Le informazioni esistenti in almeno un campo di questo tipo sono già formattate come testo. Pertanto, il formato del campo non può essere modificato in Valuta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Piano Workfront</a>*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Panoramica licenze</a>*</p> </td> 
   <td>Piano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Livello di accesso*</strong> </td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Creare rapporti, dashboard e calendari</p> </li> 
     <li> <p>Creare filtri, visualizzazioni e raggruppamenti</p> </li> 
    </ul> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Soluzione

Effettua le seguenti operazioni:

1. Creare report per tutti gli oggetti a cui questo campo potrebbe essere associato con il proprio Forms personalizzato.\
   Per informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Includi il campo personalizzato che stai tentando di modificare nella visualizzazione del rapporto, in modo da vedere quale oggetto ha questo campo popolato con un valore di testo.
1. Correggere i valori del campo personalizzato degli oggetti visualizzati in formato testo e assegnare loro un valore formattato come Valuta, quindi tentare di modificare nuovamente il campo Formato nel modulo personalizzato.\
   Oppure\
   Se sono già presenti troppi valori di campo con informazioni in formato testo, è consigliabile aggiungere un nuovo campo personalizzato al modulo personalizzato e formattarlo come Valuta.
