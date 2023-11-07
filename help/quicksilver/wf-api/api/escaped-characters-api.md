---
content-type: api
navigation-topic: api-navigation-topic
title: Caratteri con escape nelle risposte API
description: Caratteri con escape nelle risposte API
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 8%

---

# Caratteri con escape nelle risposte API

La sintassi di alcune risposte API può contenere il carattere di escape, `\` (barra rovesciata). Un carattere di escape indica che il carattere o la stringa di caratteri che seguono immediatamente il carattere di escape hanno un valore speciale. Ad esempio: `\t` comunica al dispositivo di lettura che `t` deve essere interpretato come `tab` e non come la lettera &quot;t&quot;. Una stringa di uno o più caratteri che segue la barra rovesciata è detta sequenza di escape.

Le sequenze con escape esadecimali richiedono l’uso di cifre esadecimali valide. Nella tabella seguente sono elencate le sequenze di escape codificate nelle risposte API di Adobe Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Sequenza di escape</strong> </th> 
   <th><strong>Carattere Unicode</strong> </th> 
   <th><strong>Rappresenta</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>Dove: <em>x</em> è il codice esadecimale per i numeri da 0 a 7</p> </td> 
   <td>0-7</td> 
   <td>Caratteri Unicode rappresentati dai punti di codice da 0 a 7</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>Utilizzare il tasto Backspace</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>Linguetta</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>Nuova riga</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>Scheda Verticale</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>Feed modulo</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Ritorno a capo</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>Dove xx è il codice esadecimale per i numeri da 14 a 31</em> </p> </td> 
   <td>14 - 31</td> 
   <td>Caratteri Unicode rappresentati dai punti di codice da 14 a 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (Barra)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; (minore di)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (Barra rovesciata)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>Dove: <em>xxxx</em> è il codice esadecimale per qualsiasi numero superiore a 127</p> </td> 
   <td>128+</td> 
   <td>Caratteri Unicode per qualsiasi punto di codice superiore a 127</td> 
  </tr> 
 </tbody> 
</table>
