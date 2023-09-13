---
content-type: reference
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Limiti di caratteri nei campi
description: Alcuni campi in Adobe Workfront limitano il numero di caratteri che possono essere inclusi nel campo. Workfront indicizza il contenuto in modo che sia possibile eseguirne la ricerca in un secondo momento. Viene applicato un limite di caratteri per garantire prestazioni di alta qualità del sistema Workfront.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f09dadf4-24f2-46d9-85ae-6081731d917d
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 5%

---

# Limiti di caratteri nei campi

Alcuni campi in Adobe Workfront limitano il numero di caratteri che possono essere inclusi nel campo. Workfront indicizza il contenuto in modo che sia possibile eseguirne la ricerca in un secondo momento. Viene applicato un limite di caratteri per garantire prestazioni di alta qualità del sistema Workfront.

Quando si raggiunge il limite, viene visualizzato un contatore. Quando superi il limite, vengono evidenziati i caratteri in eccesso e non puoi pubblicare il testo. Elimina i caratteri fino a raggiungere il limite consentito.

Il limite di caratteri varia a seconda del campo in uso. I limiti riportati di seguito si applicano alle lingue che utilizzano un alfabeto latino (ad esempio l&#39;inglese). Il limite potrebbe essere inferiore per le lingue che contengono caratteri estesi o a doppio byte.

Gli amministratori di Workfront o gruppi non possono modificare i limiti dei caratteri nei campi.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo di campo</strong> </p> </th> 
   <th> <p><strong>Limite carattere (</strong><strong>spazi inclusi)</strong> </p> </th> 
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
