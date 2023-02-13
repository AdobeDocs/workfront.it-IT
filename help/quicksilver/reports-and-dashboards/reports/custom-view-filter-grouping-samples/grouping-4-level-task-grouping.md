---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Raggruppamento: Raggruppamento di attività a 4 livelli per Proprietario Portfolio, Proprietario programma, Proprietario progetto e Stato progetto"
description: Questo gruppo di attività fornisce 4 livelli di raggruppamento. In questo caso, le attività sono raggruppate per Proprietario Portfolio, Proprietario programma, Proprietario progetto e Stato progetto. È possibile utilizzare solo fino a 3 livelli di raggruppamento utilizzando l’interfaccia standard. Per aggiungere un quarto livello, è necessario utilizzare la modalità testo. Non è possibile raggruppare i rapporti in base a più di 4 criteri contemporaneamente.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Raggruppamento: Raggruppamento di attività a 4 livelli per Proprietario Portfolio, Proprietario programma, Proprietario progetto e Stato progetto

Questo gruppo di attività fornisce 4 livelli di raggruppamento. In questo caso, le attività sono raggruppate per Proprietario Portfolio, Proprietario programma, Proprietario progetto e Stato progetto. È possibile utilizzare solo fino a 3 livelli di raggruppamento utilizzando l’interfaccia standard. Per aggiungere un quarto livello, è necessario utilizzare la modalità testo. Non è possibile raggruppare i rapporti in base a più di 4 criteri contemporaneamente.

![four_tier_group_for_Tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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

## Crea un raggruppamento di attività a 4 livelli per proprietario Portfolio, proprietario programma, proprietario progetto e stato progetto

Per applicare questo raggruppamento:

1. Passare a un elenco di attività.
1. Da **Raggruppamento** menu a discesa, seleziona **Nuovo raggruppamento**.

1. Fai clic su **Passa alla modalità testo**.
1. Rimuovi il testo nel **Raggruppa il rapporto** area.
1. Sostituisci il testo con il seguente codice:

   <pre>group.0.linkedname=project<br>group.0.name=Proprietario Portfolio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:proprietario:nome<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Proprietario del programma<br>group.1.notime=false<br>group.1.valuefield=project:program:proprietario:nome<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nidificato(project).nidificato(owner).string(name)<br>group.2.namekey=proiettore.mm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.value.format=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. Fai clic su **Salva raggruppamento**.
