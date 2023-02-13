---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: La configurazione influisce sulle ore in cui un oggetto viene eliminato e ripristinato
description: È possibile configurare ciò che accade alle ore in cui un utente elimina un progetto, un'attività o un problema a cui sono collegate le ore. L’opzione selezionata determina inoltre cosa accade alle ore se il progetto, l’attività o il problema vengono ripristinati in un secondo momento. (Per ulteriori informazioni sul ripristino di elementi in Workfront, vedere Ripristinare elementi eliminati.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# La configurazione influisce sulle ore in cui un oggetto viene eliminato e ripristinato

È possibile configurare ciò che accade alle ore in cui un utente elimina un progetto, un&#39;attività o un problema a cui sono collegate le ore. L’opzione selezionata determina inoltre cosa accade alle ore se il progetto, l’attività o il problema vengono ripristinati in un secondo momento. (Per ulteriori informazioni sul ripristino di elementi in Workfront, vedi [Ripristina elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configura le ore di gestione quando un elemento viene eliminato e ripristinato

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Espandi **Tempi e ore**, quindi fai clic su **Preferenze**.

1. Individua il **Preferenze di eliminazione di progetti, attività o problemi** sezione .
1. (Condizionale) Per configurare la modalità di gestione delle ore quando un progetto viene eliminato, seleziona una delle seguenti opzioni nella sezione **Eliminazione di progetti** sezione:

   * Mantieni le ore registrate già aggiunte ai fogli presenze come ore generali (se il progetto viene ripristinato in un secondo momento, le ore rimangono nella scheda attività)\
      Questa opzione è selezionata per impostazione predefinita.
   * Elimina le ore registrate (se il progetto viene ripristinato in un secondo momento, le ore registrate vengono ripristinate nel progetto)

1. (Condizionale) Per configurare la modalità di gestione delle ore quando un’attività o un problema viene eliminato, seleziona una delle opzioni seguenti nella **Quando si eliminano attività o problemi** sezione:

   * Sposta le ore registrate nel progetto in cui si trova l’attività o il problema (se l’attività o il problema viene ripristinato in un secondo momento, le ore rimangono nel progetto)\
      Questa opzione è selezionata per impostazione predefinita.
   * Elimina le ore registrate (se l&#39;attività o il problema viene ripristinato in un secondo momento, le ore registrate vengono ripristinate nell&#39;attività o nel problema)

1. Fai clic su **Salva**.
