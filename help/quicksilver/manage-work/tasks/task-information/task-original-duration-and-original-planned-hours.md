---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica dell'attività Durata originale e Orari pianificati originali
description: Come parte della pianificazione di un progetto, è necessario determinare i valori per le ore pianificate e per la durata (o durata pianificata) di ogni attività del progetto.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 1%

---

# Panoramica dell&#39;attività Durata originale e Orari pianificati originali

Come parte della pianificazione di un progetto, è necessario determinare i valori per le ore pianificate e per la durata (o durata pianificata) di ogni attività del progetto.

Per ulteriori informazioni sulle ore pianificate per le attività, vedere [Panoramica sull’orario pianificato](../../../manage-work/tasks/task-information/planned-hours.md).

Per ulteriori informazioni sulla durata dell&#39;attività, vedere [Panoramica del tipo di durata e durata dell’attività](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

È possibile visualizzare questi valori nella scheda Dettagli attività o durante la modifica di un&#39;attività.

Se si crea una visualizzazione per un elenco di attività o un rapporto di attività, è possibile visualizzare anche i campi Orario pianificato originale e Durata originale per le attività.

## Lavoro Necessario Originale

Le ore pianificate originali di un&#39;attività rappresentano il numero di ore pianificate che un&#39;attività aveva in origine prima che diventasse un&#39;attività padre. Quando un&#39;attività diventa un&#39;attività padre, le ore pianificate delle attività figlio vengono riportate all&#39;attività padre per indicare le ore pianificate dell&#39;attività padre.

Visualizzazione del campo Orari pianificati originali in un rapporto di attività o in un elenco è possibile visualizzare il numero originale di Ore pianificate prima che l&#39;attività abbia ereditato il numero di Ore pianificate dei relativi figli.

>[!NOTE]
>
>Quando si crea un&#39;attività, il numero di ore pianificate originali è zero. Se l&#39;attività diventa un&#39;attività padre, il valore di questo campo viene compilato con il numero di ore pianificate dell&#39;attività prima che sia stato modificato in padre. Questo valore rimane in questo campo anche quando l’attività torna ad essere un’attività autonoma.

## Durata Originale

La Durata originale di un&#39;attività è la Durata in minuti di un&#39;attività originariamente prima che questa diventasse un&#39;attività principale. Quando un&#39;attività diventa un&#39;attività padre, la durata tra la data di inizio pianificata del primo figlio e la data di completamento pianificata dell&#39;ultimo figlio viene eseguita fino all&#39;attività padre e diventa la durata dell&#39;attività padre. Sostituisce la Durata dell&#39;attività originale.

Visualizzazione del campo Durata originale in un report attività o in un elenco è possibile visualizzare il numero originale di giorni per la Durata dell&#39;attività prima che sia stata ereditata la Durata dei relativi figli.

>[!NOTE]
>
>Quando si crea un&#39;attività, la Durata originale è pari a zero. Se l&#39;attività diventa un&#39;attività padre, il valore di questo campo viene compilato con la Durata dell&#39;attività prima che sia stato modificato in padre. Questo valore rimane in questo campo anche quando l’attività torna ad essere un’attività autonoma. Questo valore viene visualizzato in minuti.

## Esempio

Ad esempio, quando due attività sono attività autonome, la durata originale e l&#39;ora originale pianificata sono pari a zero.

![original_scheduled_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

Quando la prima attività diventa l&#39;elemento padre della seconda attività, i campi Durata originale e Ore pianificate originali vengono compilati con i valori di Durata e Ore pianificate dell&#39;attività prima che diventi padre. La Durata originale viene visualizzata in minuti. La Durata e le Ore Pianificate del bambino diventano la Durata e le Ore Pianificate del genitore.

![original_and_scheduled_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

Quando l&#39;elemento padre diventa nuovamente un&#39;attività autonoma, la Durata e le Ore pianificate vengono ripristinate ai valori originali, mentre la Durata originale e le Ore pianificate originali rimangono popolate. Non tornano a zero.

![original_duration_and_scheduled_hours_after_reverse_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
