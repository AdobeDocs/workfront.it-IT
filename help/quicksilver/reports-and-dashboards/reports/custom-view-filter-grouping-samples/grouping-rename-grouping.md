---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Raggruppamento: modificare il nome visualizzato in un raggruppamento'
description: È possibile rinominare i raggruppamenti in elenchi e rapporti in modo più familiare agli utenti.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Raggruppamento: modificare il nome visualizzato in un raggruppamento

<!--Audited: 01/2024-->

È possibile rinominare i raggruppamenti in modo da renderli più familiari agli utenti.

Ad esempio, quando applichi il raggruppamento Nome Portfolio standard a un elenco di progetti, il nome del raggruppamento viene visualizzato come *Portfolio: Nome:`<name of portfolio>`*.

![Raggruppamento per nome non modificato](assets/grouping-unedited-name-350x167.png)

È possibile modificare questo raggruppamento utilizzando la modalità testo per visualizzare un nome più facile da leggere.

![Raggruppamento per nome modificato](assets/grouping-edited-name-350x160.png)

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> 
    <p>Nuovo:</p>
   <ul><li><p>Collaboratore per modificare un filtro </p></li>
   <li><p>Standard per modificare un rapporto</p></li> </ul>

<p>Corrente:</p>
   <ul><li><p>Richiesta di modifica di un filtro </p></li>
   <li><p>Pianificare la modifica di un rapporto</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificare il nome visualizzato in un raggruppamento

Per modificare il nome visualizzato in un raggruppamento di progetti:

1. Consente di passare a un elenco di progetti.
1. Dal menu a discesa **Raggruppamento**, selezionare **Nuovo raggruppamento**.

1. Fare clic su **Aggiungi raggruppamento** e iniziare a digitare &quot;Nome Portfolio&quot; nel campo **Raggruppa per:**, quindi selezionarlo quando viene visualizzato nell&#39;elenco.

1. Fare clic su **Passa alla modalità testo**.
1. Eseguire una delle operazioni seguenti:

   * Aggiungi il codice seguente al testo esistente disponibile nella casella **Raggruppa il report**:


     `group.0.displayname=Your Value`


     Ad esempio, aggiungi il seguente codice per cambiare il nome visualizzato in &quot;Portfolio&quot;:

     `group.0.displayname=Portfolio`

   * Rimuovi tutte le righe dell’interfaccia in modalità testo del raggruppamento contenenti la parola &quot;name&quot;, quindi aggiungi la riga:

     `group.0.name=Your Value`

     Ad esempio, aggiungi il seguente codice per cambiare il nome visualizzato in &quot;Portfolio&quot;:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >È inoltre possibile lasciare vuote le righe `group.0.name=` e `group.0.displayname=`, nel qual caso il raggruppamento mostra il valore in base al quale si sta effettuando il raggruppamento.


     ![Raggruppamento per nome modificato senza nome](assets/grouping-edited-name-no-name-350x162.png)

1. Fai clic su **Fine**, quindi su **Salva raggruppamento**.
1. (Facoltativo) Aggiornare il nome del raggruppamento, quindi fare clic su **Salva raggruppamento**.

   Il nome predefinito per il raggruppamento viene modificato in base alle informazioni sulla modalità di testo.
