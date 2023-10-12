---
title: Miglioramenti per gli amministratori del quarto trimestre 2023
description: Miglioramenti per gli amministratori del quarto trimestre 2023
author: Lisa
feature: Product Announcements
source-git-commit: 8488cb46b3dd9b377c59121597db5b6fe784fdab
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Miglioramenti per gli amministratori del quarto trimestre 2023

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione del quarto trimestre 2023 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione con la versione 23.10.

Per un elenco di tutte le modifiche disponibili a questo punto nel ciclo di rilascio del quarto trimestre del 2023, consulta [Panoramica sulla versione del quarto trimestre 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## I campi calcolati nei moduli personalizzati ora possono utilizzare il carattere jolly $$USER

Il `$$USER` il carattere jolly è ora disponibile nei campi personalizzati calcolati e nei campi di ricerca esterni nel nuovo progettista di moduli. Con riferimento `$$USER` in un calcolo aggiunge l’ID dell’utente corrente. È inoltre possibile utilizzare il carattere jolly con un altro campo. Ad esempio: `$$USER.{name}` aggiungerebbe il nome dell’utente corrente.

Per ulteriori informazioni sui campi calcolati, vedi [Aggiungere campi calcolati con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Aggiungere opzioni di valore da un’API esterna a un modulo personalizzato

Un nuovo tipo di campo, **Ricerca esterna**, è ora disponibile nel designer del modulo personalizzato. Quando i dati sono memorizzati su un sistema esterno, questo tipo di campo ti consente di caricare opzioni da un’API esterna e di filtrare in base ad altri valori di campo nel modulo personalizzato.

Quando il modulo viene aggiunto a un oggetto, i valori restituiti dall’API vengono visualizzati in un campo a discesa e l’utente può selezionarne uno.

>[!NOTE]
>
>Il nuovo **Ricerca esterna** il tipo di campo non è disponibile nel generatore di moduli legacy.

Per ulteriori informazioni, consulta [Progettare un modulo con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
