---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '''Filtro: Report di approvazione della bozza per omettere le versioni di prova precedenti'
description: In un rapporto di approvazione della bozza, è possibile utilizzare il filtro Is Current Document Version per includere solo le versioni correnti delle bozze in attesa dell'approvazione.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Filtro: rapporto di approvazione della bozza per omettere le versioni di bozza precedenti

In un rapporto di approvazione della bozza, puoi utilizzare il **È la versione corrente del documento** per includere solo le versioni correnti delle bozze in attesa dell’approvazione.

Questa opzione è utile, ad esempio, se ti è stato chiesto di approvare bozze con più versioni. Quando si esegue il rapporto Approvazione bozza con il filtro Versione documento corrente, il rapporto elenca solo la versione corrente di ogni bozza in attesa di approvazione, omettendo versioni precedenti su cui non è più necessario lavorare. 

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

## Filtrare il rapporto di approvazione della bozza per omettere le versioni di bozza precedenti

1. Se disponi già di un rapporto di approvazione della bozza, aprilo.

   Oppure

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Per creare un rapporto di approvazione della bozza personalizzato, fare clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti** ![](assets/reports-in-main-menu.png). Fai clic su **Nuovo rapporto**. Nell’elenco visualizzato, scorri verso e fai clic su **Approvazione della bozza**. Fai clic su **Salva e chiudi**, digitare a **Nome del rapporto** (facoltativo), quindi fai clic su **Salva rapporto**.

1. Fai clic su **Azioni rapporto > Modifica**.
1. Fai clic su **Filtri**, quindi fai clic su **Aggiungere una regola filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Fai clic su **Approvazione della bozza**.
1. Nell’elenco visualizzato, fai clic su **È la versione corrente del documento**.
1. Fai clic su **Salva e chiudi** nell’angolo in basso a sinistra di Adobe Workfront, quindi fai clic su **Salva rapporto** nella casella visualizzata.
