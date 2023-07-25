---
title: File di test nascosto
author: Bob
description: Nascosto dalla ricerca e dal menu di navigazione a sinistra
hidefromtoc: true
hide: true
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
source-git-commit: 5c47b09550c54b7ea4f8319bb42e93572e06324b
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---


# File di test nascosto - TEST BRANCH FUNZIONALITÀ

File nascosto dalla ricerca (`hide: yes`) e dal menu di navigazione a sinistra (`hidefromtoc: yes`).

<span class="preview">Questo file è **nascosto** dalla ricerca (`hide: yes`) e dal menu di navigazione a sinistra (`hidefromtoc: yes`).</span>

<p class="preview">Questo file viene **nascosto** dalla ricerca (`hide: yes`) e dalla navigazione a sinistra (`hidefromtoc: yes`).</p>

## Test immagine

![test immagine](assets/get-started.png){width="50" align="center"}

## Prova di evidenziazione anteprima

**Utilizza DIV per blocchi di componenti.**

Il DIV inizia di seguito.

<div class="preview">

Inizio DIV.

>[!NOTE]
>
>Questa è una nota.
>
>Ho una richiesta per evidenziare lo sfondo della nota.

![immagine](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

Ultimo elemento evidenziato.

</div>

DIV termina in alto.

**Usa SPAN per paragrafi o frasi**

Questo è un paragrafo. <span class="preview">Sono un testo giallo.</span> Ricorda di chiudere la sintassi correttamente, altrimenti la pagina potrebbe essere riprodotta in modo strano.

DIV e SPAN sono utili anche nelle tabelle HTML.

**Altri elementi HTML supportati**

È inoltre possibile specificare `class="preview"` sintassi in `<p>`, `<td>`, `<tr>`e così via. Verifica l’anteprima.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr class="preview"> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">piano Adobe Workfront</a>*</td> 
   <td> <p>Pro o superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"></td> 
   <td> <p class="preview">Piano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Accesso Jira</td> 
   <td> <p><span class="preview">Accesso amministratore di sistema</p> <p>Importante: è consigliabile creare account amministratore di sistema separati in Jira e Workfront per dedicarsi a questa integrazione, anziché utilizzare account esistenti che potrebbero essere collegati agli utenti. </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Devi essere un amministratore di Workfront. Per informazioni sugli amministratori di Workfront, consulta .</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Video con qualità = 12

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=12)

Video con qualità = 6

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=6)

Video nella tabella HTML

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  </tr> 
  <tr> 
   <td role="rowheader">Questo video funziona?</td> 
   <td>No, non è </td> 
  </tr> 
 </tbody> 
</table>

Video all’interno di una tabella markdown

| Colonna 1 | Colonna 2 |
|---|---|
| Questo funziona? | Inoltre no |


