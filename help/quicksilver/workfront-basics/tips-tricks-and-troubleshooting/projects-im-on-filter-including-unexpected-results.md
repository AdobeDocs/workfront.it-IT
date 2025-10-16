---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Il filtro Progetti in corso include risultati imprevisti
description: Leggi questo articolo per risolvere i problemi relativi al filtro Progetti in corso, inclusi i risultati imprevisti.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 3%

---

# Il filtro Progetti in corso include risultati imprevisti

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table>
  <tr>
   <td>Pacchetto Adobe Workfront
   </td>
   <td> <p>PRIME o ULTIMATE</p>
    <p>Flusso di lavoro Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Licenze Adobe Workfront
   </td>
   <td><p>Standard</p>
   <p>Piano</p>
   </td>
  </tr>
   <tr>
   <td>Configurazioni del livello di accesso
   </td>
   <td>Devi essere un amministratore [!DNL Workfront].
   </td>
  </tr>
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Problema

Il filtro [!UICONTROL **Progetti in corso**] include risultati non previsti, in quanto non sono assegnato o associato a tali progetti.

## Soluzione

Il filtro [!UICONTROL **Progetti in corso**] include progetti che contengono l&#39;utente in uno dei campi [!UICONTROL **Dettagli progetto**], inclusi campi facilmente mancanti o compilati automaticamente come [!UICONTROL **Inserito da**] o [!UICONTROL **ID sponsor**]. Per rimuovere i risultati indesiderati, esistono due soluzioni possibili:

1. Controlla [!UICONTROL **Dettagli progetto**] per ogni progetto imprevisto incluso dal filtro e rimuovi il tuo nome da tutti i campi.

   O

1. Prova a utilizzare un filtro simile, ad esempio [!UICONTROL **Progetti di cui sono Proprietario**], che include solo i progetti specificamente assegnati a te.

Per ulteriori informazioni sull&#39;utilizzo dei filtri in [!DNL Workfront], vedere [Panoramica dei filtri](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
