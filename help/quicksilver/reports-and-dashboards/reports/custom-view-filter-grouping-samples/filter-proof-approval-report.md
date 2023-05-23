---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Filtro: rapporto Proof Approval (Approvazione della bozza) per omettere le versioni precedenti della bozza"
description: In un rapporto Proof Approval (Approvazione bozza) è possibile utilizzare il filtro Is Current Document Version (È versione corrente del documento) per includere solo le versioni correnti delle bozze in attesa di approvazione.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Filtro: rapporto Proof Approval (Approvazione della bozza) per omettere le versioni precedenti della bozza

In un rapporto Proof Approval (Approvazione della bozza), è possibile utilizzare il **È la versione del documento corrente** per includere solo le versioni correnti delle bozze in attesa della tua approvazione.

Ciò è utile, ad esempio, se ti è stato chiesto di approvare bozze che hanno più versioni. Quando si esegue il rapporto Proof Approval (Approvazione della bozza) con il filtro Is Current Document Version (È versione corrente del documento), nel rapporto viene elencata solo la versione corrente di ogni bozza in attesa di approvazione, omettendo le versioni precedenti su cui non è più necessario lavorare. 

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
   <td> <p>Richiesta di modifica di un filtro </p>
   <p>Pianificare la modifica di un rapporto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare un rapporto</p> <p>Modificare l’accesso a Filtri, Viste, Raggruppamenti per modificare un filtro</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, consulta <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedi accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore Workfront.

## Filtrare il rapporto Proof Approval (Approvazione della bozza) per omettere le versioni precedenti della bozza

1. Se disponi già di un rapporto Proof Approval (Approvazione della bozza), aprilo.

   Oppure

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Per creare un rapporto Proof Approval personalizzato, fai clic sul menu principale ![](assets/main-menu-icon.png), quindi fai clic su **Rapporti** ![](assets/reports-in-main-menu.png). Clic **Nuovo rapporto**. Nell&#39;elenco visualizzato scorrere fino a e fare clic su **Approvazione bozza**. Clic **Salva e chiudi**, digitare a **Nome report** (facoltativo), quindi fai clic su **Salva report**.

1. Clic **Azioni report > Modifica**.
1. Clic **Filtri**, quindi fai clic su **Aggiungere una regola di filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Clic **Approvazione bozza**.
1. Nell&#39;elenco visualizzato fare clic su **È la versione del documento corrente**.
1. Clic **Salva e chiudi** nell’angolo in basso a sinistra di Adobe Workfront, fai clic su **Salva report** nella casella visualizzata.
