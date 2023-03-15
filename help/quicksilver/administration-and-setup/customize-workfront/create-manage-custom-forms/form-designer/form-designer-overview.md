---
title: Panoramica della finestra di progettazione dei moduli
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: È possibile progettare un modulo personalizzato che gli utenti possono allegare a un oggetto Workfront. Gli utenti che lavorano all’oggetto possono compilare il modulo personalizzato per fornire informazioni sull’oggetto.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 9b32c41c9f2971f3b0bbded230680677cc0b3c64
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 1%

---

# Panoramica della finestra di progettazione dei moduli

{{highlighted-preview-article-level}}

È possibile utilizzare la nuova struttura del modulo per progettare un modulo personalizzato che gli utenti possono allegare a un oggetto Workfront. Gli utenti che lavorano all’oggetto possono compilare il modulo personalizzato per fornire informazioni sull’oggetto.

Il nuovo form designer dispone di una nuova area di lavoro in stile area di lavoro che consente di visualizzare contemporaneamente i campi, l’area di lavoro e le impostazioni dei campi. Consente inoltre di trascinare i campi all’interno delle sezioni durante la progettazione del modulo.

<!-- add screenshot when field settings empty state is ready -->

## Accesso al nuovo form designer

È disponibile un nuovo pulsante nella parte superiore sia del nuovo form designer che del precedente form builder. È possibile utilizzare questo pulsante per passare dal generatore legacy al nuovo designer.

![](assets/switch-views.png)

## Nuove funzionalità disponibili con la struttura del modulo

Con il nuovo form designer, abbiamo aggiunto la possibilità di

* **Copiare un campo**: È ora possibile copiare i campi esistenti facendo clic sull’icona Copia sui campi direttamente dall’area di lavoro.

* **Modificare le dimensioni del testo descrittivo**: È ora possibile assegnare dimensioni piccole, medie o grandi ai campi di testo descrittivi. È inoltre possibile utilizzarli sulla stessa riga con altri campi.

* **Utilizzare una sezione predefinita**: Se l’autore del modulo non ha aggiunto una sezione nella parte superiore del modulo, nell’area di lavoro è ora visibile una sezione Predefinito, che consente agli utenti di modificare le autorizzazioni per i campi a cui non è stata assegnata alcuna sezione personalizzata.

   >[!NOTE]
   >
   >La sezione predefinita non è visibile all’interno degli oggetti una volta che il modulo è associato all’oggetto.

## Funzionalità disponibili a breve

Al momento non sono disponibili nella finestra di progettazione dei moduli, ma verranno aggiunti a breve:

* Regolare le dimensioni del testo descrittivo

* Visualizza/Ignora logica

* Filtro per campi di tipo precedente

>[!IMPORTANT]
>
>Le configurazioni esistenti per i filtri logici e per la generazione di caratteri non saranno influenzate quando si lavora con la nuova struttura del modulo.

## Funzionalità rimosse dalla struttura del modulo

Sono state rimosse le seguenti funzionalità dalla finestra di progettazione dei moduli:


* Impostazioni modulo, Condivisione modulo, schede Condivisione campi

   * Le impostazioni del modulo sono ora disponibili nella parte superiore dell’area di lavoro

   * Scheda principale Condivisione moduli e scheda secondaria Condivisione campi
   >[!NOTE]
   >
   >Puoi controllare la condivisione del modulo e del campo da Configurazione > Forms personalizzato > Forms o scheda Campi.

* Traccia le modifiche dei campi nei feed di aggiornamento
   >[!NOTE]
   >
   >Puoi trovarlo in Configurazione > Interfaccia > Aggiorna feed
