---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,protezione,certificato,Amministratore,Esenzione,configura,metadati
navigation-topic: security
title: Rinnovare il certificato di metadati SAML 2.0 di Adobe Workfront
description: I server Adobe Workfront utilizzano il protocollo SAML 2.0 per l’autenticazione e l’autorizzazione. Una volta aggiornato, il nuovo certificato rimane valido per un anno. Quando è il momento di rinnovare il certificato sul provider di identità, viene visualizzato un avviso in Workfront che segnala che questa modifica deve essere apportata. In qualità di amministratore di Workfront, puoi gestire questa modifica a livello di sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 54cbdfddb3a012b78b3428a3f8bd5c094561c860
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# Rinnovare il certificato di metadati SAML 2.0 di Adobe Workfront

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding nell’Admin Console. Se la tua organizzazione è stata integrata in Adobe Admin Console, non è necessaria alcuna azione.
>
>Per un elenco delle procedure che differiscono in base al fatto che la tua organizzazione sia stata onboarding in Adobe Admin Console, consulta [Differenze di amministrazione basate su piattaforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

I server Adobe Workfront utilizzano il protocollo SAML 2.0 per l’autenticazione e l’autorizzazione. Una volta aggiornato, il nuovo certificato rimane valido per un anno. Quando è il momento di rinnovare il certificato sul provider di identità, viene visualizzato un avviso in Workfront che segnala che questa modifica deve essere apportata. In qualità di amministratore di Workfront, puoi gestire questa modifica a livello di sistema.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

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
  <td role="rowheader">Licenza Adobe Workfront*</td> 
  <td> <p>Nuovo: Standard </p>
 <p>oppure</p> 
<p>Corrente: Piano </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurare SAML 2.0 in Workfront

Per rivedere il messaggio di avviso e confermare l’aggiornamento dei metadati SAML 2.0 nel provider di identità:

1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

1. Clic **Sistema** > **Single Sign-On**.

1. In **Tipo** menu a discesa, seleziona **SAML 2.0**.

1. Clic **Scarica metadati SAML 2.0**.

   In questo modo viene scaricato il certificato Workfront rinnovato per SAML 2.0, che contiene i metadati corretti per il server.

1. Nel provider di identità, copia l’URL ACS (Assertion Consumer Service) corrente (noto anche come URL di risposta) in un luogo sicuro.

   >[!CAUTION]
   >
   >Prima di caricare i metadati di Workfront nel provider Single Sign-On (SSO) nel passaggio 6, copiare l&#39;URL corrente del servizio consumer di asserzioni (ACS) in un luogo sicuro. Questo URL, noto anche come URL di risposta, si trova nella pagina di configurazione Workfront del provider SSO.
   >
   >
   >Se l’URL ACS cambia dopo aver caricato i metadati Workfront, questi potrebbero contenere un URL ACS errato. Per evitare l&#39;interruzione della connessione Single Sign-On, è necessario ripristinarla con quella copiata. Dopo l’aggiornamento, il certificato sarà comunque corretto.

1. Nel server del provider di identità, aggiorna il nuovo certificato scaricato.
1. (Condizionale) Se l’URL di Assertion Consumer Service (ACS) o l’URL di risposta è stato modificato nel provider di identità, riportalo all’URL copiato nel passaggio 5.
1. In Workfront, il **Pagina Single Sign-on (SSO)**, accertati che questa opzione sia selezionata: **Il nuovo certificato Workfront è già stato caricato nel provider di identità**.

   >[!NOTE]
   >
   >* Questa opzione è visibile solo se si applicano tutte le seguenti condizioni:
   >   * La tua organizzazione è già configurata per SAML 2.0
   >   * Il certificato corrente è pronto per la scadenza
   >   * Il nuovo certificato è disponibile
   >* Quando questo campo è selezionato, gli amministratori di Workfront possono accedere a Workfront con le proprie credenziali SSO o Workfront.

1. Fai clic su **Salva**.

   Il messaggio di avviso non viene più visualizzato perché hai riconosciuto il rinnovo del certificato SAML 2.0 sul server del provider di identità.

1. Clic **Verifica connessione** per testare la configurazione.

   Dovresti visualizzare un messaggio che conferma che la connessione è avvenuta correttamente.

Per ulteriori informazioni o per assistenza nella configurazione manuale dei metadati, contatta il nostro team di supporto, come spiegato in [Contatta l’Assistenza clienti](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
