---
content-type: reference
navigation-topic: get-started-with-workfront
title: Preparazione HIPAA per Workfront
description: Un cliente Workfront che, come definito in HIPAA, è un Business Associate e/o l’Entità coperta per conto del quale il Business Associate fornisce Adobe Workfront deve utilizzare le seguenti linee guida per configurare Workfront per l’utilizzo compatibile con HIPAA.
feature: Get Started with Workfront
author: Courtney
exl-id: e3cdaa03-d523-46a4-954b-8456d5f190e4
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Preparazione HIPAA per Workfront

Un cliente Workfront che, come definito in HIPAA, è un Business Associate e/o l’Entità coperta per conto del quale il Business Associate fornisce Adobe Workfront deve utilizzare le seguenti linee guida per configurare Workfront per l’utilizzo compatibile con HIPAA:


## Requisiti per la password

| **Impostazione protezione** | **Cos&#39;È?** | **Requisito** |
|----------------------|------------------|------------------|
| Numero minimo di password per i contratti | Qual è la forza minima per le password di accordo? | Non meno di 8 caratteri |
| Numero minimo di password per le password utente | Qual è il numero minimo di password degli utenti? | Caratteri di tre delle seguenti categorie:<br> Lettere maiuscole (alfabeto latino)<br> Lettere minuscole (alfabeto latino)<br> Base 10 cifre<br> Caratteri non alfanumerici |
| Durata password | Per quanto tempo le password devono rimanere invariate? | Le password devono essere modificate almeno ogni 90 giorni |
| Cronologia password | Quante password passate devono essere memorizzate e non consentite? | Non meno di 5 |


## Requisiti di accesso

| **Impostazione protezione** | **Cos&#39;È?** | **Requisito** |
|----------------------|------------------|------------------|
| Numero massimo di errori di accesso | Quanti tentativi di accesso non riusciti bloccano l&#39;utente? | Non più di 5 tentativi in un periodo di 5 minuti; è possibile riprovare dopo 30 minuti |
| Numero massimo errori di verifica SSO | Quanti tentativi di verifica SSO non riusciti causano un blocco? | Non più di 5 (si applica solo ai clienti che utilizzano SSO) |


## Requisiti della sessione

| **Impostazione protezione** | **Cos&#39;È?** | **Requisito** |
|----------------------|------------------|------------------|
| Timeout sessione | Quanti minuti di inattività causano la disconnessione? | Non più di 15 minuti |

## Responsabilità del cliente

Assicurati che tutti i dipendenti, i rappresentanti e/o gli agenti siano a conoscenza e comprendano i termini dei contratti di licenza e/o di servizio firmati tra le parti, a seconda dei casi, relativi all’utilizzo dei dati con Workfront.

In particolare, dovrebbero essere riesaminate e comunicate le seguenti responsabilità e obblighi: 

* Il Cliente è responsabile dell&#39;utilizzo del Servizio Workfront da parte di tutti i suoi utenti. 

* Il cliente deve rispettare tutti i termini del contratto con Adobe che include il caricamento di elementi dati non consentiti in Workfront. 

* Tutti i dati sensibili, inclusi, ma non limitati a ePHI, vengono caricati a rischio del cliente.  Il cliente è sempre responsabile di tutti i dati del cliente. 


## Protezione dei dati e conformità

>[!IMPORTANT]
>
>Workfront non è progettato per essere un archivio di record sanitari elettronici (EHR). ePHI può essere elaborato solo se espressamente autorizzato da Adobe per iscritto. 

* Per qualsiasi database Workfront in cui potrebbe essere accessibile ePHI, verificare che **Encryption at Rest (EAR)** sia abilitato.
   * Contatta il tuo Account Executive (AE) per verificare che l’EAR sia incluso nell’acquisto di Workfront.
   * Configurazione di sistemi/database accessibili tramite Workfront per soddisfare gli obblighi di conformità.
* Assicurati che ePHI non venga trasferito, collegato o condiviso con altre soluzioni Adobe non conformi HIPAA.
* Assicurarsi che le fotografie dei pazienti elaborate tramite Workfront siano conservate in modo sicuro e non siano accessibili pubblicamente.
