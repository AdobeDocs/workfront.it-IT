---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Stampare un riepilogo delle bozze in Adobe Workfront
description: Puoi stampare un riepilogo della bozza, salvarlo come PDF o esportarlo come file XLS o PDF ottimizzato per Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 1b85267e811f5832480316be5322ee819abaf190
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 1%

---

# Stampare un riepilogo delle bozze in Adobe Workfront

Puoi stampare un riepilogo della bozza, salvarlo come PDF o esportarlo come file XLS o PDF ottimizzato per Adobe Reader.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Piano corrente: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell'accesso con i diversi piani, vedere <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alla funzionalità di verifica in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano corrente: Lavoro o Piano</p> <p>Piano legacy: qualsiasi (per l’utente deve essere abilitata la verifica)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, la mansione o il profilo di autorizzazione della bozza di cui si dispone, contattare l&#39;amministratore di Workfront o Workfront Proof.

+++

## Stampare un riepilogo della bozza o salvarlo come file PDF

È possibile stampare un riepilogo delle bozze direttamente dall&#39;elenco dei documenti.

>[!NOTE]
>
>Non è possibile stampare contemporaneamente più riepiloghi delle bozze dall&#39;elenco dei documenti.

1. Nell&#39;elenco dei documenti che contiene la bozza, posizionare il puntatore del mouse sulla riga contenente il documento, quindi fare clic su **Stampa riepilogo**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   Oppure

   Quando visualizzi la bozza nel visualizzatore di bozze, fai clic sull&#39;icona **Stampa** nella barra degli strumenti a sinistra. ![](assets/print-icon-in-pv.png) Se la barra degli strumenti sinistra non è visibile, fare clic sull&#39;icona Menu ![](assets/menu-icon-in-pv.png) nell&#39;angolo superiore sinistro del visualizzatore di bozze.

1. Utilizza una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mostra</td> 
      <td> <p>Specificare gli elementi da stampare:</p> 
       <ul> 
        <li>La <strong>versione corrente</strong> o <strong>tutte le versioni</strong> della bozza</li> 
        <li>Solo le <strong>pagine con commenti</strong> o <strong>tutte le pagine</strong></li> 
        <li>Solo le <strong>miniature di pagina</strong> (un piccolo rendering di ogni pagina) o <strong>pagine intere</strong> (un rendering completo della bozza)<br></li> 
        <p>Nota: per visualizzare i numeri di pin nel markup nell'output stampato, è necessario selezionare Pagine intere e non Miniature pagina. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ordina commenti per</td> 
      <td> <p>(Disponibile solo se è stata selezionata l'opzione Miniature pagina in alto) Specificare l'ordine di stampa dei commenti della bozza:</p> 
       <ul> 
        <li><strong>Più vecchio</strong>: dal primo commento all'ultimo</li> 
        <li><strong>Più recente</strong>: dall'ultimo commento al primo</li> 
        <li><strong>Pagina</strong>: per pagina, dalla prima all'ultima pagina o dall'ultima alla prima</li> 
        <li><strong>Autore</strong>: in base ai nomi degli utenti che li hanno aggiunti, da A-Z o da Z-A</li> 
       </ul> <p>Queste opzioni non influiscono sull'output esportato come file XLS o PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtra commenti per</td> 
      <td> <p>È possibile utilizzare una qualsiasi combinazione di queste opzioni per includere solo determinati commenti nell'output stampato o esportato come file XLS o PDF:</p> 
       <ul> 
        <li>Autori selezionati (impostazione predefinita)</li> 
        <li>Azioni selezionate</li> 
        <li><strong>Stato non risolto</strong></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Flusso di lavoro</td> 
      <td> <p>(Disponibile solo se la bozza dispone di un flusso di lavoro automatico) È possibile fare clic su <strong>Mostra diagramma</strong> per includere un diagramma nell'output stampato che mostra le fasi della bozza e le decisioni prese in ogni fase. Nel diagramma visualizzato, i colori rappresentano le decisioni prese su uno stage:</p> <p><strong>Verde</strong>: approvato</p> <p><strong>Blu</strong>: in attesa di decisione</p> <p><strong>Rosso</strong>: è necessario modificare la decisione</p> <p><strong>Grigio</strong>: non ancora iniziato</p> <p><strong>Giallo</strong>: approvato con modifiche</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fare clic su **Stampa**.
1. Nel pannello di destra della finestra visualizzata, se desideri stampare il riepilogo, fai clic sul menu **Destinazione**, quindi fai clic su **Ulteriori informazioni**. Fare clic sulla stampante che si desidera utilizzare nell&#39;elenco visualizzato, quindi fare clic su **Stampa**.

   Oppure

   Se vuoi salvare il riepilogo come file di PDF, fai clic sul menu **Destinazione**, fai clic su **Salva come PDF** e quindi su **Salva**.

## Esportare un riepilogo della bozza come XLS o PDF

Puoi esportare un riepilogo della bozza per il contenuto statico come file XLS o come file PDF. Le esportazioni di bozze includono solo il contenuto della bozza.

1. Nell&#39;elenco dei documenti che contiene la bozza, posizionare il puntatore del mouse sulla riga contenente il documento, quindi fare clic su **Stampa riepilogo**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Fai clic sull’icona XLS o PDF nell’angolo superiore destro della pagina.

   ![](assets/xls-pdf-icons-350x136.png)

Quando il file esportato è pronto, ricevi un’e-mail da cui puoi scaricare il file.

Se hai esportato il riepilogo come file PDF, i commenti sulla bozza vengono visualizzati nel lettore PDF. Se a un commento sono associati più markup, il commento verrà visualizzato più volte nell&#39;elenco dei commenti (una volta per ogni markup).
