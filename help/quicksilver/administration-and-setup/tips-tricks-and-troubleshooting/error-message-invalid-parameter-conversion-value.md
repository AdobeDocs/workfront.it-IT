---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Messaggio di errore: Parametro non valido: Valore di conversione'
description: 'Viene visualizzato il seguente messaggio di errore quando si tenta di modificare il formato di un campo personalizzato in un modulo personalizzato esistente: "Parametro non valido: valore di conversione "&lt;..&gt;""'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 2%

---

# Messaggio di errore: Parametro non valido: valore di conversione

## Problema

Viene visualizzato il seguente messaggio di errore quando si tenta di modificare il formato di un campo personalizzato in un modulo personalizzato esistente: &quot;Parametro non valido: valore di conversione &quot;&lt;...>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Causa

Questo messaggio viene visualizzato nello scenario seguente:

Ad esempio, un campo personalizzato è formattato come testo.  Ora si desidera modificare il formato del campo personalizzato in Valuta. In un punto qualsiasi dell’istanza di Adobe Workfront, questo campo è già associato a un oggetto e contiene informazioni già specificate. Le informazioni esistenti in almeno un campo di questo tipo sono già formattate come testo. Pertanto, il formato del campo non può essere modificato in Valuta.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr>
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a:</p> 
    <ul> 
     <li> <p>Creare rapporti, dashboard e calendari</p> </li> 
     <li> <p>Creare filtri, visualizzazioni e raggruppamenti</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Soluzione

Effettua le seguenti operazioni:

1. Creare report per tutti gli oggetti a cui questo campo potrebbe essere associato con il proprio Forms personalizzato.\
   Per informazioni sulla creazione di un report, vedere [Creare un report personalizzato](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Includi il campo personalizzato che stai tentando di modificare nella visualizzazione del rapporto, in modo da vedere quale oggetto ha questo campo popolato con un valore di testo.
1. Correggere i valori del campo personalizzato degli oggetti visualizzati in formato testo e assegnare loro un valore formattato come Valuta, quindi tentare di modificare nuovamente il campo Formato nel modulo personalizzato.\
   Oppure\
   Se sono già presenti troppi valori di campo con informazioni in formato testo, è consigliabile aggiungere un nuovo campo personalizzato al modulo personalizzato e formattarlo come Valuta.
