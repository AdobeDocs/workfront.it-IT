---
title: Creare o modificare una condizione personalizzata
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: In qualità di amministratore di Adobe Workfront, puoi creare o modificare una condizione personalizzata per progetti, attività e problemi in base alle esigenze della tua organizzazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 2%

---

# Creare o modificare una condizione personalizzata

In qualità di amministratore di Adobe Workfront, puoi creare o modificare una condizione personalizzata per progetti, attività e problemi in base alle esigenze della tua organizzazione.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Creare o modificare una condizione personalizzata

1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Preferenze progetto** > **Condizioni**.

1. Fare clic sulla scheda del tipo di oggetto (**Progetto**, **Attività** o **Problema**) che si desidera associare alla condizione.

1. Per creare una nuova condizione, fare clic su **Aggiungi una nuova condizione**.

   Oppure

   Per modificare una condizione esistente, passa il cursore del mouse sulla condizione da modificare, quindi fai clic sull&#39;icona **Modifica** visualizzata all&#39;estrema destra.

   ![](assets/custom-condition-edit-nwe.jpg)

1. Configura la condizione personalizzata utilizzando le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nome condizione</td> 
      <td>(Obbligatorio) Digita un nome descrittivo per la condizione.</td> 
     </tr> 
     <tr> 
      <td>Descrizione</td> 
      <td>(Facoltativo) Digitare una descrizione dello scopo della condizione per gli utenti che la utilizzeranno.</td> 
     </tr> 
     <tr> 
      <td>Colore</td> 
      <td>(Facoltativo) Fai clic sull’icona del colore, quindi scegli il colore desiderato per la condizione quando viene visualizzata in progetti, attività o problemi. È inoltre possibile digitare un numero esadecimale.</td> 
     </tr> 
     <tr> 
      <td>Equivale a </td> 
      <td><p>(Obbligatorio, solo per i progetti) Fai clic sull’opzione nell’elenco a discesa che descrive meglio la funzione della nuova condizione. Ad esempio, per una condizione denominata Area di tracciamento, fai clic su Destinazione. Questo determina il funzionamento delle condizioni predefinite. Ogni condizione creata deve corrispondere a una delle opzioni del menu a discesa.</p>
      <p>Per informazioni sulle condizioni predefinite, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Impostare una condizione personalizzata come predefinita per i progetti</a> e <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Impostare una condizione personalizzata come predefinita per attività e problemi</a>.</p>
      <p>Questa opzione non può essere modificata dopo aver completato la creazione della condizione.</p></td> 
     </tr> 
     <tr> 
      <td>Chiave</td> 
      <td><p>(Obbligatorio) Per una condizione di progetto, digita un’abbreviazione alfanumerica che gli utenti saranno in grado di riconoscere. Per un'attività o una condizione di problema, digitare un codice numerico a due cifre compreso tra 01 e 99. </p>
      <p>Questa chiave, che viene utilizzata nell’API e può essere utilizzata a scopo di reporting, deve essere univoca per ciascun oggetto.</p>
      <p>Non è possibile modificare la chiave di una condizione dopo averla salvata. </p></td> 
     </tr> 
     <tr> 
      <td>Nascondi condizione</td> 
      <td><p>(Facoltativo) Questa opzione è disponibile per le condizioni personalizzate che non desideri più utilizzare, ma che desideri mantenere per motivi storici. </p>
      <p>Se si nasconde una condizione personalizzata utilizzata per gli elementi di lavoro, questa continua a essere visualizzata sugli elementi di lavoro dopo essere stata nascosta. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Puoi standardizzare la terminologia e i colori delle condizioni tra tutti e tre i tipi di oggetto. A questo scopo, copia il Nome della condizione e il Codice esadecimale Colore da una scheda (Progetto, Attività, Problema) alla condizione corrispondente nelle altre due schede.

1. (Facoltativo) Trascina ![](assets/move-icon---dots.png) qualsiasi condizione in una nuova posizione per riordinare l&#39;elenco.

   Questo cambia l’ordine in cui vengono visualizzate le condizioni nei progetti, nelle attività e nei problemi:

   * Quando un utente modifica un progetto

     ![](assets/change-condition-edit-project.png)

   * Quando un utente modifica la condizione per un’attività o un problema nella scheda Aggiornamenti:

     ![](assets/change-condition-update-comment.png)

   * Quando un utente modifica la condizione di un’attività o di un problema in una vista a elenco:

     ![](assets/change-conditions-list-dropdown-only.png)

1. Fai clic su **Salva**.

Puoi impostare la condizione personalizzata come condizione predefinita per i progetti o per le attività e i problemi. Per ulteriori informazioni, vedere [Impostare una condizione personalizzata come predefinita per i progetti](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) e [Impostare una condizione personalizzata come predefinita per attività e problemi](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Per ulteriori informazioni sulle condizioni personalizzate, vedere [Condizioni personalizzate](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
