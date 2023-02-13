---
product-area: reporting
navigation-topic: text-mode-reporting
title: Confronto dei campi nella formattazione condizionale
description: È possibile utilizzare la formattazione condizionale per confrontare 2 campi diversi in una visualizzazione e evidenziarli quando determinati criteri sono soddisfatti tra i campi.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Confronto dei campi nella formattazione condizionale

È possibile utilizzare la formattazione condizionale per confrontare 2 campi diversi in una visualizzazione e evidenziarli quando determinati criteri sono soddisfatti tra i campi.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modificare l’accesso a Filtri, Visualizzazioni, Gruppi</p> <p>Modificare l’accesso a Report, Dashboard e Calendari per modificare la visualizzazione in un report</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un rapporto per modificare la visualizzazione in un rapporto</p> <p>Gestire le autorizzazioni per una visualizzazione</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Esempio: Confrontare la data di inizio effettiva e la data di inizio pianificata

Ad esempio, se la data di inizio effettivo di un&#39;attività è successiva alla data di inizio pianificata, è possibile evidenziare la colonna Data inizio pianificata utilizzando la formattazione condizionale.

Per confrontare la data di inizio prevista e la data di inizio effettivo dell&#39;attività utilizzando la formattazione condizionale:

1. Passare a una visualizzazione attività o a un report.
1. (Condizionale) Se lavori con un rapporto, dalla **Colonne (visualizzazione)** fare clic sull&#39;intestazione della colonna che si desidera formattare in modo condizionale per selezionarla.\
   Ad esempio, seleziona la **Data di inizio effettiva** Se si desidera aggiungere la formattazione condizionale confrontando i campi Data inizio pianificata e Data inizio effettiva.

1. Fai clic su **Opzioni avanzate**, quindi fai clic su Aggiungi un **Regola per questa colonna**.

1. Immetti i criteri di confronto utilizzando i valori esistenti nel generatore e specifica la formattazione condizionale.\
   Ad esempio, si desidera evidenziare le attività in cui la data di inizio effettiva è successiva ( o superiore) alla data di inizio prevista. Selezionare il modificatore Maggiore di e selezionare una data effettiva nel campo data.\
     ![](assets/cond-format-1-350x84.png)

1. (Facoltativo) Seleziona **Applica a riga intera** se si desidera applicare la formattazione all&#39;intera riga.
1. Fai clic su **Aggiungi regola**, quindi **Fine**.

1. Seleziona la **Data di inizio effettiva** , quindi fai clic su **Passa alla modalità testo**.

1. **Fare clic per modificare il testo** quindi aggiungi la seguente riga di testo:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   Nel nostro esempio: 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Se si confronta un campo nativo di Workfront, utilizzare la sintassi della maiuscola per il nome del campo. Se si confronta un campo personalizzato, utilizzare **DE:Nome effettivo del campo** per il campo nome che si sta confrontando con il primo campo.\
   >Ad esempio, se confronti la **Data di inizio effettiva** con un campo personalizzato etichettato **Data di consegna**, aggiungi la seguente istruzione nel codice della modalità testo:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Assicurati che `righttext` la riga di codice corrisponde all’istruzione nel `rightmethod` riga di codice.

   ![](assets/cond-format-2-350x171.png)

1. Fai clic su **Salva**.
1. Fai clic su **Salva e chiudi**.

   La colonna evidenzia i campi che soddisfano i criteri specificati.
