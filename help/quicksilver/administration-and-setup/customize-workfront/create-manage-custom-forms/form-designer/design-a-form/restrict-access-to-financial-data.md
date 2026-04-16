---
title: Limitare l’accesso ai dati finanziari nei campi personalizzati
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Quando si crea un campo personalizzato, è possibile definire impostazioni facoltative per limitare l'accesso ai dati finanziari.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3380cce6-8372-43c0-8520-473442ea0eb4
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 9%

---

# Limitare l’accesso ai dati finanziari nei campi personalizzati

Quando si crea un campo personalizzato, è possibile definire impostazioni facoltative per limitare l&#39;accesso ai dati finanziari. In questo modo, gli utenti che dispongono di determinate autorizzazioni impostate nei loro livelli di accesso possono visualizzare i dati e non possono visualizzare dati finanziari a cui non dovrebbero avere accesso.

Per informazioni sulla creazione di un campo personalizzato, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Per informazioni sui livelli di accesso, vedere [Panoramica sui livelli di accesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md). Per informazioni sulla condivisione e sulle autorizzazioni, vedere [Panoramica sulle autorizzazioni di condivisione per gli oggetti](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr>  
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Piano</p></td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Accesso amministrativo ai moduli personalizzati</td> 
  </tr>  
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limitare l’accesso ai dati finanziari in un campo personalizzato

1. Crea un nuovo modulo personalizzato o apri un modulo esistente.

   Per informazioni, vedere [Creare un modulo personalizzato](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Aggiungi un campo personalizzato al modulo o seleziona un campo esistente.

   Questi tipi di campo possono essere limitati in base all’accesso ai dati finanziari:

   * Testo su riga singola
   * Paragrafo
   * Elenco a discesa a selezione singola
   * Elenco a discesa a selezione multipla
   * Gruppo di caselle di controllo
   * Pulsanti di scelta
   * Ricerca esterna
   * Ricerca esterna a selezione multipla
   * Calcolato

1. Nel campo **Formato**, selezionare **Valuta**.

   >[!NOTE]
   >
   >Per i campi calcolati, è consentito qualsiasi formato. Tutti gli altri tipi di campo devono utilizzare il formato **Valuta**, altrimenti il campo **Tipo di autorizzazione Finanziaria** non sarà disponibile.

1. (Facoltativo) Solo per i campi calcolati, attivare l&#39;opzione **Autorizzazione automatica** per consentire alle autorizzazioni per contabilità di provenire automaticamente dai campi della formula.

1. Selezionare un&#39;opzione per il tipo di autorizzazione **Finanza**.

   Gli utenti devono disporre di questo tipo di autorizzazione per il finanziamento prima di poter visualizzare o modificare il campo personalizzato nel modulo.

   * **Nessuna autorizzazione richiesta:** Tutti gli utenti possono visualizzare questo campo
   * **Generale:** gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le informazioni di contabilità generale
   * **Fatturazione:** gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le tariffe di fatturazione
   * **Costo:** gli utenti devono disporre delle autorizzazioni per modificare o visualizzare le tariffe

   Per i campi calcolati:

   * Il campo **Tipo di autorizzazione per contabilità** non è disponibile per l&#39;impostazione manuale delle autorizzazioni se il campo **Autorizzazione automatica** è attivato.
   * I campi utilizzati nella formula determinano se il campo delle autorizzazioni è attivo. Se il campo delle autorizzazioni è vuoto e le autorizzazioni automatiche non sono attivate, i campi della formula non supportano le autorizzazioni per la contabilità.
   * L&#39;accesso è obbligatorio per tutti i campi della formula. Ad esempio, se due campi vengono utilizzati in un campo calcolato e a uno di essi è applicata l’autorizzazione di fatturazione e al secondo è applicata l’autorizzazione di costo, l’utente deve disporre delle autorizzazioni per visualizzare sia la fatturazione che le tariffe per visualizzare il valore calcolato.

1. Per salvare le modifiche, fai clic su **Applica** e continua a creare il modulo.

   Oppure

   Fai clic su **Salva e chiudi**.

## Esempio

Due progetti sono condivisi con un utente:

* L&#39;utente dispone delle autorizzazioni per modificare tutte le opzioni di finanziamento per il primo progetto
* L’utente dispone delle autorizzazioni necessarie per visualizzare le tariffe di fatturazione e le informazioni finanziarie generali per il secondo progetto

Quando l’utente modifica il primo progetto, tutti i campi finanziari nel modulo personalizzato sono modificabili. Quando l&#39;utente modifica il secondo progetto, i campi impostati su **Fattura** o **Generale** sono di sola visualizzazione e i campi impostati su **Costo** non sono visibili.

Quando l’utente visualizza i progetti in un elenco o in un rapporto:

* I campi finanziari sono visualizzabili o modificabili in base alle autorizzazioni e alle impostazioni del rapporto
* I campi finanziari sono vuoti se l’utente non dispone delle autorizzazioni necessarie per visualizzarli

L’esportazione dei dettagli del progetto mostra gli stessi valori dei campi finanziari (o campi vuoti) dell’elenco.

Durante la modifica in blocco di entrambi i progetti, i campi Fatturazione e Finanza generale sono di sola lettura e i campi Costo sono N/D.
