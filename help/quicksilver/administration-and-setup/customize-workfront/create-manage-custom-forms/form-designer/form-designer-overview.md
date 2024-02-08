---
title: Panoramica di Progettazione moduli
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile progettare un modulo personalizzato che gli utenti possono allegare a un oggetto Workfront. Gli utenti che lavorano sull’oggetto possono compilare il modulo personalizzato per fornire informazioni sull’oggetto.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: e34a0b3bf5e2c4dc794a7d7c85245bb4d11842be
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---

# Panoramica di Progettazione moduli

È possibile utilizzare il nuovo progettista di moduli per progettare un modulo personalizzato che gli utenti possono allegare a un oggetto Workfront. Gli utenti che lavorano sull’oggetto possono compilare il modulo personalizzato per fornire informazioni sull’oggetto.

Il nuovo progettista di moduli dispone di una nuova area di lavoro in stile area di lavoro che consente di visualizzare contemporaneamente i campi, l&#39;area di lavoro e le impostazioni dei campi. Consente inoltre di trascinare i campi all&#39;interno delle sezioni durante la progettazione del modulo.

<!-- add screenshot when field settings empty state is ready -->

## Come accedere al nuovo progettista di moduli

È disponibile un nuovo pulsante nella parte superiore sia del nuovo progettista di moduli che del generatore di moduli legacy. Puoi utilizzare questo pulsante per passare dal generatore legacy al nuovo designer.

![Passa a nuovo progettista modulo](assets/switch-views.png)

## Nuova funzionalità disponibile con il progettista del modulo

Con il nuovo form designer è stata aggiunta la possibilità di:

* **Copiare un campo**: ora puoi copiare i campi esistenti facendo clic sull’icona Copia sui campi direttamente dall’area di lavoro.

* **Modificare le dimensioni per il testo descrittivo**: ora puoi assegnare dimensioni piccole, medie o grandi ai campi Testo descrittivo. È inoltre possibile utilizzarli nella stessa riga con altri campi.

* **Usa una sezione predefinita**: se il creatore del modulo non ha aggiunto una sezione nella parte superiore del modulo, nell’area di lavoro è ora visibile una sezione predefinita che consente agli utenti di regolare le autorizzazioni per i campi ai quali non è assegnata alcuna sezione personalizzata.

  >[!NOTE]
  >
  >La sezione predefinita non è visibile all&#39;interno degli oggetti dopo che il modulo è stato allegato all&#39;oggetto.

## Funzionalità in arrivo

I seguenti elementi non sono attualmente disponibili nel progettista del modulo, ma verranno aggiunti a breve:

* Filtra per campi typeahead

>[!IMPORTANT]
>
>Le configurazioni esistenti per i filtri typeahead non verranno influenzate quando si utilizza il nuovo progettista di moduli.

## Funzionalità rimossa dal progettista del modulo

Sono state rimosse le seguenti funzionalità dall’interno del progettista del modulo:

* Impostazioni modulo, Condivisione modulo, Schede Condivisione campo

   * Le impostazioni del modulo sono ora disponibili nella parte superiore dell’area di lavoro

   * Scheda principale Condivisione modulo e scheda secondaria Condivisione campo

  >[!NOTE]
  >
  >Puoi controllare la condivisione di moduli e campi dall’area Configurazione > Forms personalizzato > Forms o Campi.

* Traccia le modifiche dei campi nei feed di aggiornamento

  >[!NOTE]
  >
  >È possibile trovarlo in Configurazione > Interfaccia > Aggiorna feed
