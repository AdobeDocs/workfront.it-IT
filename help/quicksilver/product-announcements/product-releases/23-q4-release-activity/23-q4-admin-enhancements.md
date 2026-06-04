---
title: Miglioramenti per gli amministratori del quarto trimestre 2023
description: Miglioramenti per gli amministratori del quarto trimestre 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
TQID: https://experienceleague.adobe.com/6-hscCn7M4UgFBhZVCsugo-ulyuFVc4nyBKKVNN3ZiM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 317
ht-degree: 0%

---

# Miglioramenti per gli amministratori del quarto trimestre 2023

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione del quarto trimestre 2023 all’ambiente di anteprima. Questi miglioramenti sono stati resi disponibili nell’ambiente di produzione con la versione 23.10.

Per un elenco di tutte le modifiche disponibili in questo momento nel ciclo di rilascio del quarto trimestre 2023, consulta [Panoramica sulla versione del quarto trimestre 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Decisioni relative a bozze e documenti disponibili per i clienti dei modelli di licenza legacy

I clienti legacy che non hanno ancora effettuato la transizione al nuovo modello di licenza Adobe Workfront ora possono visualizzare in un unico rapporto i dati con il numero di decisioni in merito a bozze/documenti per utente al mese. Questi dati sono disponibili quando si esegue un rapporto Decisioni utenti.

Per ulteriori informazioni, vedere [Comprendere gli oggetti in Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) e [Visualizzare il numero di decisioni relative a bozze e documenti per tutti gli utenti](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## I campi calcolati nei moduli personalizzati ora possono utilizzare il carattere jolly $$USER

Il carattere jolly `$$USER` è ora disponibile nei campi personalizzati calcolati e nei campi di ricerca esterni nel nuovo progettista di moduli. Il riferimento a `$$USER` in un calcolo aggiunge l&#39;ID dell&#39;utente corrente. È inoltre possibile utilizzare il carattere jolly con un altro campo. `$$USER.{name}`, ad esempio, aggiungerebbe il nome dell&#39;utente corrente.

Per ulteriori informazioni sui campi calcolati, vedere [Aggiungere campi calcolati con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Aggiungere opzioni di valore da un’API esterna a un modulo personalizzato

Un nuovo tipo di campo, **Ricerca esterna**, è ora disponibile nella finestra di progettazione del modulo personalizzato. Quando i dati sono memorizzati su un sistema esterno, questo tipo di campo ti consente di caricare opzioni da un’API esterna e di filtrare in base ad altri valori di campo nel modulo personalizzato.

Quando il modulo viene aggiunto a un oggetto, i valori restituiti dall’API vengono visualizzati in un campo a discesa e l’utente può selezionarne uno.

>[!NOTE]
>
>Il nuovo tipo di campo **Ricerca esterna** non è disponibile nel generatore di moduli legacy.

Per ulteriori informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
