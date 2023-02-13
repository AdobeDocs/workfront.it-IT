---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Stampa un riepilogo delle prove in Adobe Workfront
description: È possibile stampare un riepilogo delle prove, salvarlo come PDF o esportarlo come file XLS o PDF ottimizzato per Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 1%

---

# Stampa un riepilogo delle prove in Adobe Workfront

È possibile stampare un riepilogo delle prove, salvarlo come PDF o esportarlo come file XLS o PDF ottimizzato per Adobe Reader.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Piano attuale: Pro o superiore</p> <p>oppure</p> <p>Piano legacy: Seleziona o Premium</p> <p>Per ulteriori informazioni sulla verifica dell’accesso con i diversi piani, consulta <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accesso alle funzionalità di correzione in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano attuale: Lavoro o piano</p> <p>Piano legacy: Qualsiasi (è necessario che la correzione sia attivata per l’utente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profilo autorizzazione bozza </td> 
   <td>Manager o superiore</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso ai documenti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il ruolo o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Stampa un riepilogo della bozza o salvalo come file PDF

È possibile stampare un riepilogo della bozza direttamente dall’elenco dei documenti.

>[!NOTE]
>
>Non è possibile stampare contemporaneamente più riepiloghi di bozza dall&#39;elenco dei documenti.

1. Nell’elenco dei documenti che contiene la bozza, passa il cursore del mouse sulla riga contenente il documento e fai clic su **Riepilogo stampa**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   Oppure

   Quando visualizzi la bozza nel visualizzatore di bozze, fai clic sul pulsante **Stampa** icona ![](assets/print-icon-in-pv.png) nella barra degli strumenti a sinistra. Se la barra degli strumenti a sinistra non è visibile, fare clic sull&#39;icona Menu ![](assets/menu-icon-in-pv.png) nell’angolo in alto a sinistra del visualizzatore di correzione).

1. Utilizza una delle seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mostra</td> 
      <td> <p>Specificare l'elemento da stampare:</p> 
       <ul> 
        <li>La <strong>Versione corrente</strong> o <strong>Tutte le versioni</strong> della prova</li> 
        <li>Solo il <strong>Pagine con commenti</strong> o <strong>Tutte le pagine</strong></li> 
        <li>Solo il <strong>Miniature delle pagine</strong> (un piccolo rendering di ogni pagina) o <strong>Pagine complete</strong> (rendering completo della bozza)<br></li> 
        <p>Nota: Per visualizzare i numeri dei pin sul markup nell’output stampato, devi selezionare Pagine intere, non Miniature di pagina. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ordina i commenti per</td> 
      <td> <p>(Disponibile solo se hai selezionato Miniature di pagina sopra) Specifica l’ordine in cui stampare i commenti della bozza:</p> 
       <ul> 
        <li><strong>Oldest</strong>: Dal primo commento all'ultimo</li> 
        <li><strong>Più recente</strong>: Da ultimo commento fatto a primo</li> 
        <li><strong>Pagina</strong>: Per pagina, dalla prima all’ultima pagina o dall’ultima alla prima</li> 
        <li><strong>Creatore</strong>: Con i nomi degli utenti che li hanno aggiunti, da A-Z o da Z-A</li> 
       </ul> <p>Queste opzioni non influiscono sull’output esportato come file XLS o PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtra commenti per</td> 
      <td> <p>È possibile utilizzare una qualsiasi combinazione di queste opzioni per includere solo alcuni commenti nell'output stampato o esportato come file XLS o PDF:</p> 
       <ul> 
        <li>Autori selezionati (predefinito)</li> 
        <li>Azioni selezionate</li> 
        <li><strong>Non risolto</strong> status</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Flusso di lavoro</td> 
      <td> <p>(Disponibile solo se la bozza dispone di un flusso di lavoro automatizzato) Puoi fare clic su <strong>Mostra diagramma</strong> per includere un diagramma nell'output stampato che illustri le fasi della prova e le decisioni prese in ogni fase. Nel diagramma che appare, i colori rappresentano le decisioni prese su un palco:</p> <p><strong>Verde</strong>: Approvato</p> <p><strong>Blu</strong>: In attesa di una decisione</p> <p><strong>Rosso</strong>: Modifiche alla decisione necessaria</p> <p><strong>Grigio</strong>: Non ancora iniziato</p> <p><strong>Giallo</strong>: Approvato con modifiche</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fai clic su **Stampa**.
1. Nel pannello di destra della finestra visualizzata, se desideri stampare il riepilogo, fai clic sul pulsante **Destinazione** menu, quindi fai clic su **Vedi altro**. Fare clic sulla stampante da utilizzare nell&#39;elenco visualizzato, quindi fare clic su **Stampa**.

   Oppure

   Se desideri salvare il riepilogo come file PDF, fai clic sul pulsante **Destinazione** menu, fai clic su **Salva come PDF**, quindi fai clic su **Salva**.

## Esporta un riepilogo delle prove come XLS o PDF

Puoi esportare un riepilogo delle prove per il contenuto statico come file XLS o come file PDF. Le esportazioni di prove includono solo il contenuto della bozza.

1. Nell’elenco dei documenti che contiene la bozza, passa il cursore del mouse sulla riga contenente il documento e fai clic su **Riepilogo stampa**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Fai clic sull’icona XLS o sull’icona di PDF posta nell’angolo in alto a destra della pagina.

   ![](assets/xls-pdf-icons-350x136.png)

Quando il file esportato è pronto, ricevi un’e-mail da cui puoi scaricare il file.

Se il riepilogo è stato esportato come file PDF, i commenti sulla bozza vengono visualizzati nel lettore PDF. Se a un commento sono associate più marcature, il commento verrà visualizzato più volte nell’elenco dei commenti (una volta per ogni markup).
