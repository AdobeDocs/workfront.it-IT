---
product-area: resource-management
navigation-topic: resource-planning
title: Esporta informazioni dal planner risorse
description: È possibile esportare le informazioni da qualsiasi visualizzazione del Planner risorse in un file Excel (.xlsx) salvato sul computer.
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# Esporta informazioni dal planner risorse

È possibile esportare le informazioni da qualsiasi visualizzazione del Planner risorse in un file Excel (.xlsx) salvato sul computer.

>[!IMPORTANT]
>
>Sono presenti limitazioni nella visualizzazione delle informazioni e nelle informazioni che è possibile esportare dal Planner risorse. Per informazioni su queste limitazioni, vedi [Limitazioni della visualizzazione di Resource Planner](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

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
   <td> <p>Revisione o superiore <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso a progetti, utenti e gestione risorse</p> <p><b>NOTA</b>

Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza autorizzazioni o versioni successive per progetti</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Esporta informazioni dal planner risorse

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Risorsa**. La **Planner** viene visualizzato per impostazione predefinita.

1. Selezionare la visualizzazione per il planner. Puoi selezionare una delle seguenti opzioni:

   * Visualizza per utente
   * Visualizza per progetto
   * Visualizza per ruolo

1. Fai clic su **Esporta**.

   Viene visualizzata la finestra di dialogo Opzioni esportazione.

   ![](assets/rp-export-options-box-350x421.png)

1. Specifica le seguenti informazioni:\
   **Data di inizio**: Data di inizio dell’esportazione. Il file esportato contiene informazioni sull’allocazione e sulla disponibilità a partire dal primo giorno della settimana contenente il giorno specificato.\
   **Numero di periodi**: Il numero di periodi di tempo da includere nel file. Il valore predefinito è 4 periodi.\
   **Tipo**: Il tipo di periodi di tempo in base ai quali visualizzare le informazioni nel file esportato (settimane, mesi o trimestri).\
   Di seguito sono riportati i periodi di tempo massimi esportabili:

   * 52 settimane
   * 36 mesi
   * 12 trimestri

   **Seleziona per esportare**: A seconda della visualizzazione selezionata, è possibile esportare le informazioni di disponibilità e budget per tutti gli oggetti elencati sullo schermo o per quelli specifici.
Puoi scegliere di esportare le seguenti informazioni:

   * Nella visualizzazione Progetto, seleziona per esportare:

      * Progetti
      * Progetti e Ruoli
      * Tutto (opzione predefinita)
   * Nella visualizzazione utente, seleziona per esportare:

      * Utenti
      * Utenti e Progetti
      * Tutto (opzione predefinita)
   * Nella Vista ruolo, seleziona per esportare:

      * Mansioni
      * Ruoli e Progetti
      * Tutto (opzione predefinita)

   **Formattazione dati**: A seconda di come si desidera visualizzare il file Excel, selezionare le seguenti opzioni:

   * **Raw**: Selezionare questa opzione per visualizzare le informazioni sulla disponibilità e sull&#39;allocazione non raggruppate in base agli oggetti a cui appartiene nel file Excel. (opzione predefinita)
   * **Raggruppato**: Selezionare questa opzione per visualizzare le informazioni sulla disponibilità e sull&#39;allocazione raggruppate in base agli oggetti a cui appartengono. In questo modo le informazioni esportate vengono visualizzate come visualizzate sullo schermo.

   Nella finestra di dialogo Opzioni di esportazione viene visualizzato un esempio dell’aspetto delle informazioni nel file esportato.

1. Fai clic su **Esporta** per esportare le informazioni dal planner risorse.\
   Vengono esportate solo le informazioni salvate.

1. (Condizionale) Se nelle visualizzazioni Ruolo o Progetto sono presenti ore budget non salvate, fai clic su **Salva e continua.**
Un file Excel (.xlsx) viene scaricato sul computer.
\
   L&#39;esportazione dal planner risorse non è disponibile mentre il file è pronto per il download.\
   (Condizionale) Se esporti una grande quantità di dati, riceverai un’e-mail con un collegamento in cui puoi scaricare il file.\
   ![RP_eamil_with_export_planner_attach.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Condizionale) Quando ricevi l’e-mail con il file esportato, fai clic su **Scarica** per scaricare il file.\
   Questo ti riporta a Workfront dove puoi scaricare il file.\
   Devi aver effettuato l’accesso a Workfront per completare il download.\
   Se non scarichi il file quando viene consegnato, il collegamento Scarica rimane attivo per 7 giorni dopo l’avvio dell’esportazione.
