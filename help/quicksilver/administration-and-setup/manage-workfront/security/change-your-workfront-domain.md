---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Modificare il dominio di Adobe Workfront
description: In qualità di amministratore Adobe Workfront e di contatto autorizzato del supporto Workfront, puoi richiedere assistenza al team del supporto Workfront per modificare il dominio Workfront della tua organizzazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b9e088a0cdb32f3e8c565ea17f4613dda104bd7b
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Modificare il dominio di Adobe Workfront

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding nell’Admin Console. Se per la tua organizzazione è stato eseguito l’onboarding in Adobe Admin Console, non è possibile modificare il dominio Workfront.
>
>Per un elenco delle procedure che differiscono in base al fatto che la tua organizzazione sia stata onboarding in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore Adobe Workfront e di contatto autorizzato del supporto Workfront, puoi richiedere assistenza al team del supporto Workfront per modificare il dominio Workfront della tua organizzazione.

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
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Richiedi modifica dominio

1. Fai clic su **Supporto** nella pagina Workfront One, quindi inizia a creare un caso di supporto.
1. In **Descrizione** , includi il nuovo dominio desiderato e l’intervallo di tempo in cui desideri che il nuovo dominio venga reso live.
1. Completare la compilazione delle caselle relative al caso di supporto, quindi fare clic su **Invia**.

È inoltre possibile chiamare il supporto tecnico Workfront per ottenere assistenza nella modifica del dominio.

## Aggiorna il nuovo dominio se sei un cliente SSO

Se l&#39;azienda utilizza l&#39;SSO, dopo aver modificato il dominio Workfront sono necessari i seguenti passaggi.

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nella barra laterale a sinistra, fai clic su **Sistema** > **Informazioni Cliente** e assicurati che il tuo dominio sia aggiornato nella pagina Informazioni cliente.

1. Nella barra laterale a sinistra, fai clic su **Sistema** > **Single Sign-On (SSO)**.

1. Clic **Scarica metadati SAML 2.0**.
1. Dopo aver scaricato il file, aprilo e accertati che:

   1. **entityID** sta puntando al nuovo dominio.
   1. Tutte le posizioni in **`<md:AssertionConsumerService>`** selezionare il nuovo dominio.

1. Fornisci il file di metadati scaricato al provider di identità in modo che possa aggiornarlo alla fine.
1. Assicurati che il dominio sia aggiornato per tutte le integrazioni Workfront utilizzate dalla tua organizzazione.
