---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Esempio di campo personalizzato calcolato: visualizza il manager dell’autore di un problema sul modulo personalizzato relativo al problema'
description: Utilizzando un campo personalizzato calcolato, è possibile visualizzare il nome del responsabile dell’autore di un problema in un modulo personalizzato allegato al problema. Utilizzando la stessa istruzione, è possibile creare campi calcolati simili per progetti, problemi e altri oggetti.
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '334'
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

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Pacchetto Adobe Workfront</p> </td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licenza Adobe Workfront</p> </td> 
   <td>
      <p>Standard</p>
      <p>Piano</p></td>
  </tr> 
  <tr> 
   <td><p>Configurazioni del livello di accesso</p></td> 
   <td> <p>Accesso amministrativo ai moduli personalizzati</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorizzazioni oggetto</p> </td> 
   <td> <p>Contribuire all’accesso all’oggetto in cui è allegato il modulo con l’accesso Modifica modulo personalizzato</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visualizzare il manager dell’autore di un problema nel modulo personalizzato del problema

I passaggi seguenti mostrano come creare un campo calcolato per un modulo personalizzato relativo a un problema in cui è possibile acquisire il nome del manager dell’utente che ha creato il problema. Il processo è identico quando si desidera acquisire il nome del manager di un utente che ha creato un&#39;attività, un progetto o un portfolio, ad esempio.

1. Crea un modulo personalizzato per la segnalazione di un problema e aggiungi un campo calcolato.

   Per informazioni sulla creazione di un modulo personalizzato e sull&#39;aggiunta di campi calcolati, vedere gli articoli seguenti:

   * [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
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
