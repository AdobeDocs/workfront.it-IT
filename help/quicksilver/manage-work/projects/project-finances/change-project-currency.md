---
product-area: projects
navigation-topic: financials
title: Modificare la valuta del progetto
description: In qualità di Project Manager, puoi configurare un progetto per l’utilizzo di una valuta diversa da quella predefinita per il sistema Adobe Workfront. Questo consente di visualizzare le informazioni finanziarie sul progetto nella valuta desiderata quando si calcolano i costi del lavoro e i ricavi.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Modificare la valuta del progetto

In qualità di Project Manager, puoi configurare un progetto per l’utilizzo di una valuta diversa da quella predefinita per il sistema Adobe Workfront. Questo consente di visualizzare le informazioni finanziarie sul progetto nella valuta desiderata quando si calcolano i costi del lavoro e i ricavi.

Prima di poter utilizzare le valute alternative come descritto in questa sezione, l&#39;amministratore di Workfront deve prima abilitare e configurare più valute, come descritto nell&#39;articolo [Imposta i tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Modifica accesso a progetti</p> <p>Nota: Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.

## Considerazioni sulla modifica della valuta di un progetto in Workfront

* Non è possibile modificare la valuta di un progetto se nel progetto sono presenti informazioni finanziarie.
* I tassi sono utilizzati per i costi del lavoro; Calcoli dei ricavi e vengono utilizzati in futuro a scopo di reporting.
* Se non si specifica una valuta diversa per un progetto, Workfront presuppone che la valuta del progetto sia la valuta predefinita del sistema. Per informazioni sulla valuta predefinita a livello di sistema, vedere [Imposta i tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Per impostazione predefinita, tutti gli utenti con licenza completa hanno accesso alla visualizzazione di valute e tassi di cambio. L’amministratore di Workfront deve concedere un accesso amministrativo aggiuntivo per **Tassi di cambio** per consentire agli utenti di impostare tassi specifici sui progetti.
* I tassi di cambio in Workfront non sono dinamici. Il valore viene impostato da un amministratore e deve essere aggiornato quando si verificano modifiche ai tassi di cambio.
* Quando si crea un rapporto per riflettere la valuta di un progetto, per impostazione predefinita tutti i rapporti sono raggruppati in base alla valuta predefinita del progetto. Se si crea un rapporto con più progetti con tassi di cambio diversi, tutti i raggruppamenti applicati al progetto riflettono il tasso di cambio predefinito a livello di sistema. Per ulteriori informazioni, consulta l’articolo [Creare rapporti di dati finanziari con tassi di cambio univoci](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configurare la valuta per un progetto

1. Passa al progetto in cui desideri modificare la valuta predefinita.

   >[!TIP]
   >
   >Assicurati che il progetto non disponga già di informazioni finanziarie. Ad esempio, assicurati che non vi siano costi pianificati o effettivi associati al progetto.

1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi vai alla **Finanza** area.
1. Fai clic su **Aggiungi** in **Valuta** e selezionare la valuta che si desidera utilizzare come valuta predefinita per il progetto. Vengono visualizzate tutte le valute impostate dall’amministratore di Workfront per l’istanza Workfront.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Condizionale) Se si seleziona una valuta diversa da quella predefinita impostata per il sistema Workfront, specificare il tasso per la valuta selezionata, in quanto si riferisce alla valuta impostata come valuta di base nel sistema.
1. Fai clic su **Salva modifiche**.
