---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Nome utente già in uso
description: Leggi questi suggerimenti quando ricevi un errore che indica che il nome utente è già utilizzato.
author: Becky
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
TQID: https://experienceleague.adobe.com/uGrOaZZzbE6CkodhE1TlCtW4rRJkfqljWGJbNSzxODc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 300
ht-degree: 14%

---

# Nome utente già in uso.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td><p>Amministratore di sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Domanda

Durante la creazione di un nuovo utente, viene visualizzato un errore [!UICONTROL Ops] che indica che il nome utente è già utilizzato. Non ci sono altre occorrenze di questa e-mail nel sistema. Perché viene visualizzato?

## Soluzione

Ciò può verificarsi perché il nome utente o l&#39;indirizzo e-mail non è univoco nell&#39;istanza [!DNL Adobe Workfront] corrente. Gli utenti possono avere lo stesso nome utente o indirizzo e-mail in istanze separate. Ad esempio, l&#39;utente A potrebbe avere i seguenti indirizzi e-mail associati a un account [!DNL Workfront]: usera@company1.com e usera@company2.com.

>[!NOTE]
>
>L&#39;amministratore [!DNL Workfront] primario non può avere lo stesso nome utente o indirizzo di posta elettronica se si trova in istanze Workfront separate nello stesso cluster.
>
>Se le istanze si trovano in cluster diversi, l’amministratore principale può avere lo stesso nome utente o indirizzo e-mail. Puoi visualizzare il cluster in cui si trova l&#39;istanza in [!UICONTROL Configurazione] > [!UICONTROL Sistema] > [!UICONTROL Informazioni cliente].

### Verifica se il nome utente è univoco nella tua istanza

Verificare che il nome utente e l&#39;indirizzo di posta elettronica siano univoci nell&#39;istanza [!DNL Workfront] corrente:

{{step-1-to-users}}

1. Nell&#39;elenco delle persone, cerca nella colonna **[!UICONTROL E-mail]** per verificare che non siano presenti e-mail duplicate.
1. Aggiungi alla vista una colonna per il nome utente.

   1. Nel menu a discesa **[!UICONTROL Visualizza]**, fare clic su **[!UICONTROL Personalizza visualizzazione]**.
   1. Fai clic su **[!UICONTROL Aggiungi colonna]**.
   1. Nel campo di ricerca digitare *[!UICONTROL nomeutente]*.
   1. Selezionare **[!UICONTROL Utente]** > **[!UICONTROL Nome utente]**.
   1. Salvate la vista.\
      In questo modo viene visualizzata una vista in cui vengono visualizzati i nomi utente da cui cercare il duplicato.

1. Nell&#39;elenco delle persone, controllare nella colonna **[!UICONTROL Nome utente]** per verificare che non siano presenti nomi utente duplicati.
