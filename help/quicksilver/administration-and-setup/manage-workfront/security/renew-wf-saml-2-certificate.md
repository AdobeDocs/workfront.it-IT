---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0, sicurezza, certificato, amministratore, esenzione, configurazione, metadati
navigation-topic: security
title: Rinnovare il certificato metadati Adobe Workfront SAML 2.0
description: La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata configurata per Adobe Admin Console, devi eseguire questa azione tramite Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Rinnovare il certificato metadati Adobe Workfront SAML 2.0

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non sono ancora state integrate nell’Admin Console. Se l’organizzazione è stata integrata in Adobe Admin Console, non è necessaria alcuna azione.
>
>Per un elenco delle procedure che variano a seconda che l’organizzazione sia stata caricata in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

I server Adobe Workfront utilizzano il protocollo SAML 2.0 per l’autenticazione e l’autorizzazione. Una volta aggiornato, il nuovo certificato rimane valido per un anno. Quando è il momento di rinnovare il certificato sul provider di identità, in Workfront viene visualizzato un avviso che segnala che la modifica deve verificarsi. In qualità di amministratore di Workfront, puoi gestire questa modifica a livello di sistema.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgiti al tuo amministratore di rete o IT.

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

## Configurare SAML 2.0 in Workfront

Per esaminare il messaggio di avviso e confermare l’aggiornamento dei metadati SAML 2.0 nel provider di identità:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Fai clic su **Sistema** > **Single Sign-On**.

1. In **Tipo** menu a discesa, seleziona **SAML 2.0**.

1. Fai clic su **Scarica i metadati SAML 2.0**.

   In questo modo viene scaricato il certificato Workfront rinnovato per SAML 2.0, che contiene i metadati corretti per il server.

   >[!CAUTION]
   >
   >Prima di caricare i metadati Workfront sul provider Single Sign-On (SSO) al passaggio 5, copia l’URL corrente di Assertion Consumer Service (ACS) in un luogo sicuro. Questo URL, noto anche come URL di risposta, si trova nella pagina di configurazione Workfront del provider SSO.
   >
   >
   >Se l’URL ACS cambia dopo aver caricato i metadati Workfront, ciò significa che i metadati potrebbero contenere un URL ACS errato. Per evitare di interrompere la connessione Single Sign-On, è necessario ripristinarla a quella copiata. Il certificato aggiornato continuerà a essere corretto dopo questa operazione.

1. Vai al server del provider di identità e aggiorna il nuovo certificato scaricato.
1. In Workfront, sul **Pagina Single Sign-On (SSO)**, assicurati che questa opzione sia selezionata: **Il nuovo certificato Workfront è già stato caricato nel provider di identità**.

   Quando questo campo è selezionato, gli amministratori di Workfront possono accedere a Workfront con le proprie credenziali SSO o Workfront.

1. Fai clic su **Salva**.

   Il messaggio di avviso non viene più visualizzato perché è stato riconosciuto il rinnovo del certificato SAML 2.0 sul server del provider di identità.

1. Fai clic su **Prova connessione** per verificare la configurazione.

   Dovresti visualizzare un messaggio di conferma del corretto funzionamento della connessione.

Per ulteriori informazioni o per assistenza nella configurazione manuale dei metadati, contatta il nostro team di supporto, come spiegato in [Contatta l’Assistenza clienti](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
