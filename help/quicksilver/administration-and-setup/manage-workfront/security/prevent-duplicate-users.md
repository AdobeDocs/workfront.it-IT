---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Impedisci utenti duplicati
description: Durante la creazione di un nuovo utente in Adobe Workfront, non è più possibile utilizzare un indirizzo e-mail già utilizzato da un altro utente, anche se l’indirizzo e-mail varia in base al caso (ad esempio, JohnDoe@example.com e johndoe@example.com). Inoltre, per prepararsi ai miglioramenti futuri dell’autenticazione, assicurati che tutti gli utenti abbiano indirizzi e-mail univoci in un’istanza di Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Impedisci utenti duplicati

Durante la creazione di un nuovo utente in Adobe Workfront, non è più possibile utilizzare un indirizzo e-mail già utilizzato da un altro utente, anche se l’indirizzo e-mail varia in base al caso (ad esempio, JohnDoe@example.com e johndoe@example.com). Inoltre, per prepararsi ai miglioramenti futuri dell’autenticazione, assicurati che tutti gli utenti abbiano indirizzi e-mail univoci in un’istanza di Workfront.

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
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se non disponi ancora dell'accesso, chiedi all'amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Creare utenti con indirizzi e-mail univoci

A partire dalla versione 2019.4, quando si crea un nuovo utente in Workfront, non è più possibile utilizzare un indirizzo e-mail già utilizzato da un altro utente, anche se l’indirizzo e-mail varia in base ai casi. Ad esempio, non puoi creare un utente con l’indirizzo e-mail JohnDoe@example.com se un altro utente ha l’indirizzo e-mail johndoe@example.com.

## Aggiornare gli indirizzi e-mail degli utenti esistenti nell’istanza Workfront

In qualità di amministratore di Workfront, devi aggiornare gli utenti esistenti che hanno indirizzi e-mail corrispondenti che differiscono solo per maiuscole e minuscole.
Per correggere gli indirizzi e-mail duplicati all’interno di un’istanza di Workfront:

1. Esamina eventuali utenti duplicati e decidi quale utente non è più necessario.

   1. Fai clic sull&#39;icona ![](assets/main-menu-icon.png) del **menu principale** nell&#39;angolo superiore destro di Workfront, quindi fai clic su **Utenti**. ![](assets/users-icon-in-main-menu.png)

   1. Nel menu **Filtro**, seleziona **Tutto**.

   1. Nel menu **Visualizza**, selezionare **Accesso utente**.

   1. Nel menu **Raggruppamento**, seleziona **Niente**.

   1. Personalizzare la visualizzazione Accesso utente.

      1. Fare clic su **Visualizza** > **Personalizza visualizzazione**.

      1. Sostituisci la colonna **ID** con la colonna **Indirizzo e-mail**.

      1. Rinomina la visualizzazione e salvala.

   1. Crea un nuovo Raggruppamento.

      1. Fai clic su **Raggruppamento** > **Nuovo raggruppamento**.

      1. Fare clic su **Passa alla modalità testo** nell&#39;angolo superiore destro della pagina.
      1. Incolla il seguente codice in modalità testo:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. Rinomina il raggruppamento e salvalo.

1. Effettua una delle seguenti operazioni:

   * (Metodo preferito) Aggiungi un indirizzo + all’indirizzo e-mail dell’utente per ogni account aggiuntivo.

     Scegli questa opzione se un singolo utente dell’organizzazione deve accedere a più di un account utente. Se l&#39;indirizzo più non è supportato dal provider di posta elettronica, è necessario fornire un account di posta elettronica separato per ogni account Workfront.

     Ad esempio, John Doe può avere un account utente per il suo account di utilizzo giornaliero e uno da utilizzare a scopo di test:

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * Modifica il dominio per utilizzare un dominio falso aggiungendo il seguente testo all’indirizzo e-mail:

     `.inactive`

     Ad esempio, John Doe potrebbe avere i seguenti domini: (Questi devono essere univoci).

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     Non puoi più accedere a questi account perché per reimpostare la password è necessario un indirizzo e-mail valido. È possibile accedere a questi account solo utilizzando la funzione Accedi come.

   * Elimina utenti non necessari

     >[!IMPORTANT]
     >
     >Scegliere questa opzione solo per i conti creati per errore o per i conti di test. Questa opzione viene in genere eseguita solo per gli account con zero o 1 accesso errato. Gli account che sono stati utilizzati regolarmente non dovrebbero mai essere cancellati.

Se in un’istanza di Workfront sono presenti utenti con indirizzi e-mail corrispondenti che si differenziano solo per maiuscole e minuscole, Workfront ti contatterà con informazioni aggiuntive e una timeline quando è necessario aggiornarli.
