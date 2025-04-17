---
title: Importa campi da Adobe Workfront
description: In Adobe Workfront Planning è possibile creare campi personalizzati per ogni tipo di record. È quindi possibile associare il campo ai record di Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 7%

---

<!--add to TOC-->

# Importare campi da Adobe Workfront

<span class="preview">Le informazioni evidenziate in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell’ambiente di anteprima per tutti i clienti. Dopo i rilasci mensili in Produzione, le stesse funzioni sono disponibili nell’ambiente di Produzione per i clienti che hanno abilitato i rilasci rapidi. </span>

<span class="preview">Per informazioni sulle versioni rapide, vedere [Abilitare o disabilitare le versioni rapide per l&#39;organizzazione](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Puoi importare copie dei campi Workfront esistenti. L&#39;importazione di campi da Workfront crea una copia di ogni campo per un tipo di record di Workfront Planning.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Prodotti</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Piano Adobe Workfront*</p></td> 
   <td> 
<p>Uno dei seguenti piani di Workfront:</p> 
<ul><li>Seleziona</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning non è disponibile per i piani Workfront legacy</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacchetto Adobe Workfront Planning*</p></td> 
   <td> 
<p>Qualsiasi </p> 
<p>Per ulteriori informazioni su quanto incluso in ogni piano di Workfront Planning, contattare l'account manager Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Piattaforma Adobe Workfront</p></td> 
   <td> 
<p>Per poter accedere a tutte le funzionalità di Workfront Planning, l’istanza di Workfront della tua organizzazione deve essere integrata in Adobe Unified Experience.</p> 
<p>Per ulteriori informazioni, vedere <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Esperienza unificata Adobe per Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licenza Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning non è disponibile per le licenze Workfront legacy</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurazione del livello di accesso</p></td> 
   <td> <p>Nessun controllo del livello di accesso per Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorizzazioni oggetto</p></td> 
   <td>   <p>Gestisci le autorizzazioni per un'area di lavoro <span class="preview"> e tipo di record</span> </a> </p>  
   <p>Gli amministratori di sistema dispongono delle autorizzazioni per tutte le aree di lavoro, incluse quelle che non hanno creato.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modello layout</p></td> 
   <td> <p>A tutti gli utenti, inclusi gli amministratori di Workfront, deve essere assegnato un modello di layout che includa l'area Planning nel menu principale. </p> </td> 
  </tr> 
</tbody> 
</table>

*Per ulteriori informazioni sui requisiti di accesso a Workfront, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni sull’importazione di campi da Workfront

* È possibile importare campi Workfront nativi o personalizzati in un tipo di record in Workfront Planning.
* L&#39;importazione dei campi di Workfront consente di creare copie degli stessi campi e di mantenere il nome del campo in Workfront Planning. Dopo essere stati copiati in Workfront Planning, i campi sono indipendenti dai campi Workfront originali e non condividono informazioni.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* Puoi aggiungere campi nativi o personalizzati dai seguenti oggetti Workfront:
   * Portfolio
   * Programma
   * Progetto
   * Attività
   * Problema
   * Documento
   * Azienda
   * Gruppo
   * Utente
   * Ruolo
   * Assegnazione
   * Ora
   * Fatturazione
     <!--Available only to Preview, but might not come to Prod:* Rate card - visible in Production but asking PM if it should be hidden-->
   * Spesa
   * Iterazione
     <!--* Non-labor resource - - visible in Production but asking PM if it should be hidden-->
     <!--* Non-labour resource category - - visible in Production but asking PM if it should be hidden-->
* È possibile che i campi di Workfront non conservino il tipo di campo, dopo essere stati importati in Workfront Planning.

  La tabella seguente mostra i tipi di campo di Workfront e il corrispondente tipo di campo di Workfront Planning.

  | Tipo di campo Workfront | Tipo di campo Workfront Planning |
  |------------------------------------------|-------------------------------|
  | Testo a riga singola in formato testo | Testo a riga singola |
  | Testo a riga singola in formato numerico | Numero |
  | Testo a riga singola in formato valuta | Valuta |
  | Paragrafo | Paragrafo |
  | Testo con formattazione | Paragrafo |
  | Elenco a discesa a selezione singola | Selezione singola |
  | Elenco a discesa multi-selezione | Selezione multipla |
  | I filtri di digitazione utente non sono supportati | Persone |
  | Calcolato* | Formula |
  | Data | Data |
  | Gruppo di caselle di controllo | Selezione multipla |
  | Pulsante di opzione | Selezione multipla |

  *I campi calcolati saranno disponibili in un secondo momento.
Tutti gli altri tipi di campo di Workfront non sono supportati in Workfront Planning.


## Importa campi da Workfront

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Fare clic sull&#39;area di lavoro di cui si desidera creare i tipi di record.

   Viene aperto il workspace e vengono visualizzati i tipi di record.

1. Fare clic sulla scheda di un tipo di record.

   Tutti i record esistenti associati al tipo di record vengono visualizzati nelle righe della vista tabella.

   >[!TIP]
   >
   >    Alcuni campi potrebbero essere nascosti. Fare clic su **Campi** e attivare l&#39;interruttore per i campi che si desidera visualizzare come colonne nella vista tabella.

1. Fai clic sull&#39;icona **+** nell&#39;angolo superiore destro della vista tabella

   Oppure

   Passa il puntatore del mouse sull&#39;intestazione di una colonna, fai clic sulla freccia rivolta verso il basso dopo il nome del campo, quindi fai clic su **Inserisci a sinistra** o **Inserisci a destra** per aggiungere il nuovo campo.
1. Fai clic su **Aggiungi esistente** nell&#39;angolo inferiore destro della scheda **Nuovo campo**. <!--check UI - did they change this??-->

   ![Aggiungi campi esistenti dal modale Workfront](assets/add-existing-fields-from-workfront-modal.png)

1. Inizia a digitare il nome di un campo Workfront esistente nell&#39;area di ricerca, quindi fai clic su **+** quando viene visualizzato nell&#39;elenco.
1. (Facoltativo) Digitare un altro campo, quindi fare clic su **+** quando viene visualizzato nell&#39;elenco.
1. (Facoltativo) Fai clic sull&#39;icona **Filtri** ![Icona Filtri nei campi di importazione](assets/filters-in-import-fields-icon.png), quindi aggiorna uno o entrambi i campi seguenti:

   * Tipo di oggetto: selezionare un tipo di oggetto Workfront di cui si desidera importare i campi.
   * Modulo personalizzato: seleziona uno o più moduli personalizzati da Workfront. È possibile selezionare un modulo personalizzato senza prima selezionare un tipo di oggetto.
1. Fai clic su **+**, quindi su **Aggiungi campi**.
I campi vengono aggiunti alla vista tabella e alle pagine dei dettagli dei record.

   >[!IMPORTANT]
   >
   >    È previsto un limite di 500 campi per qualsiasi tipo di record. I campi esistenti e i campi importati contribuiscono a questo limite.

   I campi aggiunti sono copie dei campi Workfront e non si connettono più ai campi originali in Workfront.