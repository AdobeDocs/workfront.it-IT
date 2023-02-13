---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Raggruppamento: modifica il nome visualizzato in un raggruppamento'
description: È possibile rinominare i raggruppamenti in modo più familiare agli utenti.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Raggruppamento: modificare il nome visualizzato in un raggruppamento

È possibile rinominare i raggruppamenti in modo più familiare agli utenti.

Ad esempio, quando applichi il raggruppamento Nome Portfolio standard a un elenco di progetti, il nome del raggruppamento viene visualizzato come *Portfolio: Nome:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

È possibile modificare il raggruppamento utilizzando la modalità testo per visualizzare un nome più leggibile.

![](assets/grouping-edited-name-350x160.png)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a rapporti, dashboard, calendari</p> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Modificare il nome visualizzato in un raggruppamento

Per modificare il nome visualizzato in un raggruppamento di progetti:

1. Vai a un elenco di progetti.
1. Da **Raggruppamento** menu a discesa, seleziona **Nuovo raggruppamento**.

1. Fai clic su **Aggiungi raggruppamento** e inizia a digitare &quot;Nome Portfolio&quot; nella **Primo da:** , quindi selezionalo quando viene visualizzato nell’elenco.

1. Fai clic su **Passa alla modalità testo**.
1. Effettuare una delle seguenti operazioni:

   * Aggiungi il codice seguente al testo esistente disponibile nel **Raggruppa il rapporto** casella:

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      Oppure, in questo caso:

      ```
      group.0.displayname=Portfolio
      ```

   * Rimuovi tutte le righe nell’interfaccia della modalità testo del raggruppamento che contiene la parola &quot;nome&quot;, quindi aggiungi la riga:

      ```
      group.0.name=Your Value
      ```

      Oppure, in questo caso:

      ```
      group.0.name=Portfolio
      ```

      Puoi anche lasciare la

      ```
      group.0.name
      ```

      riga vuota, nel qual caso il raggruppamento mostra il nome del valore per il quale stai raggruppando.

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. Fai clic su **Fine**, quindi **Salva raggruppamento**.
