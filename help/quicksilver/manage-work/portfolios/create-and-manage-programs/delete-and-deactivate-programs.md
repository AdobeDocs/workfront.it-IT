---
product-area: programs
navigation-topic: Create and manage programs
title: Eliminare e disattivare i programmi
description: Un programma rappresenta una raccolta di progetti che condividono una strategia, un obiettivo o un obiettivo comune che trascende i limiti del progetto. I programmi sono una suddivisione dei portafogli e non possono esistere al di fuori di un portfolio. In genere, i programmi condividono le stesse risorse di altri programmi all’interno dello stesso portfolio. È possibile eliminare o disattivare un programma quando diventa irrilevante.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 605d1ec5-ca2e-4ff0-87e1-fa53d8ac4a95
TQID: https://experienceleague.adobe.com/nXFATsZ0uMLsgS-q4VlSQxL1Zh29QSCSAWTHxEGBgMw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 464
ht-degree: 7%

---

# Eliminare e disattivare i programmi

Un programma rappresenta una raccolta di progetti che condividono una strategia, un obiettivo o un obiettivo comune che trascende i limiti del progetto. I programmi sono una suddivisione dei portafogli e non possono esistere al di fuori di un portfolio. In genere, i programmi condividono le stesse risorse di altri programmi all’interno dello stesso portfolio.

Quando un programma diventa irrilevante, puoi effettuare una delle seguenti operazioni per impedire agli utenti di associare progetti al programma:

* Disattivala: i progetti in uscita rimangono associati al programma e al relativo portfolio. Gli utenti non vedono più il programma come un’opzione quando tentano di associare nuovi progetti al programma.
* Eliminalo: i progetti esistenti perdono la loro associazione con il programma e passano direttamente sotto il portfolio. Gli utenti non vedono più il programma come un’opzione quando tentano di associare i loro progetti futuri al programma.

È consigliabile disattivare un portfolio, anziché eliminarlo, per conservare le informazioni storiche per i progetti. Tuttavia, a volte può essere necessario eliminare un programma.

## Requisiti di accesso

+++ Espandere per visualizzare i requisiti di accesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] pacchetto</td>

<td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licenza</td> 
   <td> <p>[!UICONTROL Standard]</p><p>[!UICONTROL Piano]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso a portafogli e programmi tramite [!UICONTROL Edit] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni sugli oggetti</td> 
   <td> <p>Autorizzazioni di [!UICONTROL Manage] per il portfolio</p> <p>Per impostazione predefinita, dopo aver creato un programma, si dispone di autorizzazioni [!UICONTROL Manage].</p>  </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, consulta [Requisiti di accesso nella documentazione Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eliminare un programma

{{step1-to-programs}}

1. Fare clic sul nome di un programma per aprirlo.
1. Fai clic sul menu **Altro** a destra del nome del programma, quindi fai clic su **Elimina programma**.
1. Fai clic su **Sì, eliminalo** per confermare.

   Il programma viene eliminato e si verificano gli eventi seguenti:

   * I progetti esistenti perdono la loro associazione con il programma e passano direttamente sotto il portafoglio.
   * Gli utenti non vedono più il programma come un’opzione quando tentano di associare i loro progetti futuri al programma.

## Disattivare un programma

{{step1-to-programs}}

1. Fare clic sul nome di un programma per aprirlo.
1. Esegui una delle operazioni seguenti:

   * Fai clic sul menu **Altro** a destra del nome del programma, quindi fai clic su **Disattiva programma**.
   * Fai clic sul menu **Altro** a destra del programma, quindi fai clic su **Modifica**

     Oppure

     Fai clic sulla sezione **Dettagli programma** nel pannello a sinistra e deseleziona la casella **È attivo**.

   Il programma viene disattivato immediatamente e si verificano i seguenti eventi:

   * I progetti in uscita rimangono associati al programma e al relativo portafoglio.
   * Gli utenti non vedono più il programma come un’opzione quando tentano di associare nuovi progetti al programma.
