---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato con il generatore di moduli legacy
description: È possibile utilizzare lo stesso campo personalizzato calcolato nei moduli personalizzati che appartengono a oggetti diversi. È ad esempio possibile utilizzare il campo calcolato Profitto creato per il modulo personalizzato del progetto in un modulo personalizzato per le attività.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 24482fca-94e4-406d-9d62-3db9f51481e6
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Riutilizzare un campo personalizzato calcolato esistente in un modulo personalizzato con il generatore di moduli legacy

È possibile utilizzare lo stesso campo personalizzato calcolato nei moduli personalizzati che appartengono a oggetti diversi. È ad esempio possibile utilizzare il campo calcolato Profitto creato per il modulo personalizzato del progetto in un modulo personalizzato per le attività.

Per informazioni sull’aggiunta di un campo personalizzato calcolato a un modulo personalizzato, consulta [Aggiungere dati calcolati a un modulo personalizzato con il generatore di moduli legacy](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Quando si utilizza un campo personalizzato calcolato esistente, il calcolo non viene trasferito nel nuovo modulo. È necessario aggiungere nuovamente il calcolo nello stesso campo del nuovo modulo personalizzato.

>[!TIP]
>
>Ciò si verifica quando si utilizzano i calcoli memorizzati nel **Istruzioni** del modulo personalizzato.

È inoltre possibile avere un calcolo diverso per lo stesso campo nel nuovo modulo. Mantenere lo stesso nome per il campo personalizzato calcolato garantisce coerenza e uniformità nella convenzione di denominazione.

>[!IMPORTANT]
>
>I campi personalizzati calcolati possono non essere più aggiornati nel tempo. Per essere certi di visualizzare sempre il calcolo aggiornato in questi campi, effettuare una delle seguenti operazioni:
>
>* Dopo aver salvato un oggetto in cui sono stati modificati dati in un modulo personalizzato allegato, fare clic sull&#39;icona Altro ![](assets/more-icon.png) nella pagina principale dell&#39;oggetto, quindi Ricalcola espressioni personalizzate.
>* Selezionare l&#39;opzione Ricalcola espressioni personalizzate quando si modificano oggetti in blocco.
>* Selezionare l&#39;opzione Aggiorna calcoli precedenti durante la modifica di un campo personalizzato calcolato in un modulo personalizzato.
>
