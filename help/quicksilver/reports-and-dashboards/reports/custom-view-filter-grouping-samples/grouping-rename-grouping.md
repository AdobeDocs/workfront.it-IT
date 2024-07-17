---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: modificare il nome visualizzato in un raggruppamento"
description: È possibile rinominare i raggruppamenti in elenchi e rapporti in modo più familiare agli utenti.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 138181de2ad8257785773a5296bc5bcfc144a801
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Raggruppamento: modificare il nome visualizzato in un raggruppamento

<!--Audited: 01/2024-->

È possibile rinominare i raggruppamenti in modo da renderli più familiari agli utenti.

Quando ad esempio si applica il raggruppamento Nome Portfolio standard a un elenco di progetti, il nome del raggruppamento viene visualizzato come *Portfolio: Nome:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

È possibile modificare questo raggruppamento utilizzando la modalità testo per visualizzare un nome più facile da leggere.

![](assets/grouping-edited-name-350x160.png)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td>

<p>Nuovo: </p>
   <ul>
   <li> <p>Collaboratore per modificare un raggruppamento </p></li>
   <li><p>Standard per modificare un rapporto</p></li></ul>

<p> Corrente:</p>
   <ul>  
   <li><p>Richiesta di modifica di un raggruppamento </p></li>
   <li><p>Pianificare la modifica di un rapporto</p></li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modifica l'accesso a Filtri, Viste, Raggruppamenti per modificare un raggruppamento</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Modificare il nome visualizzato in un raggruppamento

Per modificare il nome visualizzato in un raggruppamento di progetti:

1. Consente di passare a un elenco di progetti.
1. Dal menu a discesa **Raggruppamento**, selezionare **Nuovo raggruppamento**.

1. Fare clic su **Aggiungi raggruppamento** e iniziare a digitare &quot;Nome Portfolio&quot; nel campo **Primo per:**, quindi selezionarlo quando viene visualizzato nell&#39;elenco.

1. Fare clic su **Passa alla modalità testo**.
1. Eseguire una delle operazioni seguenti:

   * Aggiungi il codice seguente al testo esistente disponibile nella casella **Raggruppa il report**:


     `group.0.displayname=Your Value`


     Oppure, in questo caso:

     `group.0.displayname=Portfolio`

   * Rimuovi tutte le righe dell’interfaccia in modalità testo del raggruppamento contenenti la parola &quot;name&quot;, quindi aggiungi la riga:

     `group.0.name=Your Value`

     Oppure, in questo caso:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >È inoltre possibile lasciare vuote le righe `group.0.name=` e `group.0.displayname=`, nel qual caso il raggruppamento mostra il valore in base al quale si sta effettuando il raggruppamento.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Fai clic su **Fine**, quindi su **Salva raggruppamento**.

   Il nome predefinito per il raggruppamento viene modificato in base alle informazioni sulla modalità di testo.
