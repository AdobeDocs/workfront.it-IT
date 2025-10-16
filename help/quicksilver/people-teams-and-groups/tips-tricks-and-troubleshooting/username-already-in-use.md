---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Nome utente già in uso
description: Leggi questi suggerimenti quando ricevi un errore che indica che il nome utente è già utilizzato.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 722295463c1338a70ff42c26acf69b09cf33f725
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 2%

---

# Nome utente già in uso

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
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
