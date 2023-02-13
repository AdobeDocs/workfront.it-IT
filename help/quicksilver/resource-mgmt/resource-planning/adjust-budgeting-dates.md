---
product-area: resource-management
navigation-topic: resource-planning
title: Adeguare le date di budget nel Planner risorse
description: Se si riscontrano sovrassegnazioni delle risorse dopo averle inserite in budget nel Planner risorse, è possibile esplorare scenari What-if spostando le ore in budget, FTE o Costi in un altro intervallo di tempo. In base ai risultati di questi scenari, puoi quindi regolare le ore, gli FTE o i costi preventivati.
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 1%

---

# Adeguare le date di budget nel Planner risorse

Se si riscontrano sovrassegnazioni delle risorse dopo averle inserite in budget nel Planner risorse, è possibile esplorare scenari What-if spostando le ore in budget, FTE o Costi in un altro intervallo di tempo. In base ai risultati di questi scenari, puoi quindi regolare le ore, gli FTE o i costi preventivati.

Le sovrallocazioni possono apparire quando le ore previste, gli FTE o i costi delle risorse sono superiori alle ore disponibili, agli FTE o ai Costi. Questo genera un valore netto negativo.

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro e superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica l'accesso a Gestione risorse che include l'accesso a Modifica priorità e ore di budget nel Planner risorse</p> <p>Modificare l’accesso a Dati finanziari, Progetti e Utenti</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Consente di gestire le autorizzazioni per i progetti per i quali si desidera assegnare il budget alle informazioni con la possibilità di gestire le finanze</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Modifica date budget

1. Vai al Planner risorse e seleziona **Visualizza per progetto**.

   >[!NOTE]
   >
   >È possibile utilizzare l&#39;opzione Regola date budget solo quando si visualizza il planner risorse per progetto.

1. Passa il puntatore del mouse sul nome di un progetto, quindi fai clic sul pulsante **Altro** menu.
1. Fai clic su **Adeguamento date budget**.\
   Viene visualizzata la timeline dell’allocazione del progetto.\
   L&#39;intervallo di tempo in cui le ore sono attualmente in budget viene evidenziato in arancione in caso di conflitto di budget e in blu in caso di conflitti.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Trascina e rilascia l’intervallo di tempo evidenziato in un altro momento per capire dove non ci sono conflitti di budget per il progetto selezionato. Quando si trova un intervallo di tempo in cui il valore Net è positivo, l&#39;intervallo di tempo evidenziato diventa blu.
1. Fai clic sulla &quot;x&quot; nell’angolo in alto a destra della timeline di allocazione del progetto per chiuderla.
1. Rimuovi le ore previste dalla timeline esistente del progetto e aggiungili alla timeline che mostra la maggiore disponibilità.
1. Fai clic su **Salva**.
1. (Condizionale e facoltativo) Se gli intervalli di tempo senza conflitti di budget si trovano al di fuori della timeline del progetto, fai clic sul nome del progetto per accedere al progetto.
1. (Condizionale e facoltativo) Fai clic su **Modifica progetto**, quindi modifica il **Data di inizio prevista** o **Data completamento pianificata** modificare la cronologia del progetto per l&#39;intervallo di tempo senza conflitti di budget.\
   Per ulteriori informazioni sulla modifica dei progetti, consulta l’articolo [Modifica progetti](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Condizionale e facoltativo) Fai clic su **Salva modifiche**.
1. Tornare al Planner risorse e reinserire le ore previste, le FTE o i Costi nell&#39;intervallo di tempo senza conflitti di budget.
1. Fai clic su **Salva**.
