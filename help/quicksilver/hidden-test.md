---
title: File di prova nascosto
author: Bob
description: Nascosto dalla ricerca e dalla navigazione a sinistra
hidefromtoc: true
hide: true
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
source-git-commit: 1655726151338c47d8f81201db9ef0bb92d9ce9a
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---


# File di test nascosto - TEST DEL RAMO CARATTERISTICHE

Questo file è nascosto dalla ricerca (`hide: yes`) e dal menu di navigazione a sinistra (`hidefromtoc: yes`).

<span class="preview">Questo file è **nascosto** da ricerca (`hide: yes`) e dal menu di navigazione a sinistra (`hidefromtoc: yes`).</span>

<p class="preview">Questo file è **hidden*** dalla ricerca (`hide: yes`) e dal menu di navigazione a sinistra (`hidefromtoc: sì").</p>

## Test immagine

![test immagine](assets/get-started.png){width="50" align="center"}

## Test dell&#39;evidenziazione dell&#39;anteprima

**Utilizza DIV per i blocchi di componenti.**

DIV inizia qui sotto.

<div class="preview">

Inizio del DIV.

>[!NOTE]
>
>Questa è una nota.
>
>Ho una richiesta per evidenziare il contesto della nota.

![immagine](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

Ultimo elemento evidenziato.

</div>

DIV termina sopra.

**Usa SPAN per paragrafi o frasi**

Questo è un paragrafo. <span class="preview">Sono un testo giallo.</span> Ricordarsi di chiudere correttamente la sintassi, o la pagina potrebbe renderizzarsi stranamente.

DIV e SPAN sono utili anche nelle tabelle HTML.

**Altri elementi HTML supportati**

Puoi inoltre specificare la `class="preview"` sintassi in `<p>`, `<td>`, `<tr>`e così via. Assicurati di verificare l’anteprima.

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
   <td role="rowheader">Accesso a Jira</td> 
   <td> <p><span class="preview">Accesso amministratore di sistema</p> <p>Importante: È consigliabile creare account di amministratore di sistema separati in Jira e Workfront per dedicarsi a questa integrazione, anziché utilizzare quelli esistenti che potrebbero essere collegati agli utenti. </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Devi essere un amministratore Workfront. Per informazioni sugli amministratori di Workfront, consulta .</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
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
   <td>No </td> 
  </tr> 
 </tbody> 
</table>

Video all’interno di una tabella Markdown

| Colonna 1 | Colonna 2 |
|---|---|
| Questo funziona? | Anche no |
