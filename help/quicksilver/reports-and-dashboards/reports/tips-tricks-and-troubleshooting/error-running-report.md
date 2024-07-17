---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Messaggio di errore durante l’esecuzione di un rapporto: "Non hai effettuato l’accesso"."'
description: Scopri il messaggio di errore "Non hai effettuato l’accesso".
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 3%

---

# Messaggio di errore durante l’esecuzione di un rapporto: &quot;Non hai effettuato l’accesso&quot;.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano, Lavoro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Problema

Quando si esegue un report o lo si visualizza in un dashboard, viene restituito il seguente errore:\
*Riproviamo. Non si è al momento connessi.*

Nessun risultato viene visualizzato nel rapporto.

## Causa

Il report è attualmente impostato per l&#39;esecuzione come utente disattivato.

## Soluzione

Per modificare le impostazioni del report è necessario disporre delle autorizzazioni di gestione.\
Per adeguare il rapporto e visualizzare i risultati:

1. Passa al report.
1. Fai clic su **Azioni report** > **Modifica** > **Impostazioni report**.

1. Specificare il nome di un utente attivo nel campo **Esegui report con diritti di accesso di:**.\
   Oppure\
   Lasciare vuoto il campo **Esegui report con diritti di accesso di:**.

1. Fai clic su **Fine**.
1. Fai clic su **Salva e Chiudi**.\
   L’errore non dovrebbe più essere visualizzato durante l’esecuzione del rapporto.
