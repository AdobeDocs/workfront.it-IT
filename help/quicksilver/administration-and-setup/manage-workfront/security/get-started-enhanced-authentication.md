---
title: File nascosto
description: Nascosto dalla ricerca e dal menu di navigazione a sinistra
hidefromtoc: true
hide: true
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: a151fa70a1093db3d9a0af1f4024d5d4cb5fd317
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 3%

---

# Panoramica dell’autenticazione avanzata

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront sta modificando la gestione del sistema di utenti e password. Queste modifiche verranno implementate in una versione graduale denominata **Autenticazione avanzata** esperienza. L’autenticazione avanzata offre agli utenti un’esperienza di accesso più coerente e sicura su tutti i prodotti e i servizi Workfront.

La tabella seguente fornisce dettagli sulle funzionalità correnti e future:

>[!IMPORTANT]
>
>La maggior parte dei clienti utilizza attualmente l’autenticazione legacy, mentre alcuni utilizzano l’autenticazione avanzata 1.0.
> 
>Per verificare il tipo di autenticazione in uso, vai a *dominio_utente*.my.workfront.com/login. Se si viene reindirizzati a /auth/login, si utilizza l&#39;autenticazione avanzata 1.0.
> 
>Se sei reindirizzato a https://login-a-xx.workfront.com/, dove &quot;xx&quot; potrebbe essere US (Stati Uniti), EU (Europa) o GCP (Google Cloud Platform) a seconda della tua posizione/piattaforma, stai utilizzando l’autenticazione avanzata 2.0.
>
>Tutti i clienti passeranno a Autenticazione avanzata 2.0 entro la fine del 2021.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Funzionalità</strong> </p> </th> 
   <th><strong>Autenticazione legacy</strong> </th> 
   <th><strong>Autenticazione avanzata 1.0</strong> </th> 
   <th> <p>Autenticazione avanzata 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Opzioni di accesso</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Possibilità di utilizzare un singolo nome utente per tutti i prodotti e servizi Workfront, inclusi formazione, supporto e altri</p> </td> 
   <td>Non disponibile</td> 
   <td> <p>Non disponibile</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Consenti l’utilizzo dello stesso indirizzo e-mail nelle istanze di Workfront</p> </td> 
   <td> <p>✓</p> <p>Disponibile dalla versione 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponibile dalla versione 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponibile dalla versione 2019.3</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gli indirizzi e-mail non fanno distinzione tra maiuscole e minuscole</p> </td> 
   <td> <p>✓</p> <p>Disponibile dalla versione 2019.3</p> </td> 
   <td> <p>✓</p> <p>Più utenti non possono avere lo stesso indirizzo e-mail se l’indirizzo differisce solo per maiuscole e minuscole. </p> </td> 
   <td> <p>✓</p> <p>Più utenti non possono avere lo stesso indirizzo e-mail se l’indirizzo differisce solo per maiuscole e minuscole. </p> <p>Gli amministratori di Workfront riceveranno una notifica verso la fine del 2019 per iniziare a correggere gli indirizzi e-mail duplicati.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Opzioni di gestione delle password</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Creare un messaggio e-mail di reimpostazione della password per un utente come amministratore di Workfront</p> </td> 
   <td> <p>Non disponibile </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Impostare una password temporanea per un utente come amministratore di Workfront</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Non pianificato</p> <p>Questa funzionalità non è una best practice per la sicurezza</p> </td> 
   <td> <p>Non pianificato</p> <p>Questa funzionalità non è una best practice per la sicurezza</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Requisiti dei criteri per le password</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Richiede agli utenti di reimpostare le password dopo un determinato intervallo di tempo</p> </td> 
   <td>✓</td> 
   <td> <p>Non pianificato</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Limita l'utilizzo di una password precedente </p> </td> 
   <td>✓</td> 
   <td>Non pianificato </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Protezione da tentativi di immissione di password non corretti </p> </td> 
   <td> <p>✓ </p> <p>Blocca l’account dopo 5 tentativi di immissione di password non corretti. Tempo di attesa necessario dopo la configurazione del blocco da parte dell'amministratore di Workfront</p> </td> 
   <td> <p>✓</p> <p>Il tempo di attesa aumenta in modo esponenziale dopo ogni password errata consecutiva in base alle best practice del settore; il tempo richiesto non è configurabile dall’amministratore Workfront</p> </td> 
   <td> <p>✓</p> <p>Utilizza un algoritmo di blocco che blocca in modo proattivo diversi comportamenti sospetti.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Richiede una combinazione di lettere minuscole, lettere maiuscole, numeri e caratteri speciali</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Maggiore flessibilità nella scelta dei requisiti specifici</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Imposta una lunghezza minima per la password </p> </td> 
   <td> Non disponibile </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>Supporto del protocollo Single Sign-On</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Supporta le integrazioni SSO conformi con Active Directory e i protocolli LDAP</p> </td> 
   <td> ✓ </td> 
   <td> <p> Obsoleto</p> <p>I sistemi Active Directory, Azure e LDAP devono utilizzare SAML 2.0</p> </td> 
   <td> <p>Obsoleto</p> <p>I sistemi Active Directory, Azure e LDAP possono essere configurati con SAML 2.0 o OpenID Connect crittografati.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supporta protocolli SSO conformi a SAML 2.0 </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supporta i protocolli Open ID Connect</p> </td> 
   <td> <p>Non disponibile</p> </td> 
   <td> <p>Non disponibile</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Configura la pagina di accesso di Workfront per reindirizzare sempre alla pagina di accesso del provider di identità </p> </td> 
   <td> Abilitato per impostazione predefinita e non disabilitato</td> 
   <td> <p>✓</p> <p>L’amministratore di Workfront può configurare la pagina di accesso in modo che venga reindirizzata alla pagina di accesso del provider di identità oppure può configurare uno o più pulsanti di accesso.</p> </td> 
   <td> <p>✓</p> <p> Gli amministratori di Workfront possono configurare la pagina di accesso in modo da reindirizzarla alla pagina di accesso del provider di identità oppure configurare uno o più pulsanti di accesso.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Consenti a ogni istanza di abilitare più provider SSO</p> </td> 
   <td> <p>N/D</p> </td> 
   <td> <p>Non pianificato</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Supporto per l’ambiente</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Un singolo nome utente e una singola password per gli ambienti di anteprima</p> </td> 
   <td> <p>Non disponibile</p> </td> 
   <td> <p>Non disponibile</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Un singolo nome utente e una singola password per gli ambienti sandbox</p> </td> 
   <td> <p>Non disponibile</p> </td> 
   <td> <p>Non disponibile</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
