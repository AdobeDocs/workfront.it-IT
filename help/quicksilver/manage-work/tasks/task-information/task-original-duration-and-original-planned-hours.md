---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Panoramica della durata originale e delle ore pianificate originali dell'attività
description: Durante la pianificazione di un progetto, è necessario determinare i valori per le ore pianificate e per la durata (o durata pianificata) di ogni attività del progetto.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 1%

---

# Panoramica della durata originale e delle ore pianificate originali dell&#39;attività

Durante la pianificazione di un progetto, è necessario determinare i valori per le ore pianificate e per la durata (o durata pianificata) di ogni attività del progetto.

Per ulteriori informazioni sulle ore pianificate per le attività, vedi [Panoramica sulle ore pianificate](../../../manage-work/tasks/task-information/planned-hours.md).

Per ulteriori informazioni sulla durata dell&#39;attività, vedere [Panoramica sulla durata dell&#39;attività e sul tipo di durata](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

È possibile visualizzare questi valori nella scheda Dettagli attività o durante la modifica di un&#39;attività.

Se si crea una visualizzazione per un elenco di attività o un report di attività, è possibile visualizzare anche i campi Ore pianificate originali e Durata originale per le attività.

## Ore pianificate originali

Le ore pianificate originali di un&#39;attività rappresentano il numero di ore pianificate che un&#39;attività aveva in origine prima di diventare un&#39;attività padre. Quando un&#39;attività diventa un&#39;attività padre, le ore pianificate delle attività figlio vengono riportate all&#39;attività padre per indicare le ore pianificate dell&#39;attività padre.

Visualizzazione del campo Ore pianificate originali in un report o elenco di attività È possibile visualizzare il numero originale di ore pianificate prima che l&#39;attività ereditasse il numero di ore pianificate dei relativi figli.

>[!NOTE]
>
>Quando si crea un&#39;attività, il numero di ore pianificate originali è zero. Se l&#39;attività diventa un&#39;attività padre, il valore di questo campo viene popolato con il numero delle ore pianificate dell&#39;attività prima che fosse trasformata in padre. Questo valore rimane in questo campo anche quando l’attività torna a essere autonoma.

## Durata Originale

La durata originale di un&#39;attività è la durata che un&#39;attività aveva prima di diventare un&#39;attività padre, espressa in minuti. Quando un&#39;attività diventa padre, la durata tra la data di inizio pianificata del primo figlio e la data di completamento pianificata dell&#39;ultimo figlio viene aggregata all&#39;attività padre e diventa la durata dell&#39;attività padre. Questo sostituisce la Durata dell&#39;attività originale.

Visualizzazione del campo Durata originale in un report o in un elenco delle attività È possibile visualizzare il numero originale di giorni per la Durata dell&#39;attività prima che ereditasse la Durata dei relativi figli.

>[!NOTE]
>
>Quando si crea un&#39;attività, la Durata originale è uguale a zero. Se l&#39;attività diventa un&#39;attività padre, il valore di questo campo viene popolato con la Durata dell&#39;attività prima che fosse trasformata in attività padre. Questo valore rimane in questo campo anche quando l’attività torna a essere autonoma. Questo valore viene visualizzato in minuti.

## Esempio

Se ad esempio due attività sono attività autonome, la durata originale e le ore pianificate originali sono pari a zero.

![original_planned_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

Quando la prima attività diventa padre della seconda attività, nei campi Durata originale e Ore pianificate originali vengono inseriti i valori per la Durata e le Ore pianificate dell&#39;attività prima che diventi padre. La Durata originale viene visualizzata in minuti. La Durata e le Ore pianificate del figlio diventano la Durata e le Ore pianificate del padre.

![ore_pianificate_e_originali_con_un_task_padre.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

Quando l&#39;attività padre diventa di nuovo un&#39;attività autonoma, la Durata e le Ore pianificate tornano ai valori originali, mentre la Durata originale e le Ore pianificate originali rimangono popolate. Non tornano a zero.

![original_duration_and_scheduled_hours_after_reversal_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
