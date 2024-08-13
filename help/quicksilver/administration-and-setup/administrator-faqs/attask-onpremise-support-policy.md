---
title: Criterio di supporto AtTask OnPremise
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
description: Adobe Workfront è passato a un modello Software-As-A-Service al 100% e ha cessato di vendere software on-premise il 31 dicembre 2011. A partire dal 2014, AtTask OnPremise non è più supportato, ad eccezione dei problemi relativi alle chiavi di licenza. L'applicazione locale non è più disponibile per il download o l'installazione.
feature: System Setup and Administration
role: Admin
exl-id: 37c65360-6587-43b3-8eaf-4f1a9b375c1d
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Criterio di supporto AtTask OnPremise

Adobe Workfront è passato a un modello Software-As-A-Service al 100% e ha cessato di vendere software on-premise il 31 dicembre 2011. A partire dal 2014, AtTask OnPremise non è più supportato, ad eccezione dei problemi relativi alle chiavi di licenza. L&#39;applicazione locale non è più disponibile per il download o l&#39;installazione.

Se si dispone già dell&#39;applicazione e si desidera reinstallare OnPremise, scaricare la guida all&#39;installazione .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">OnPremise optimization tips can be found.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more about reporting in AtTask OnPremise, click.</p>
-->

Istruzioni per il download della configurazione SSL/TSL.

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront. Per ulteriori informazioni, vedere <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Concedere a un utente l'accesso amministrativo completo</a>.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aggiornare il codice di licenza OnPremise

Se hai bisogno di una nuova chiave di licenza, chiama l&#39;Assistenza clienti Workfront al numero 844-306-HELP(4357).

Dopo aver ottenuto una nuova chiave di licenza,

1. Arresta il server atTask.
1. Rinomina il file license.key corrente (che si trova nella cartella AtTaskDoc).
1. Copia il nuovo file license.key nella posizione corretta.
1. Riavviare atTask Server.

Questo articolo include i seguenti allegati:
