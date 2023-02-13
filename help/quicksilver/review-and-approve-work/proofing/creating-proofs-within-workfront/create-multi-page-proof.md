---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Creare una bozza a più pagine
description: È possibile combinare più file in un’unica bozza multipagina. I revisori possono utilizzare gli strumenti di navigazione nel visualizzatore di correzione per sfogliare le pagine in una bozza a più pagine.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# Creare una bozza a più pagine

È possibile combinare più file in un’unica bozza multipagina. I revisori possono utilizzare gli strumenti di navigazione nel visualizzatore di correzione per sfogliare le pagine in una bozza a più pagine.

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

&#42;Per informazioni sul piano, la licenza o il profilo delle autorizzazioni di prova, contattare l&#39;amministratore Workfront o Workfront Proof.

## Creare una bozza a più pagine

Quando questa opzione è abilitata, i file statici e i siti web sono disponibili in un’unica bozza. Quando questa opzione è disabilitata, tutti i documenti e i siti web vengono generati come singole bozze e puoi caricare fino a 100 file alla volta.

Per creare una bozza a più pagine:

1. Vai al progetto, all&#39;attività o al problema in cui desideri ottenere la bozza, quindi fai clic sul pulsante **Documenti** sezione .
1. Fai clic su **Aggiungi nuovo** > **Prova** .
1. Trascina e rilascia i file oppure sfoglia e selezionali dall’elenco di cartelle dei file. Puoi caricare fino a 50 file alla volta. Per informazioni sui limiti dei file, consulta la sezione [Considerazioni](#considerations) in questo articolo.

   >[!NOTE]
   >
   >I file interattivi, compresi i video e i siti web interattivi, non possono essere combinati in un’unica bozza.

1. Sotto **A prova singola**, abilita l’opzione , **Combinare tutti i file compatibili in un’unica bozza**.
1. In **Nome della bozza** Specifica un nuovo nome per la bozza combinata.
1. (Facoltativo) Nell’elenco dei file caricati, riordina i file trascinandoli. L’ordine dei file corrisponde all’ordine di pagina della bozza combinata.
1. (Facoltativo) Per rimuovere un singolo file dalla pagina Nuova bozza, passa il puntatore del mouse sul file e fai clic sul pulsante **Cestino** a destra.

   Oppure

   Per eliminare tutti i file caricati contemporaneamente, fai clic su **Elimina tutto** nell&#39;angolo superiore destro dell&#39;elenco.

1. Una volta caricati tutti i file, devi decidere se configurare una bozza di base o una bozza automatica:

   * Con una bozza di base, puoi aggiungere tutti i revisori desiderati a una bozza, ma non sono organizzati in fasi. Tutti i revisori aggiunti possono accedere alla bozza immediatamente dopo la creazione. Per configurare una bozza di base, vedi [Creare una bozza avanzata con un flusso di lavoro di base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Con una bozza automatica, la bozza si sposta da un passaggio all’altro e Adobe Workfront notifica a ogni utente quando tocca a lui rivederla. per configurare una bozza automatica, vedi [Creare una bozza avanzata con un flusso di lavoro automatizzato](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Considerazioni {#considerations}

Quando si combinano file in un’unica bozza, considera quanto segue:

* Puoi caricare fino a 500 file separati.
* È possibile combinare file statici di tipi diversi (ad esempio, PDF, JPG, DOC, PPT, EXC), fino a un totale di 2.000 pagine.
* È possibile combinare le immagini web statiche.
* È possibile combinare file GIF; tuttavia, i GIF animati vengono elaborati come file statici.
* Non è possibile combinare file AV e acquisizione web interattiva.
* L’immagine miniatura della bozza viene presa dalla prima pagina della bozza (vedi [Gestire i dettagli delle prove in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Puoi controllare i nomi dei file combinati per creare la bozza nella pagina dei dettagli della bozza. Per ulteriori informazioni, consulta [Gestire i dettagli delle prove in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Se l’opzione per scaricare i file originali è abilitata nella bozza, puoi scaricare tutti i file che sono stati combinati per creare la bozza come file .zip. Per ulteriori informazioni, consulta  [Scarica i file archiviati in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
