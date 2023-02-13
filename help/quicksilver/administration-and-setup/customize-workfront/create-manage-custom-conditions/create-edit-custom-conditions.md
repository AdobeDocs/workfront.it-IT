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
source-wordcount: '640'
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
   <td>Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Creare o modificare una condizione personalizzata

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Preferenze del progetto** > **Condizioni**.

1. Fai clic sulla scheda del tipo di oggetto (**Progetto**, **Attività** oppure **Problema**) che si desidera associare alla condizione.

1. Per creare una nuova condizione, fai clic su **Aggiungi una nuova condizione**.

   Oppure

   Per modificare una condizione esistente, passa il puntatore del mouse sulla condizione da modificare, quindi fai clic sul pulsante **Modifica** all’estrema destra.

   ![](assets/custom-condition-edit-nwe.jpg)

1. Configura la condizione personalizzata utilizzando le seguenti opzioni:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nome condizione</td> 
      <td>(Obbligatorio) Immetti un nome descrittivo per la condizione.</td> 
     </tr> 
     <tr> 
      <td>Descrizione</td> 
      <td>(Facoltativo) Immetti una descrizione dello scopo della condizione per gli utenti che la utilizzeranno.</td> 
     </tr> 
     <tr> 
      <td>Clr icn</td> 
      <td>(Facoltativo) Fai clic sull’icona del colore, quindi scegli il colore desiderato per la condizione quando viene visualizzata in progetti, attività o problemi. È inoltre possibile digitare un numero esadecimale.</td> 
     </tr> 
     <tr> 
      <td>Equivale a </td> 
      <td><p>(Obbligatorio, solo per i progetti) Fai clic sull’opzione nell’elenco a discesa che descrive meglio la funzione della nuova condizione. Ad esempio, per una condizione denominata Bene di tracciamento , fai clic su Su Target . Questo determina il funzionamento delle condizioni predefinite. Ogni condizione creata deve corrispondere a una delle opzioni del menu a discesa.</p>
      <p>Per informazioni sulle condizioni predefinite, consulta <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Impostare una condizione personalizzata come predefinita per i progetti</a> e <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Imposta una condizione personalizzata come predefinita per le attività e i problemi</a>.</p>
      <p>Non è possibile modificare questa opzione dopo aver completato la creazione della condizione.</p></td> 
     </tr> 
     <tr> 
      <td>Chiave</td> 
      <td><p>(Obbligatorio) Per una condizione di progetto, digita un’abbreviazione alfanumerica che gli utenti saranno in grado di riconoscere. Per un'attività o una condizione di problema, digitare un codice numerico a due cifre da 01 a 99. </p>
      <p>Questa chiave, utilizzata nell’API e utilizzabile a scopo di reporting, deve essere univoca per ciascun oggetto.</p>
      <p>Non è possibile modificare la chiave di una condizione dopo aver salvato la condizione. </p></td> 
     </tr> 
     <tr> 
      <td>Nascondi condizione</td> 
      <td><p>(Facoltativo) Questa opzione è disponibile per condizioni personalizzate che non desideri più utilizzare, ma che desideri mantenere per motivi storici. </p>
      <p>Se si nasconde una condizione personalizzata utilizzata per gli elementi di lavoro, questa continua a essere visualizzata su tali elementi di lavoro dopo averla nascosta. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >È possibile standardizzare la terminologia e i colori delle condizioni per tutti e tre i tipi di oggetti. A questo scopo, copia la condizione Nome e il codice esadecimale di colore da una scheda (Progetto, Attività, Problema) alla condizione corrispondente nelle altre due schede.

1. (Facoltativo) Trascina ![](assets/move-icon---dots.png) qualsiasi condizione a una nuova posizione per riordinare l’elenco.

   Questo modifica l’ordine in cui vengono visualizzate le condizioni nei progetti, nelle attività e nei problemi:

   * Quando un utente modifica un progetto

      ![](assets/change-condition-edit-project.png)

   * Quando un utente modifica la condizione di un’attività o un problema nella scheda Aggiornamenti:

      ![](assets/change-condition-update-comment.png)

   * Quando un utente modifica la condizione di un&#39;attività o di un problema in una visualizzazione a elenco:

      ![](assets/change-conditions-list-dropdown-only.png)

1. Fai clic su **Salva**.

È possibile impostare la condizione personalizzata come condizione predefinita per i progetti o per le attività e i problemi. Per ulteriori informazioni, consulta [Impostare una condizione personalizzata come predefinita per i progetti](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) e [Imposta una condizione personalizzata come predefinita per le attività e i problemi](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Per ulteriori informazioni sulle condizioni personalizzate, consulta [Condizioni personalizzate](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
