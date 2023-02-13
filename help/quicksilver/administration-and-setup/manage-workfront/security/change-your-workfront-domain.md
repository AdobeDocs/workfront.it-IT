---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Modificare il dominio Adobe Workfront
description: In qualità di amministratore Adobe Workfront e di contatto autorizzato per l’Assistenza Workfront, puoi richiedere aiuto al team di supporto Workfront per modificare il dominio Workfront della tua organizzazione.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b413ffc2416439629e073b32b5e9828df2f5de90
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Modificare il dominio Adobe Workfront

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
>
>Per modificare il dominio Adobe Workfront se l’organizzazione è stata caricata in Adobe Admin Console, consulta [Configurare i domini](https://helpx.adobe.com/enterprise/using/set-up-identity.html#setup-domains).
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

In qualità di amministratore Adobe Workfront e di contatto autorizzato per l’Assistenza Workfront, puoi richiedere aiuto al team di supporto Workfront per modificare il dominio Workfront della tua organizzazione.

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
   <td role="rowheader">Configurazioni a livello di accesso</td> 
   <td> <p>Devi essere un amministratore Workfront.</p> <p><b>NOTA</b>: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Richiesta di modifica del dominio

1. Fai clic sul pulsante **Supporto** nella pagina Workfront One , quindi inizia a creare un caso di supporto.
1. In **Descrizione** Includi il nuovo dominio desiderato, nonché l’intervallo di tempo in cui desideri che il nuovo dominio diventi attivo.
1. Completare la compilazione delle caselle per il caso di assistenza, quindi fare clic su **Invia**.

Puoi anche chiamare il supporto Workfront per ricevere assistenza sulla modifica del dominio.

## Aggiorna il nuovo dominio se sei un cliente SSO

Se l&#39;azienda utilizza SSO, dopo la modifica del dominio Workfront sono necessari i seguenti passaggi.

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Nella barra laterale sinistra, fai clic su **Sistema** > **Informazioni cliente** e assicurati che il tuo dominio sia aggiornato nella pagina Informazioni cliente .

1. Nella barra laterale sinistra, fai clic su **Sistema** > **Single Sign-On (SSO)**.

1. Fai clic su **Scarica i metadati SAML 2.0**.
1. Dopo aver scaricato il file, aprilo e accertati di quanto segue:

   1. **entityID** indica il nuovo dominio.
   1. Tutte le posizioni all&#39;interno di **`<md:AssertionConsumerService>`** puntare al nuovo dominio.

1. Fornisci il file di metadati scaricato al provider di identità in modo che possa aggiornarlo al termine.
1. Assicurati che il dominio sia aggiornato per tutte le integrazioni Workfront utilizzate dalla tua organizzazione.
