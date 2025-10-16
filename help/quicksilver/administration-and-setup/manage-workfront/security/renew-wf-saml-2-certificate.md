---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,protezione,certificato,Amministratore,Esenzione,configura,metadati
navigation-topic: security
title: Rinnovare il certificato metadati SAML 2.0 di Adobe Workfront
description: I server Adobe Workfront utilizzano il protocollo SAML 2.0 per l’autenticazione e l’autorizzazione. Una volta aggiornato, il nuovo certificato rimane valido per un anno. Quando è il momento di rinnovare il certificato sul provider di identità, viene visualizzato un avviso in Workfront che segnala che questa modifica deve essere apportata. In qualità di amministratore di Workfront, puoi gestire questa modifica a livello di sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Rinnovare il certificato di metadati SAML 2.0 di Adobe Workfront

>[!IMPORTANT]
>
>La procedura descritta in questa pagina si applica solo alle organizzazioni che non hanno ancora effettuato l’onboarding in Admin Console. Se la tua organizzazione è stata integrata in Adobe Admin Console, non è necessaria alcuna azione.
>
>Per un elenco delle procedure che differiscono a seconda che l&#39;organizzazione sia stata integrata in Adobe Admin Console, consulta [Differenze di amministrazione basate su Platform (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

I server Adobe Workfront utilizzano il protocollo SAML 2.0 per l’autenticazione e l’autorizzazione. Una volta aggiornato, il nuovo certificato rimane valido per un anno. Quando è il momento di rinnovare il certificato sul provider di identità, viene visualizzato un avviso in Workfront che segnala che questa modifica deve essere apportata. In qualità di amministratore di Workfront, puoi gestire questa modifica a livello di sistema.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Questa opzione non è disponibile se l’istanza Workfront della tua organizzazione è abilitata con Adobe IMS. Per ulteriori informazioni, rivolgersi all&#39;amministratore di rete o IT.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td><p>Qualsiasi</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td><p>Standard</p><p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurare SAML 2.0 in Workfront

Per rivedere il messaggio di avviso e confermare l’aggiornamento dei metadati SAML 2.0 nel provider di identità:

{{step-1-to-setup}}

1. Fare clic su **Sistema** > **Single Sign-On**.

1. Nel menu a discesa **Tipo**, selezionare **SAML 2.0**.

1. Fare clic su **Scarica metadati SAML 2.0**.

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
1. In Workfront, nella **pagina Single Sign-on (SSO)**, verificare che questa opzione sia selezionata: **Il nuovo certificato Workfront è già stato caricato nel provider di identità**.

   >[!NOTE]
   >
   >* Questa opzione è visibile solo se si applicano tutte le seguenti condizioni:
   >   * La tua organizzazione è già configurata per SAML 2.0
   >   * Il certificato corrente è pronto per la scadenza
   >   * Il nuovo certificato è disponibile
   >* Quando questo campo è selezionato, gli amministratori di Workfront possono accedere a Workfront con le proprie credenziali SSO o Workfront.

1. Fai clic su **Salva**.

   Il messaggio di avviso non viene più visualizzato perché hai riconosciuto il rinnovo del certificato SAML 2.0 sul server del provider di identità.

1. Fai clic su **Verifica connessione** per verificare la configurazione.

   Dovresti visualizzare un messaggio che conferma che la connessione è avvenuta correttamente.

Per ulteriori informazioni o per assistenza nella configurazione manuale dei metadati, contatta il nostro team di supporto, come spiegato in [Contatta l&#39;Assistenza clienti](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
