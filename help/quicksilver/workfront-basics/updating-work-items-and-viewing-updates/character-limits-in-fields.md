---
content-type: reference
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Limiti dei caratteri nei campi
description: Alcuni campi in Adobe Workfront limitano il numero di caratteri che possono essere inclusi nel campo . Workfront indicizza il contenuto in modo che possa essere ricercato in un secondo momento. Viene applicato un limite di caratteri per garantire prestazioni di alta qualità del sistema Workfront.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f09dadf4-24f2-46d9-85ae-6081731d917d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 5%

---

# Limiti dei caratteri nei campi

Alcuni campi in Adobe Workfront limitano il numero di caratteri che possono essere inclusi nel campo . Workfront indicizza il contenuto in modo che possa essere ricercato in un secondo momento. Viene applicato un limite di caratteri per garantire prestazioni di alta qualità del sistema Workfront.

Quando si avvicina il limite, viene visualizzato un contatore. Quando si supera il limite, i caratteri in eccesso vengono evidenziati e non è possibile pubblicare il testo. Elimina i caratteri fino a quando non ti trovi entro il limite consentito.

Il limite di caratteri varia a seconda del campo in uso. I limiti indicati di seguito si applicano alle lingue che utilizzano un alfabeto latino (come l&#39;inglese). Il limite potrebbe essere inferiore per le lingue che contengono caratteri a byte esteso o doppio.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo di campo</strong> </p> </th> 
   <th> <p><strong>Limite caratteri (</strong><strong>spazi inclusi)</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Campo di testo con formattazione in un modulo personalizzato</td> 
   <td>15,000</td> 
  </tr> 
  <tr> 
   <td> <p>Aggiornamento di stato</p> </td> 
   <td> <p>15,000</p>
   <p> 4.000 quando si utilizza l’API</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aggiorna</p> </td> 
   <td> <p>15,000</p> 
   <p> 4.000 quando si utilizza l’API</p></td> 
  </tr> 
  <tr> 
   <td> <p>Descrizione (documenti, attività, problemi, portafogli, programmi e progetti)</p> </td> 
   <td> <p>4,000</p> </td> 
  </tr> 
  <tr> 
   <td>Campo descrizione in un modulo personalizzato</td> 
   <td>4,000</td> 
  </tr> 
  <tr> 
   <td> <p>Paragrafo dati personalizzato o testo a riga singola </p> </td> 
   <td> <p>2,000</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Campo descrizione nel Report Builder</p> </td> 
   <td> <p>512</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Etichetta menu a discesa</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nome Oggetto</p> </td> 
   <td> <p>255</p> </td> 
  </tr> 
 </tbody> 
</table>
