---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Esempio di campo personalizzato calcolato: visualizza il manager dell’autore di un problema sul modulo personalizzato relativo al problema"
description: Utilizzando un campo personalizzato calcolato, è possibile visualizzare il nome del responsabile dell’autore di un problema in un modulo personalizzato allegato al problema. Utilizzando la stessa istruzione, è possibile creare campi calcolati simili per progetti, problemi e altri oggetti.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Esempio di campo personalizzato calcolato: visualizza il manager dell’autore di un problema sul modulo personalizzato relativo al problema

Utilizzando un campo personalizzato calcolato, è possibile visualizzare il nome del responsabile dell’autore di un problema in un modulo personalizzato allegato al problema. Utilizzando la stessa istruzione, è possibile creare campi calcolati simili per progetti, problemi e altri oggetti.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Piano Adobe Workfront*</p> </td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Adobe Workfront*</p> </td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configurazioni del livello di accesso*</td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati<br>Per informazioni sulla concessione dell'accesso amministrativo dal livello di accesso, vedere <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Concedere agli utenti l'accesso amministrativo ad alcune aree</a>.</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorizzazioni oggetto</p> </td> 
   <td> <p>Accesso di Contribute all’oggetto in cui è allegato il modulo con accesso per modificare il modulo personalizzato</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Visualizzare il manager dell’autore di un problema nel modulo personalizzato del problema

I passaggi seguenti mostrano come creare un campo calcolato per un modulo personalizzato relativo a un problema in cui è possibile acquisire il nome del manager dell’utente che ha creato il problema. Il processo è identico quando si desidera acquisire il nome del manager di un utente che ha creato un&#39;attività, un progetto o un portfolio, ad esempio.

1. Crea un modulo personalizzato per la segnalazione di un problema e aggiungi un campo calcolato.

   Per informazioni sulla creazione di un modulo personalizzato e sull&#39;aggiunta di campi calcolati, vedere gli articoli seguenti:

   * [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Aggiungere campi calcolati a un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Copia e incolla il seguente codice in modalità testo nel campo **Calcolo** del modulo personalizzato:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Nei calcoli dei campi personalizzati viene fatta distinzione tra maiuscole e minuscole.

1. Fai clic su **Fine**, quindi su **Salva + Chiudi**.

   Il manager dell’utente che ha creato il problema viene visualizzato nel campo calcolato quando il modulo che contiene il campo viene allegato a un problema.
