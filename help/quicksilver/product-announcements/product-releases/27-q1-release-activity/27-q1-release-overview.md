---
title: Panoramica sulla versione del primo trimestre 2027
description: Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del primo trimestre 2027. Questi miglioramenti saranno disponibili nell’ambiente di produzione durante tutto il trimestre.
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a8c35fd2f1059bd91de7d6d59db7e447ec6af6a9
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 30%
---

# Panoramica sulla versione del primo trimestre 2027

Questa pagina fornisce informazioni sulle funzionalità incluse nella versione del primo trimestre 2027 pianificata per gennaio 2027.

I miglioramenti in questa pagina sono disponibili nell’ambiente di anteprima. Questa pagina verrà aggiornata con ulteriori miglioramenti man mano che il rilascio del primo trimestre 2027 si avvicina al rilascio pianificato in produzione.

>[!IMPORTANT]
>
>
>Salvo diversa indicazione, i rilasci mensili e trimestrali dovrebbero essere disponibili il giovedì della seconda settimana completa del mese.
>
>| Rilascio mensile | Rilascio trimestrale |
>|----|----|
>| <ul><li>2026.11 (12 novembre 2026)</li><li>2026.12 (17 dicembre 2026)</li><li>2027.01 (21 gennaio 2027)</li></ul> | <ul><li>2027.01 (21 gennaio 2027)</li></ul> |
>
>Per ulteriori informazioni sul processo di rilascio rapido, consulta [Abilitare o disabilitare il processo di rilascio rapido](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Miglioramenti in Adobe Workfront

* [Miglioramenti ai progetti](#project-enhancements)

### Miglioramenti ai progetti

<table>
    <tbody>
        <tr>
            <td><strong>Funzione</strong>
            </td>
            <td><strong>Anteprima</strong></td>
            <td><strong>Rilascio rapido</strong></td>
            <td><strong>Trimestrale</strong></td>
        </tr>
        <tr>
            <td>
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">Aggiungi thread all’inizio degli aggiornamenti</a></p>
                <p>Ora puoi fissare i thread più importanti nella parte superiore dell’area Aggiornamenti su un progetto, un’attività, un problema o una richiesta in modo che le informazioni chiave rimangano visibili per il team.</p>
            </td>
            <td><p>15 ottobre 2026</p></td>
            <td><p>12 novembre 2026</p></td>
            <td><p>21 gennaio 2027</p></td>
        </tr>
    </tbody>
</table>

## Note sulla versione per altre aree

* [Attività di rilascio di Adobe Workfront Fusion](https://experienceleague.adobe.com/it/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).
* [Attività di rilascio di Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

Al momento, in questa versione non sono presenti aggiornamenti per i seguenti elementi:

* Pianificazione scenari
* Bozza
* Obiettivi

## Annunci

### I campi fatturazione e tariffa di costo legacy nelle visualizzazioni elenco mansioni sono obsoleti

Nel tempo, abbiamo introdotto funzionalità avanzate di gestione dei tassi e esperienze di Ruolo dedicate che forniscono un approccio più completo e scalabile per mantenere le informazioni sui tassi. Di conseguenza, l’amministrazione dei tassi si sta spostando verso queste esperienze dedicate piuttosto che verso flussi di lavoro di gestione basati su elenchi.

Con la versione di gennaio 2027, i campi legacy **Fatturazione all&#39;ora** e **Costo all&#39;ora** non saranno più disponibili nell&#39;API di Workfront o nelle visualizzazioni elenco Ruoli, incluse le configurazioni Filtro/Visualizzazione/Raggruppamento (sia riferimenti diretti che colonne calcolate in modalità testo).

In sostituzione nei report, è possibile utilizzare il codice della modalità testo consigliato (utilizzare `costRates` o `billingRates` in base alle esigenze):

    &quot;
    displayname=Test
    listdelimiter=&lt;br>
    listmethod=nested(costRates).LISTS
    type=iterate
    valueexpression=CONCAT({startDate},&quot; - &quot;,{endDate},&quot;: &quot;,{value})
    valueformat=HTML
    &quot;

Per gestire e rivedere i tassi di ruolo, utilizza le esperienze di gestione dei tassi dedicate:

* Accedere e gestire le tariffe dei ruoli direttamente dalla pagina Ruolo > Tariffe.
* Utilizzare i rapporti Tasso per esaminare, analizzare e creare rapporti sulle informazioni relative ai tassi tra le mansioni.

Non è richiesta alcuna azione per prepararsi alla modifica. Tuttavia, gli amministratori che attualmente visualizzano i campi **Fatturazione all&#39;ora** e **Costo all&#39;ora** nelle visualizzazioni elenco Ruolo devono aggiornare i propri flussi di lavoro per utilizzare le esperienze di gestione delle tariffe consigliate descritte in precedenza.

Per informazioni sulle percentuali dei ruoli, vedere [Creare e gestire ruoli](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

-->

### Aggiornamenti della formazione

Esplora gli ultimi aggiornamenti apportati a programmi e percorsi di apprendimento, video e guide per ciascuna versione di Adobe Workfront. Per ulteriori informazioni, consulta la sezione “Novità” della [pagina dei tutorial di Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=it).
