---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Cambia il dominio di Adobe Workfront
description: In qualità di amministratore Adobe Workfront e di contatto autorizzato del supporto Workfront, puoi richiedere assistenza al team del supporto Workfront per modificare il dominio Workfront della tua organizzazione.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Modificare il dominio di Adobe Workfront

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding in Admin Console. Se per la tua organizzazione è stato eseguito l’onboarding in Adobe Admin Console, non è possibile modificare il dominio Workfront.
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata in Adobe Admin Console, consulta [Differenze di amministrazione basate su Platform (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore Adobe Workfront e di contatto autorizzato del supporto Workfront, puoi richiedere assistenza al team del supporto Workfront per modificare il dominio Workfront della tua organizzazione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

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
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Richiedi modifica dominio

1. Inizia a creare un ticket di supporto su Experience League.
1. Nella casella **Descrizione** includere il nuovo dominio desiderato e l&#39;intervallo di tempo in cui si desidera che il nuovo dominio venga attivato.
1. Completare la compilazione delle caselle relative al caso di supporto, quindi fare clic su **Invia**.

È inoltre possibile chiamare il supporto tecnico Workfront per ottenere assistenza nella modifica del dominio.

## Aggiorna il nuovo dominio se sei un cliente SSO

Se l&#39;azienda utilizza l&#39;SSO, dopo aver modificato il dominio Workfront sono necessari i seguenti passaggi.

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

{{step-1-to-setup}}

1. Nella barra laterale a sinistra, fai clic su **Sistema** > **Informazioni cliente** e assicurati che il tuo dominio sia aggiornato nella pagina Informazioni cliente.

1. Nella barra laterale sinistra, fare clic su **Sistema** > **Single Sign-On (SSO)**.

1. Fare clic su **Scarica metadati SAML 2.0**.
1. Dopo aver scaricato il file, aprilo e accertati che:

   1. **entityID** punta al nuovo dominio.
   1. Tutte le posizioni in **`<md:AssertionConsumerService>`** puntano al nuovo dominio.

1. Fornisci il file di metadati scaricato al provider di identità in modo che possa aggiornarlo alla fine.
1. Assicurati che il dominio sia aggiornato per tutte le integrazioni Workfront utilizzate dalla tua organizzazione.
