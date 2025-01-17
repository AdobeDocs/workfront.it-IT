---
title: Miglioramenti per gli amministratori del primo trimestre 2025
description: Miglioramenti per gli amministratori del primo trimestre 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Miglioramenti per gli amministratori del primo trimestre 2025

Questa pagina descrive tutti i miglioramenti per gli amministratori apportati con la versione del primo trimestre 2025 all’ambiente di anteprima. Questi miglioramenti saranno resi disponibili nell’ambiente di produzione come indicato.

Per un elenco di tutte le modifiche disponibili al momento nel ciclo di rilascio del primo trimestre 2025, consulta [Panoramica sulla versione del primo trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

## Le regole business sono ora supportate per più oggetti

>[!NOTE]
>
>Versione di anteprima: 16 gennaio 2025; versione di produzione per tutti i clienti: con la versione 25.1 (gennaio 2025)
>
>_Disponibile solo per le organizzazioni nel piano Ultimate._

È ora possibile creare regole business e applicare la convalida a questi oggetti aggiuntivi: Società, Iterazione, Categoria risorsa non manodopera, Ruolo, Utente, Assegnazione, Pool di risorse, Indisponibilità, Documento e Ora.

I seguenti oggetti erano già supportati per le regole business: Progetto, Attività, Richiesta, Portfolio, Programma, Spesa, Record fatturazione, Gruppo, Rischio e Scheda tariffa.

Per ulteriori informazioni, vedere [Creare e modificare le regole business](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Confrontare gli oggetti tra ambienti diversi per la promozione dell’ambiente

>[!NOTE]
>
>Versione di anteprima: 6 gennaio 2025; versione di produzione per tutti i clienti: con la versione 25.1 (gennaio 2025)

Per determinare più facilmente quale oggetto deve essere incluso in un pacchetto di promozione dell’ambiente, è stata aggiunta la possibilità di confrontare oggetti tra ambienti diversi. Ora è possibile selezionare tipi di oggetto e ambienti. Workfront genera un elenco di oggetti di quel tipo, se sono presenti nell’ambiente di destinazione e se tale oggetto presenta differenze tra l’ambiente di origine e l’ambiente di destinazione. È quindi possibile aggiungere oggetti a un pacchetto direttamente da questo elenco.

In precedenza, per confrontare gli oggetti tra ambienti diversi, l’utente doveva sottoporli a controllo manuale.

Per ulteriori informazioni, vedere [Confrontare gli oggetti tra ambienti](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).

## Altri oggetti disponibili per la promozione dell’ambiente

>[!NOTE]
>
>Versione di anteprima: 6 gennaio 2025; versione di produzione per tutti i clienti: con la versione 25.1 (gennaio 2025)

Per espandere le funzionalità di promozione dell’ambiente, sono stati aggiunti altri oggetti. Ora è possibile aggiungere i seguenti oggetti a un pacchetto di promozione dell’ambiente:

* Posizioni
* Schede tariffa
* Assegnazioni

In precedenza, questi oggetti non erano disponibili per la promozione dell’ambiente.

Per ulteriori informazioni sugli oggetti disponibili per la promozione dell&#39;ambiente, vedere [Oggetti supportati per la promozione dell&#39;ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) nell&#39;articolo Panoramica sulla promozione dell&#39;ambiente.

## Impedisci lo spostamento delle attività quando sono presenti ore registrate

>[!NOTE]
>
>Versione di anteprima: 19 dicembre 2024; versione di produzione per tutti i clienti: con la versione 25.1 (16 gennaio 2025)

Poiché lo spostamento di attività o problemi che hanno registrato ore può talvolta causare problemi di conformità o di controllo, nell’area Preferenze attività e problemi di Configura è stata aggiunta una preferenza che consente di impedire agli utenti di spostare attività e problemi se sono presenti ore registrate. Prima di questo miglioramento, gli utenti potevano spostare attività e problemi in altri progetti, anche se avevano effettuato l’accesso in ore.

Per informazioni, consulta [Configurare le preferenze per attività e problemi a livello di sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Preferenza per l&#39;utilizzo della pianificazione del progetto o dell&#39;utente per le attività a assegnazione singola

>[!NOTE]
>
>Versione di anteprima: 21 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (16 gennaio 2025)

In qualità di amministratore di sistema o di gruppo, è ora disponibile una nuova preferenza per indicare se Workfront deve utilizzare la pianificazione del progetto o quella dell&#39;utente per calcolare la sequenza temporale del progetto quando si assegna un utente a un&#39;attività e sia il progetto che l&#39;utente sono associati a una pianificazione. Prima di questo miglioramento, questa impostazione esisteva per le assegnazioni a più utenti. L’impostazione è ora disponibile per le assegnazioni di attività per singolo utente.

Per ulteriori informazioni, vedere [Configurare le preferenze di progetto a livello di sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Le regole business ora supportano i collegamenti ipertestuali

>[!NOTE]
>
>Versione di anteprima: 21 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (16 gennaio 2025)

È ora possibile includere collegamenti ipertestuali nel messaggio di errore personalizzato di una regola business, per guidare l’utente nella modifica della propria azione all’interno del vincolo della regola. L’URL statico potrebbe contenere un collegamento alla documentazione o ad altre pagine utili per l’utente.

Per informazioni, vedere [Creare e modificare le regole business](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## È ora disponibile il filtro per i campi nativi typeahead

>[!NOTE]
>
>Versione di anteprima: 21 novembre 2024; produzione per rilascio rapido: con la versione 24.12 (12 dicembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (16 gennaio 2025)

Quando si aggiunge un riferimento a un campo nativo in un modulo personalizzato che fa riferimento a un campo typeahead, ad esempio Portfolio, Società o Proprietario, è ora disponibile un&#39;opzione di filtro. Il filtro consente di limitare gli oggetti che gli utenti possono scegliere quando utilizzano il campo. Questo filtro personalizzato funziona come un filtro in un campo typeahead personalizzato, utilizzando la modalità testo per definire il filtro.

Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Icona &quot;Sposta in&quot; aggiunta ai campi personalizzati

>[!NOTE]
>
>Versione di anteprima: 29 ottobre 2024; produzione per rilascio rapido: con la versione 24.11 (14 novembre 2024); produzione per rilascio trimestrale: con la versione 25.1 (16 gennaio 2025)

Quando un modulo personalizzato contiene più sezioni con molti campi, può essere difficile spostare un campo da una sezione all’altra trascinandolo. A ciascun campo è stata aggiunta l’icona &quot;sposta in&quot;, che consente di selezionare la sezione in cui inserire il campo.

Per ulteriori informazioni, vedere [Organizzazione e anteprima di un modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
