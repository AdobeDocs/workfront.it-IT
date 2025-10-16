---
product-area: reporting
navigation-topic: text-mode-reporting
title: Confrontare i campi nella formattazione condizionale
description: È possibile utilizzare la formattazione condizionale per confrontare due campi diversi in una visualizzazione ed evidenziarli quando vengono soddisfatti determinati criteri tra i campi.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 1%

---

# Confrontare i campi nella formattazione condizionale

<!-- Audited: 1/2025 -->

È possibile utilizzare la formattazione condizionale per confrontare due campi diversi in una visualizzazione ed evidenziarli quando vengono soddisfatti determinati criteri tra i campi.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
     <p>Standard</p>
     <p>Piano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare la visualizzazione in un rapporto</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per modificare la visualizzazione in un report</p> <p>Gestire le autorizzazioni per una visualizzazione</p></td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Esempio: confrontare la data di inizio effettiva e la data di inizio pianificata

Se ad esempio la data di inizio effettiva di un&#39;attività è successiva alla data di inizio pianificata, è possibile evidenziare la colonna Data di inizio pianificata utilizzando la formattazione condizionale.

Per confrontare la Data inizio pianificata e la Data inizio effettiva dell&#39;attività utilizzando la formattazione condizionale:

1. Passare a una visualizzazione delle attività o a un report.
1. (Condizionale) Se si utilizza un report, dalla scheda **Colonne (Visualizzazione)** dell&#39;editor report fare clic sull&#39;intestazione della colonna che si desidera formattare in modo condizionale per selezionarla.\
   Selezionare ad esempio la colonna **Data inizio effettiva** se si desidera aggiungere la formattazione condizionale confrontando i campi Data inizio pianificata e Data inizio effettiva.

1. Fai clic su **Opzioni avanzate**, quindi fai clic su Aggiungi una **regola per questa colonna**.

1. Immetti i criteri di confronto utilizzando i valori esistenti trovati nel generatore e specifica la formattazione condizionale.\
   Ad esempio, si desidera evidenziare le attività in cui la data di inizio effettiva è successiva alla data di inizio pianificata (o successiva). Selezionare il modificatore Maggiore di e selezionare una data effettiva nel campo data.

   ![Formattazione condizionale per la data di inizio effettiva](assets/cond-format-1-350x84.png)

1. (Facoltativo) Selezionare **Applica a tutta la riga** se si desidera applicare la formattazione all&#39;intera riga.
1. Fai clic su **Salva**.

1. Selezionare la colonna **Data di inizio effettiva**, quindi fare clic su **Passa alla modalità testo**.

1. Fai clic su **Modifica modalità testo**, quindi aggiungi la seguente riga di testo:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   Nel nostro esempio:

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Se confronti un campo nativo di Workfront, utilizza la sintassi Camel Case per il nome del campo. Se si confronta un campo personalizzato, utilizzare **DE:Actual Nome del campo** per il campo del nome che si sta confrontando con il primo campo.\
   >Ad esempio, se confronti la **Data di inizio effettiva** con un campo personalizzato con etichetta **Data di consegna**, aggiungi la seguente istruzione nel codice della modalità di testo:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Verificare che la riga di codice `righttext` corrisponda all&#39;istruzione nella riga di codice `rightmethod`.

   ![Formattazione condizionale](assets/cond-format-2-350x171.png)

1. Fai clic su **Salva**.
1. Fai clic su **Salva e Chiudi**.

   La colonna evidenzia i campi che soddisfano i criteri.
