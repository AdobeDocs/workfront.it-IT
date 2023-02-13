---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Esempio di campo personalizzato calcolato: visualizza il manager del creatore di un problema sul modulo personalizzato del problema"
description: Utilizzando un campo personalizzato calcolato, puoi visualizzare il nome del manager del creatore di un problema su un modulo personalizzato allegato al problema. Utilizzando la stessa istruzione, è possibile creare campi calcolati simili per progetti, problemi e altri oggetti.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Esempio di campo personalizzato calcolato: visualizza il manager del creatore di un problema sul modulo personalizzato del problema

Utilizzando un campo personalizzato calcolato, puoi visualizzare il nome del manager del creatore di un problema su un modulo personalizzato allegato al problema. Utilizzando la stessa istruzione, è possibile creare campi calcolati simili per progetti, problemi e altri oggetti.

>[!TIP]
>
>Per informazioni su ulteriori esempi di modalità di testo personalizzata forniti da altri clienti, consulta la sezione [Reporting in modalità testo](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) argomento sul nostro sito Community.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Adobe Workfront*</p> </td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configurazioni a livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati<br>Per informazioni sulla concessione dell'accesso amministrativo dal livello di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Consentire agli utenti l'accesso amministrativo a determinate aree</a>.</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto</p> </td> 
   <td> <p>Accesso a Contribute per l'oggetto a cui è allegato il modulo con accesso a Modifica modulo personalizzato</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Visualizza il manager del creatore di un problema sul modulo personalizzato per il problema

I passaggi seguenti mostrano come creare un campo calcolato per un modulo personalizzato per problemi in cui acquisire il nome del manager dell’utente che ha creato il problema. Il processo è identico quando desideri acquisire il nome del manager di un utente che ha creato un’attività, un progetto, un portfolio, ad esempio.

1. Crea un modulo personalizzato per un problema e aggiungi un campo calcolato.

   Per informazioni sulla creazione di un modulo personalizzato e sull’aggiunta di campi calcolati, vedere i seguenti articoli:

   * [Creare o modificare un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [Aggiungere dati calcolati a un modulo personalizzato](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. Copia e incolla il seguente codice della modalità testo nel **Calcolo** campo del modulo personalizzato:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Per i calcoli dei campi personalizzati viene fatta distinzione tra maiuscole e minuscole.

1. Fai clic su **Fine**, quindi **Salva e chiudi**.

   Il gestore dell’utente che ha creato il problema viene visualizzato nel campo calcolato quando il modulo che contiene il campo è associato a un problema.
