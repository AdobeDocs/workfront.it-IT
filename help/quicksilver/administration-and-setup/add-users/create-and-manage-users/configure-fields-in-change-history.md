---
user-type: administrator
product-area: system-administration;setup
title: Configurare i campi da tenere traccia nella cronologia modifiche
description: In qualità di amministratore di Workfront, puoi configurare quali campi oggetto e azioni tenere traccia di Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 9%

---

# Configurare i campi da tenere traccia della cronologia delle modifiche

{{highlighted-preview-article-level}}

Adobe Workfront genera aggiornamenti automatici di sistema per registrare i seguenti eventi:

* Modifiche apportate dagli utenti in un campo oggetto
* Azioni eseguite dagli utenti su un oggetto

Questi aggiornamenti di sistema includono i seguenti tipi di informazioni:

* La modifica apportata
* Nome dell&#39;utente che ha apportato la modifica
* Ora e data della modifica

In qualità di amministratore di Workfront, puoi configurare quali campi oggetto e azioni tenere traccia di Workfront.

Workfront, ad esempio, può tenere traccia di tutte le modifiche apportate dagli utenti ai nomi dei problemi all&#39;interno del sistema. Qualsiasi modifica del nome del problema viene quindi visualizzata come una voce nel registro della cronologia delle modifiche. Per ulteriori informazioni, vedere [Visualizzare e gestire la cronologia modifiche](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di sistema</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limiti al tracciamento dei campi

I limiti per il numero di campi che è possibile monitorare sono definiti dal pacchetto Workfront.

| Pacchetto Workfront | Numero massimo di campi tracciati |
|---------|----------|
| Seleziona | 700 |
| Prime | 3000 |
| Ultimate | 5000 |
| Selezione flusso di lavoro | 1000 |
| Flusso di lavoro Prime | 5000 |
| Flusso di lavoro Ultimate | Senza limiti |

## Aggiungi i campi di cui vuoi tenere traccia

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Tracciamento modifiche > Configurazione**.
1. Nella schermata Configurazione, fare clic su **Aggiungi campo**.
1. Nella casella **Aggiungi campi** selezionare un oggetto. È possibile iniziare a digitare il nome dell&#39;oggetto, quindi selezionarlo quando viene visualizzato nell&#39;elenco.
1. Quindi, selezionare i nomi dei campi di cui si desidera tenere traccia per l&#39;oggetto. È possibile iniziare a digitare il nome del campo, quindi selezionarlo quando viene visualizzato nell&#39;elenco.

   Per l’oggetto sono disponibili sia campi personalizzati che campi nativi.
   I campi già tracciati vengono visualizzati come selezionati nell’elenco.

   ![Aggiungi campi per rilevamento modifiche](assets/change-history-config-add-fields.png)

1. Dopo aver selezionato tutti i campi da monitorare, fai clic su **Aggiungi**.

   I campi vengono aggiunti all&#39;elenco Campi tracciati.

## Rimuovi i campi che non desideri più tracciare

È possibile rimuovere i campi di cui non si desidera tenere traccia per un particolare tipo di oggetto nell&#39;interfaccia di Workfront.

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su **Tracciamento modifiche > Configurazione**.
1. Nella schermata Configuration, seleziona il campo o i campi che desideri interrompere il tracciamento.

   È possibile che lo stesso nome di campo venga visualizzato più volte. I campi sono raggruppati per oggetto, in modo da poter individuare il campo corretto. Puoi anche utilizzare la casella di ricerca nella parte superiore dello schermo.

1. Seleziona **Elimina** nella barra delle azioni nella parte inferiore dello schermo.
1. Fai clic su **Rimuovi** nel messaggio di conferma.

   I campi vengono rimossi dall&#39;elenco Campi tracciati.


