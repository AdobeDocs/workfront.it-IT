---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configura effetto sulle ore in cui un oggetto viene eliminato e ripristinato
description: Puoi configurare cosa succede alle ore quando qualcuno elimina un progetto, un’attività o un problema per il quale sono state registrate le ore. L’opzione scelta determina anche cosa accade alle ore se il progetto, l’attività o il problema viene ripristinato in un secondo momento. Per ulteriori informazioni sul ripristino degli elementi in Workfront, vedere Ripristinare gli elementi eliminati.
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 1%

---

# Configura l&#39;effetto sulle ore di eliminazione e ripristino di un oggetto

Puoi configurare cosa succede alle ore quando qualcuno elimina un progetto, un’attività o un problema per il quale sono state registrate le ore. L’opzione scelta determina anche cosa accade alle ore se il progetto, l’attività o il problema viene ripristinato in un secondo momento. Per ulteriori informazioni sul ripristino di elementi in Workfront, vedere [Ripristinare gli elementi eliminati](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di Sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare la modalità di gestione delle ore quando un elemento viene eliminato e ripristinato

{{step-1-to-setup}}

1. Espandi **Schede orario e ore**, quindi fai clic su **Preferenze**.

1. Individua la sezione **Preferenze eliminazione progetto, attività o problema**.
1. (Condizionale) Per configurare la gestione delle ore quando un progetto viene eliminato, selezionare una delle opzioni seguenti nella sezione **Durante l&#39;eliminazione dei progetti**:

   * Mantieni le ore registrate già aggiunte alle schede orario come ore generali (se il progetto viene ripristinato in un secondo momento, le ore rimangono nella scheda orario)\
     Questa opzione è selezionata per impostazione predefinita.
   * Elimina le ore registrate (se il progetto viene ripristinato in un secondo momento, le ore registrate vengono ripristinate nel progetto)

1. (Condizionale) Per configurare la gestione delle ore quando un&#39;attività o un problema viene eliminato, selezionare una delle opzioni seguenti nella sezione **Per l&#39;eliminazione di attività o problemi**:

   * Sposta le ore registrate nel progetto in cui si trova l’attività o il problema (se l’attività o il problema viene ripristinato in un secondo momento, le ore rimangono sul progetto)\
     Questa opzione è selezionata per impostazione predefinita.
   * Elimina le ore registrate (se l&#39;attività o il problema viene ripristinato in un secondo momento, le ore registrate vengono ripristinate nell&#39;attività o nel problema)

1. Fai clic su **Salva**.
