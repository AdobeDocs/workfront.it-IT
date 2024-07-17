---
product-area: reporting
navigation-topic: text-mode-reporting
title: Confrontare i campi nella formattazione condizionale
description: È possibile utilizzare la formattazione condizionale per confrontare due campi diversi in una visualizzazione ed evidenziarli quando vengono soddisfatti determinati criteri tra i campi.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Confrontare i campi nella formattazione condizionale

È possibile utilizzare la formattazione condizionale per confrontare due campi diversi in una visualizzazione ed evidenziarli quando vengono soddisfatti determinati criteri tra i campi.

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
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso a Filtri, Viste, Raggruppamenti</p> <p>Modificare l’accesso a Rapporti, Dashboard, Calendari per modificare la visualizzazione in un rapporto</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un report per modificare la visualizzazione in un report</p> <p>Gestire le autorizzazioni per una visualizzazione</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Esempio: confrontare la data di inizio effettiva e la data di inizio pianificata

Se ad esempio la data di inizio effettiva di un&#39;attività è successiva alla data di inizio pianificata, è possibile evidenziare la colonna Data di inizio pianificata utilizzando la formattazione condizionale.

Per confrontare la Data inizio pianificata e la Data inizio effettiva dell&#39;attività utilizzando la formattazione condizionale:

1. Passare a una visualizzazione delle attività o a un report.
1. (Condizionale) Se si utilizza un report, dalla scheda **Colonne (visualizzazione)** fare clic sull&#39;intestazione della colonna che si desidera formattare in modo condizionale per selezionarla.\
   Selezionare ad esempio la colonna **Data inizio effettiva** se si desidera aggiungere la formattazione condizionale confrontando i campi Data inizio pianificata e Data inizio effettiva.

1. Fai clic su **Opzioni avanzate**, quindi fai clic su Aggiungi una **regola per questa colonna**.

1. Immetti i criteri di confronto utilizzando i valori esistenti trovati nel generatore e specifica la formattazione condizionale.\
   Ad esempio, si desidera evidenziare le attività in cui la data di inizio effettiva è successiva alla data di inizio pianificata (o successiva). Selezionare il modificatore Maggiore di e selezionare una data effettiva nel campo data.\
     ![](assets/cond-format-1-350x84.png)

1. (Facoltativo) Selezionare **Applica a tutta la riga** se si desidera applicare la formattazione all&#39;intera riga.
1. Fai clic su **Aggiungi regola**, quindi su **Fine**.

1. Selezionare la colonna **Data di inizio effettiva**, quindi fare clic su **Passa alla modalità testo**.

1. **Fare clic per modificare il testo**, quindi aggiungere la seguente riga di testo:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   Nel nostro esempio: 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Se confronti un campo nativo di Workfront, utilizza la sintassi Camel Case per il nome del campo. Se si confronta un campo personalizzato, utilizzare **DE:Nome effettivo del campo** per il campo del nome che si sta confrontando con il primo campo.\
   >Ad esempio, se confronti la **Data di inizio effettiva** con un campo personalizzato con etichetta **Data di consegna**, aggiungi la seguente istruzione nel codice della modalità di testo:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Verificare che la riga di codice `righttext` corrisponda all&#39;istruzione nella riga di codice `rightmethod`.

   ![](assets/cond-format-2-350x171.png)

1. Fai clic su **Salva**.
1. Fai clic su **Salva e Chiudi**.

   La colonna evidenzia i campi che soddisfano i criteri.
