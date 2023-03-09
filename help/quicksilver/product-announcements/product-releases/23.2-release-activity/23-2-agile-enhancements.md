---
title: 23.2 Miglioramenti di Agile
description: 23.2 Miglioramenti di Agile
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: d9fa1c876f2b789c3c387387964ba749c5453a1e
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# 23.2 Miglioramenti di Agile

Questa pagina descrive tutti i miglioramenti agili apportati con la versione 23.2 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione con la versione 23.2.

Per un elenco di tutte le modifiche disponibili a questo punto del ciclo di rilascio 23.2, consulta [Panoramica sulla versione 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Aggiungere attività e problemi alle bacheche Workfront da elenchi e rapporti

Ora è possibile aggiungere attività o problemi esistenti a una bacheca Workfront direttamente da una vista a elenco o report. Tutti gli elementi aggiunti alla bacheca diventeranno schede collegate.

Inoltre, il campo Bacheche è ora disponibile per l’aggiunta agli elenchi e ai rapporti relativi alle attività o ai problemi. Questo campo visualizza tutte le bacheche a cui è stata aggiunta un’attività o un problema.

Per ulteriori informazioni, consulta [Aggiungere attività o problemi esistenti a una bacheca](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## Registra le ore sulle schede collegate su una bacheca

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Ora è possibile registrare le ore sulle schede collegate, come si farebbe su un&#39;attività o un problema. Per registrare l’ora, è necessario disporre delle autorizzazioni corrette per l’attività o il problema.

Per impostazione predefinita, i campi di registrazione ora non vengono visualizzati sulle schede collegate. Devi abilitare **Ore** nell’area Configura in Schede.

Per ulteriori informazioni, consulta [Utilizzare le schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Personalizzare la visualizzazione dei campi su una scheda

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.


È ora disponibile la personalizzazione per configurare quali campi visualizzare su una scheda, sia nella visualizzazione completa quando la scheda è aperta che nella visualizzazione ridotta sulla scheda. Quando si disattiva, un campo non viene visualizzato in nessuna delle due visualizzazioni. È inoltre possibile attivare un campo nella visualizzazione completa e nasconderlo dalla visualizzazione ridotta.

Per ulteriori informazioni, consulta [Personalizzare i campi visualizzati su una scheda](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3415710/){target=_blank}

## Definisci uno stato predefinito per le schede spostate in una colonna della bacheca

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Ora puoi impostare uno stato predefinito da applicare alle schede spostate in una colonna specifica, selezionando uno stato personalizzato e uno stato di sistema nei criteri delle colonne. Quando sposti una scheda nella colonna, Workfront tenta prima di applicare lo stato personalizzato (ad esempio, In attesa di feedback). Se lo stato personalizzato non è disponibile per tale scheda, Workfront applicherà invece lo stato del sistema (ad esempio, In sospeso). Inoltre, se lo stato dell’attività o del problema connesso viene modificato nello stato personalizzato o di sistema impostato nella policy di colonna, la scheda viene automaticamente spostata nella colonna.

In precedenza, veniva richiesto di selezionare uno stato per ogni scheda spostata nella colonna, se erano disponibili più stati.

Per ulteriori informazioni, consulta [Gestisci colonne](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3415711/){target=_blank}

## Le raccolte sono ora disponibili nelle bacheche di Adobe Workfront

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Ora puoi creare raccolte nel dashboard delle bacheche. Una raccolta è un gruppo di bacheche per la collaborazione sul lavoro. Dopo aver denominato la raccolta, puoi aggiungere bacheche alla raccolta utilizzando un set di modelli che offrono impostazioni predefinite, ad esempio i nomi delle colonne. Puoi anche spostare le bacheche autonome in una raccolta. Una volta che una bacheca è in una raccolta, può essere spostata in un’altra raccolta ma non può diventare una bacheca autonoma.

L&#39;aggiunta di membri a una raccolta funziona come l&#39;aggiunta di membri a una bacheca. Una persona o un team deve essere un membro della raccolta prima di poter essere aggiunto come membri a una bacheca della raccolta.

Per ulteriori informazioni, consulta [Gestione raccolte](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[Visualizza una dimostrazione video di questa funzione](https://video.tv.adobe.com/v/3415609/){target=_blank}

## Il campo Stima sulle schede collegate viene mappato sul campo Punti storia sugli oggetti Workfront

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Il campo Stima sulle schede collegate in Bacheche Workfront ora viene mappato sul campo Story Points (Punti storia) per l’oggetto Workfront associato.

Il nuovo campo Story Points (Punti storia) è un campo libero modificabile che puoi aggiungere a una visualizzazione in un elenco o in un rapporto per attività o problemi. Non è legato alle ore pianificate o alle assegnazioni del team.

In precedenza, la stima della scheda era una voce manuale e non veniva mappata su alcun campo di un’attività o di un problema.

Inoltre, il campo Stima sia sulle schede ad hoc che su quelle connesse non ha più un limite di caratteri. In precedenza, il numero massimo di caratteri era 99.

Per ulteriori informazioni, consulta [Utilizzare le schede collegate sulle bacheche](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Scheda di anteprima nella colonna Acquisizione

>[!NOTE]
>
>Questa funzione è disponibile solo tramite la funzionalità opt-in anticipato per le schede madri Workfront.

Ora puoi fare clic su una scheda collegata nella colonna Acquisizione per visualizzare una versione di sola visualizzazione del suo contenuto. Non puoi modificare il contenuto della scheda finché questa non viene spostata fuori dalla colonna di acquisizione in un’altra colonna sulla bacheca.
