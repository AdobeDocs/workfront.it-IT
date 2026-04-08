---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Configurare i collaboratori IA
description: In qualità di amministratore di Adobe Workfront, puoi configurare i collaboratori IA e assegnarli a progetti e attività.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: 25d5fef46bc8f02e92d778685c2ad6e93439f9ff
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 6%

---

# Configurare i collaboratori IA

{{highlighted-preview-article-level}}

I collaboratori IA sono un modo per integrare gli agenti IA nei progetti e nelle attività. Puoi configurare un Collaboratore IA, quindi assegnarlo come faresti con un utente.

Ad esempio, puoi configurare un collaboratore IA di tipo revisore con le linee guida del brand, quindi assegnare tale collaboratore per rivedere un documento.

I tipi di Collaboratore IA disponibili includono:

* Revisore: crea un collaboratore utilizzando i marchi<!-- or Adobe Brand Intelligence-->, quindi assegna il collaboratore come revisore delle risorse.

  Per ulteriori informazioni, vedere [Introduzione a Revisore contenuto Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

  >[!NOTE]
  >
  >Attualmente, Reviewer è l’unico tipo di Collaboratore IA disponibile. In futuro saranno disponibili più funzionalità di AI Collaborator.


## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td><p>Standard, Prime o Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>[!UICONTROL Amministratore di sistema]</td> 
  </tr> 
  </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti



* La tua organizzazione deve disporre di un contratto Adobe Gen AI firmato.

  Per ulteriori informazioni, consulta [Firmare il contratto di Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) nell&#39;articolo Assistente IA in Workfront.
* È necessario aver configurato un marchio in Workfront prima di poterlo utilizzare per un collaboratore di IA di tipo Revisore.

  Per istruzioni, consulta [Creare e gestire i brand per il revisore dei contenuti](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Crea un nuovo Collaboratore IA di tipo Revisore

{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. Fai clic su **Nuovo collaboratore** nell&#39;angolo superiore destro della schermata.
1. Fai clic su **Revisore**, quindi su **Continua**.

   >[!NOTE]
   >
   >Attualmente, è disponibile solo il tipo Revisore. In futuro saranno disponibili più tipi di collaboratori IA.

1. Nel campo Nome collaboratore immettere un nome per il collaboratore. Questo è il nome visualizzato nell&#39;elenco degli assegnatari disponibili per un&#39;attività.
   <!--1. Select whether the collaborator will use a brand or Adobe Brand Intelligence for its reviews.-->
   <!--1. (Conditional) If the AI Collaborator will use Adobe Brand Intelligence, select the tenant that it will use.-->
1. &#x200B;<!--(Conditional) If the AI Collaborator will use a Brand,-->Seleziona il marchio e la linea guida del marchio che utilizzerà.
1. Fai clic su **Salva**.

## Gestisci collaboratori IA

È possibile modificare, copiare ed eliminare i collaboratori IA esistenti.

{{step-1-to-setup}}

1. Nel menu di navigazione a sinistra, fai clic su **Collaboratori IA**.
1. (Condizionale) Per modificare un collaboratore, fare clic sul nome del collaboratore che si desidera modificare, apportare le modifiche desiderate nella finestra Modifica collaboratore e fare clic su **Salva**.
1. (Condizionale) Per copiare un collaboratore, fare clic sull&#39;icona Copia ![icona Copia](assets/copy-ai-collaborator.png) nella riga del collaboratore AI che si desidera copiare, fare clic sul nome della copia, apportare le modifiche desiderate nella finestra Modifica collaboratore e fare clic su **Salva**.
1. (Condizionale) Per eliminare un collaboratore, fare clic sull&#39;icona Elimina ![icona Elimina](assets/delete-collaborator-icon.png) nella riga del collaboratore AI che si desidera eliminare, quindi fare clic su **Elimina**.
