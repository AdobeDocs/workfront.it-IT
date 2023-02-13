---
title: Crittografatore
description: I moduli di crittografia di Adobe Workfront Fusion consentono di crittografare qualsiasi dato di testo. Attualmente supportano la crittografia dei messaggi tramite AES256 e PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Crittografatore

[!DNL Adobe Workfront Fusion] [!UICONTROL Crittografatore] I moduli ti consentono di crittografare qualsiasi dato di testo. Attualmente supportano la crittografia dei messaggi tramite AES256 e PGP ([!UICONTROL OpenPGP]).

## Requisiti di accesso

Per utilizzare le funzionalità di questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] piano*</td>
  <td> <p>[!UICONTROL Pro] o superiore</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licenza**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] per automazione e integrazione del lavoro] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] per automazione del lavoro</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prodotto</td> 
   <td>La tua organizzazione deve acquistare [!DNL Adobe Workfront Fusion] nonché [!DNL Adobe Workfront] per utilizzare le funzionalità descritte in questo articolo.</td> 
  </tr> 
 </tbody> 
</table>

Per sapere quale piano, tipo di licenza o accesso hai, contatta il tuo [!DNL Workfront] amministratore.

Per informazioni su [!DNL Adobe Workfront Fusion] licenze, vedi [[!DNL Adobe Workfront Fusion] licenze](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Crittografia e decrittografia dei messaggi con PGP

Quando si crittografano e si decrittografano tramite PGP, è necessario utilizzare una portachiavi e creare una chiave privata o pubblica (o entrambe).

Per ulteriori informazioni sulle chiavi pubblica e privata, vedi [Termini di base in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Per ulteriori informazioni sulle portachiavi, vedi [Chiavi in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Crittografatore] moduli e relativi campi

Durante la configurazione [!UICONTROL Crittografatore] vengono visualizzati i campi seguenti. Un titolo in grassetto in un modulo indica un campo obbligatorio.

### Cifrare un messaggio PGP

Questo modulo ti consente di crittografare un messaggio utilizzando chiavi pubbliche e private.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Chiave privata]</td>
        <td>Immetti la chiave privata del mittente. In questo modo è possibile autenticare l’identità del mittente.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Chiave pubblica]</td>
        <td>Immetti la chiave pubblica del destinatario.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Immetti il messaggio da crittografare.</td>
    </tr>

### Decrittografare un messaggio PGP

Questo modulo ti consente di decrittografare un messaggio utilizzando chiavi pubbliche e private.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Chiave privata]</td>
        <td>Immetti la chiave privata del destinatario.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Chiave pubblica]</td>
        <td>Immetti la chiave pubblica del destinatario. In questo modo è possibile autenticare l’identità del mittente.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Mappa il messaggio da decrittografare.</td>
    </tr>
</table>
