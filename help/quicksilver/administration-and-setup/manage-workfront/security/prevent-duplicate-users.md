---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Impedisci agli utenti duplicati
description: Quando crei un nuovo utente in Adobe Workfront, non puoi più utilizzare un indirizzo e-mail già utilizzato da un altro utente, anche se l’indirizzo e-mail varia a seconda dei casi (ad esempio, JohnDoe@example.com e johndoe@example.com). Inoltre, per preparare i miglioramenti futuri dell’autenticazione, assicurati che tutti gli utenti abbiano indirizzi e-mail univoci in un’istanza di Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6f5b9e7638a85eca16d722cec6185cd5ed755eca
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Impedisci agli utenti duplicati

Quando crei un nuovo utente in Adobe Workfront, non puoi più utilizzare un indirizzo e-mail già utilizzato da un altro utente, anche se l’indirizzo e-mail varia a seconda dei casi (ad esempio, JohnDoe@example.com e johndoe@example.com). Inoltre, per preparare i miglioramenti futuri dell’autenticazione, assicurati che tutti gli utenti abbiano indirizzi e-mail univoci in un’istanza di Workfront.

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

## Procedura dettagliata

<!--WRITER
<iframe class="vimeo-player_0" src="assets/371505632?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>
-->

[Guarda un video dimostrativo di questa funzione.](https://vimeo.com/371505632/2e6938ce06)

## Creare utenti con indirizzi e-mail univoci

A partire dalla versione 2019.4, quando crei un nuovo utente in Workfront, non puoi più utilizzare un indirizzo e-mail già utilizzato da un altro utente, anche se l’indirizzo e-mail varia a seconda dei casi. Ad esempio, non puoi creare un utente con l’indirizzo e-mail JohnDoe@example.com se un altro utente ha l’indirizzo e-mail johndoe@example.com.

## Aggiorna gli indirizzi e-mail degli utenti esistenti nella tua istanza Workfront

In qualità di amministratore di Workfront, devi aggiornare gli utenti esistenti che hanno indirizzi e-mail corrispondenti che differiscono solo per caso.
Per correggere gli indirizzi e-mail duplicati all’interno di un’istanza di Workfront:

1. Esamina gli utenti duplicati e decidi quale utente non è più necessario.

   1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Workfront, quindi fai clic su **Utenti**. ![](assets/users-icon-in-main-menu.png)

   1. In **Filtro** menu, seleziona **Tutto**.

   1. In **Visualizza** menu, seleziona **Accesso utente**.

   1. In **Raggruppamento** menu, seleziona **Niente**.

   1. Personalizza la visualizzazione Accesso utente.

      1. Fai clic su **Visualizza** > **Personalizza visualizzazione**.

      1. Sostituisci il **ID** con **Indirizzo e-mail** colonna.

      1. Rinomina la visualizzazione e salvala.
   1. Crea un nuovo raggruppamento.

      1. Fai clic su **Raggruppamento** > **Nuovo raggruppamento**.

      1. Fai clic su **Passa alla modalità testo** nell’angolo superiore destro della pagina.
      1. Incolla il seguente codice della modalità testo:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. Rinomina il raggruppamento e salvalo.



1. Effettua una delle seguenti operazioni:

   * (metodo preferito) Aggiungi un indirizzo + all’indirizzo e-mail dell’utente per ogni account aggiuntivo.

      Scegli questa opzione se un singolo utente dell’organizzazione deve avere accesso a più di 1 account utente. Se l&#39;indirizzo più non è supportato dal provider di posta elettronica, devi fornire un account e-mail separato per ciascun account Workfront.

      Ad esempio, John Doe può avere un account utente per il suo account di utilizzo giornaliero e uno da utilizzare a scopo di test:

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * Modifica il dominio per utilizzare un dominio falso aggiungendo il seguente testo all&#39;indirizzo e-mail:

      `.inactive`

      Ad esempio, John Doe potrebbe avere i seguenti domini: (devono essere univoci).

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      Non è più possibile accedere a questi account perché i reinsiemi di password richiedono un indirizzo e-mail valido. Per accedere a questi account è possibile utilizzare la funzione Accedi come .

   * Eliminare gli utenti non necessari

      >[!IMPORTANT]
      >
      >Scegliere questa opzione solo per gli account creati per errore o per gli account di test. Questa opzione di solito viene eseguita solo per gli account con accesso errato pari a zero o 1. Gli account utilizzati regolarmente non devono mai essere eliminati.



Se disponi di utenti in un’istanza di Workfront con indirizzi e-mail corrispondenti che differiscono solo per caso, Workfront ti contatterà con informazioni aggiuntive e una timeline quando questi devono essere aggiornati.
