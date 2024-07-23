---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creare una bozza con più pagine
description: È possibile combinare più file in un’unica bozza multipagina. I revisori possono utilizzare gli strumenti di navigazione nel visualizzatore di bozze per sfogliare le pagine di una bozza multipagina.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Creare una bozza con più pagine

È possibile combinare più file in un’unica bozza multipagina. I revisori possono utilizzare gli strumenti di navigazione nel visualizzatore di bozze per sfogliare le pagine di una bozza multipagina.

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

&#42;Per conoscere il piano, la licenza o il profilo di autorizzazione della bozza di cui si dispone, contattare l&#39;amministratore di Workfront o Workfront Proof.

+++

## Creare una bozza con più pagine

Quando questa opzione è abilitata, i file statici e i siti web sono disponibili in un’unica bozza. Quando questa opzione è disattivata, tutti i documenti e i siti web vengono generati come bozze individuali e puoi caricare fino a 100 file alla volta.

Per creare una bozza con più pagine:

1. Vai al progetto, all&#39;attività o al problema in cui desideri la bozza, quindi fai clic sulla sezione **Documenti**.
1. Fai clic su **Aggiungi nuovo** > **Bozza**.
1. Trascina e rilascia i file o sfoglia e selezionali dall’Esplora file. Puoi caricare fino a 50 file alla volta. Per informazioni sui limiti dei file, consulta la sezione [Considerazioni](#considerations) in questo articolo.

   >[!NOTE]
   >
   >I file interattivi, inclusi video e siti web interattivi, non possono essere combinati in un’unica bozza.

1. In **Bozza singola**, abilita l&#39;opzione **Combina tutti i file compatibili in un&#39;unica bozza**.
1. Nel campo **Nome bozza**, specifica un nuovo nome per la bozza combinata.
1. (Facoltativo) Nell’elenco dei file che hai caricato, riordina i file trascinandoli. L’ordine dei file è l’ordine di pagina della bozza combinata.
1. (Facoltativo) Per rimuovere un singolo file dalla pagina New proof (Nuova bozza), passa il puntatore del mouse sul file e fai clic sull&#39;icona **Cestino** visualizzata a destra.

   Oppure

   Per eliminare tutti i file caricati contemporaneamente, fare clic su **Elimina tutti** nell&#39;angolo superiore destro dell&#39;elenco.

1. Una volta caricati tutti i file, devi decidere se configurare una bozza di base o automatica:

   * Con una bozza di base, puoi aggiungere tutti i revisori che desideri a una bozza, ma non sono organizzati in più fasi. Tutti i revisori aggiunti possono accedere alla bozza immediatamente dopo la sua creazione. Per configurare una bozza di base, vedere [Creare una bozza avanzata con un flusso di lavoro di base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Con una bozza automatizzata, la bozza si sposta da un palco all’altro e Adobe Workfront notifica a ogni utente quando è il momento di rivederla. per configurare una bozza automatizzata, vedere [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Considerazioni {#considerations}

Quando combini i file in una singola bozza, tieni presente quanto segue:

* Puoi caricare fino a 500 file separati.
* È possibile combinare file statici di tipi diversi (ad esempio, PDF, JPG, DOC, PPT, EXC), fino a un totale di 2.000 pagine.
* È possibile combinare le acquisizioni Web statiche.
* È possibile combinare file di GIF; tuttavia, i GIF animati vengono elaborati come file statici.
* Non è possibile combinare file AV e clip Web interattive.
* L&#39;immagine miniatura della bozza viene presa dalla prima pagina della bozza (vedi [Gestione dettagli bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Puoi controllare i nomi dei file combinati per creare la bozza nella pagina Dettagli bozza. Per ulteriori informazioni, vedere [Gestire i dettagli della bozza in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Se nella bozza è abilitata l’opzione per scaricare i file originali, puoi scaricare tutti i file che sono stati combinati per creare la bozza come file .zip. Per ulteriori informazioni, consulta  [Scarica i file archiviati in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
