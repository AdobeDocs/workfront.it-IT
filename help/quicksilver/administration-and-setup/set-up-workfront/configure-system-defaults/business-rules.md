---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Creare e modificare le regole business
description: È possibile scegliere se ricevere nuove funzionalità Workfront con frequenza mensile o trimestrale.
author: Lisa
feature: System Setup and Administration
role: Admin
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d96ddcc2f514d9f79e94a3437a3b66e07a270abc
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Creare e modificare le regole business

Una regola business consente di applicare la convalida agli oggetti di Workfront e di impedire agli utenti di creare, modificare o eliminare un oggetto quando vengono soddisfatte determinate condizioni. Le regole aziendali contribuiscono a migliorare la qualità dei dati e l’efficienza operativa impedendo azioni che potrebbero compromettere l’integrità dei dati.

Una singola regola business può essere assegnata a un solo oggetto. Ad esempio, se si crea una regola business per non modificare i progetti in determinate condizioni, non è possibile applicare la stessa regola alle attività. È necessario creare una regola business separata con le stesse condizioni per le attività.

I livelli di accesso e la condivisione degli oggetti hanno una priorità più alta rispetto alle regole di business quando un utente interagisce con un oggetto. Ad esempio, se un utente dispone di un livello di accesso o di un’autorizzazione che non consente la modifica di un progetto, questi hanno la precedenza su una regola business che consente la modifica di un progetto in determinate condizioni.

Una gerarchia esiste anche quando a un oggetto vengono applicate più regole business. Ad esempio, sono disponibili due regole business. Uno limita la creazione di spese nel mese di febbraio. La seconda impedisce la modifica di un progetto quando lo stato del progetto è Completo. Se un utente tenta di aggiungere una spesa a un progetto completato nel mese di giugno, la spesa non può essere aggiunta perché ha attivato la seconda regola.

Le regole business si applicano alla creazione, modifica ed eliminazione di oggetti tramite l’API e nell’interfaccia di Workfront.

>[!NOTE]
>
>Poiché le regole business bloccano alcune azioni, è sempre necessario configurare le regole business prima in un ambiente sandbox o di anteprima e testarle completamente prima di abilitarle in produzione.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>piano Adobe Workfront</td> 
   <td>Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licenza Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Amministratore di sistema</td> 
  </tr>  
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Scenari per le regole business

Alcuni semplici scenari di regole di business sono:

* Gli utenti non possono aggiungere nuove spese durante l&#39;ultima settimana di febbraio. Questa formula potrebbe essere così formulata: `IF(AND(MONTH($$TODAY) = 2, DAYOFMONTH($$TODAY) >= 22), "You cannot add new expenses during the last week of February.")`
* Gli utenti non possono modificare un progetto che si trova nello stato Completato. Questa formula potrebbe essere così formulata: `IF({status} = "CPL", "You cannot edit this project because it is in Complete status.")`

La sintassi per la creazione di una regola business è la stessa della creazione di un campo calcolato in un modulo personalizzato. Per ulteriori informazioni sulla sintassi, consulta [Aggiungere campi calcolati con il progettista del modulo](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Per informazioni sulle istruzioni IF, vedere [Panoramica delle istruzioni &quot;IF&quot;](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) e [Operatori condizione nei campi personalizzati calcolati](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Per informazioni sui caratteri jolly basati sull&#39;utente, vedere [Utilizzare caratteri jolly basati sull&#39;utente per generalizzare i rapporti](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Per informazioni sui caratteri jolly basati sulla data, vedere [Utilizzare caratteri jolly basati sulla data per generalizzare i rapporti](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

## Aggiungere una nuova regola business

{{step-1-to-setup}}

1. Clic **Regole aziendali** nel pannello a sinistra.
1. Clic **Nuova regola business**.
1. Selezionare il tipo di oggetto a cui assegnare la regola business, quindi fare clic su **Continua**.

   ![Seleziona un oggetto](assets/object-for-business-rule2.png)

1. Digita il **Nome** per la regola business.
1. In **È attivo** , selezionare se la regola deve essere attiva al momento del salvataggio.

   Se si seleziona **No**, la regola viene salvata come inattiva e puoi attivarla in un secondo momento.

1. Seleziona un **Trigger** per la regola business. Le opzioni sono:

   * **Durante la creazione dell&#39;oggetto:** La regola viene applicata quando un utente tenta di creare un oggetto.
   * **Alla modifica dell&#39;oggetto:** La regola viene applicata quando un utente tenta di modificare un oggetto.
   * **All&#39;eliminazione dell&#39;oggetto:** La regola viene applicata quando un utente tenta di eliminare un oggetto.

1. (Facoltativo) Inserisci un **Descrizione** della regola business e ciò che accade quando viene applicata.
1. Crea la formula nell’editor di formule, al centro della finestra di dialogo della regola business.

   Il formato di una regola business è &quot;Se la condizione definita viene soddisfatta, l&#39;utente non è in grado di eseguire l&#39;azione sull&#39;oggetto e viene visualizzato il messaggio&quot;.

   Nell&#39;area della formula, le parti della regola business creata sono la condizione e il messaggio visualizzato in Workfront quando la condizione viene soddisfatta.

   * L&#39;&quot;oggetto&quot; è il tipo di oggetto selezionato durante la creazione della regola business. Viene visualizzato nell’intestazione della finestra di dialogo.
   * L’&quot;azione&quot; è il trigger selezionato per la regola: crea, modifica o elimina l’oggetto.
   * Poiché l&#39;oggetto e l&#39;azione sono già definiti, non vengono inclusi nella formula.
   * Il messaggio di errore personalizzato viene visualizzato quando l&#39;utente attiva la regola business. Dovrebbe fornire istruzioni chiare su cosa è andato storto e su come correggere il problema.

   ![Finestra di dialogo Aggiungi regola business](assets/add-business-rule-dialog-no-ai-button.png)

   Questo esempio è una regola business per le spese. Se il mese corrente è giugno, agli utenti non è consentito creare nuove spese, e questo viene spiegato nel messaggio.

   Per ulteriori esempi di regole business, consulta [Scenari per le regole business](#scenarios-for-business-rules) in questo articolo.

1. (Facoltativo) Usa la formula **Espressioni** e **Campi** nel pannello a destra per assistenza nella creazione della regola.

   Cerca un&#39;espressione o un campo per restringere l&#39;elenco degli elementi disponibili.

   L&#39;elenco dei campi disponibili è limitato ai campi correlati al tipo di oggetto per la regola business.

1. Clic **Salva** al termine della creazione della regola business.

>[!NOTE]
>
>Dopo aver aggiunto una regola business, è necessario verificarla aggiungendo, modificando o eliminando l&#39;oggetto associato per assicurarsi che la regola venga applicata correttamente.

## Attivare una regola business

Quando una regola business è inattiva, il campo È attivo nell&#39;elenco delle regole business visualizza False. Impossibile aggiornare lo stato della regola nella vista a elenco.

Per attivare una regola business:

1. Selezionare la regola business nell&#39;elenco di regole e fare clic sull&#39;icona Modifica.
1. Seleziona **Sì** per **È attivo** nella finestra di dialogo regola business.
1. Fai clic su **Salva**.
