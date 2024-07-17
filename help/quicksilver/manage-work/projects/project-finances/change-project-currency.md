---
product-area: projects
navigation-topic: financials
title: Modificare la valuta del progetto
description: In qualità di Project Manager, puoi configurare un progetto in modo che utilizzi una valuta diversa da quella predefinita per il sistema Adobe Workfront. Questo consente di visualizzare le informazioni finanziarie sul progetto nella valuta desiderata durante il calcolo dei costi della manodopera e dei ricavi.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Modificare la valuta del progetto

In qualità di Project Manager, puoi configurare un progetto in modo che utilizzi una valuta diversa da quella predefinita per il sistema Adobe Workfront. Questo consente di visualizzare le informazioni finanziarie sul progetto nella valuta desiderata durante il calcolo dei costi della manodopera e dei ricavi.

Prima di poter utilizzare valute alternative come descritto in questa sezione, l&#39;amministratore di Workfront deve innanzitutto abilitare e configurare più valute, come descritto nell&#39;articolo [Imposta tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Requisiti di accesso

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Piano Adobe Workfront*</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso*</td> 
   <td> <p>Modifica accesso ai progetti</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Considerazioni durante la modifica della valuta di un progetto in Workfront

* Non è possibile modificare la valuta di un progetto se sono presenti informazioni finanziarie nel progetto.
* I tassi vengono utilizzati per il calcolo dei costi della manodopera e dei ricavi e vengono utilizzati in futuro a scopo di reporting.
* Se non si specifica una valuta diversa per un progetto, Workfront presuppone che la valuta del progetto sia la valuta predefinita del sistema. Per informazioni sulla valuta predefinita a livello di sistema, vedere [Impostare i tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Per impostazione predefinita, tutti gli utenti con licenza completa hanno accesso alla visualizzazione delle valute e dei tassi di cambio. L&#39;amministratore di Workfront deve concedere un accesso amministrativo aggiuntivo per **Tassi di cambio** per consentire agli utenti di impostare tassi specifici sui progetti.
* I tassi di cambio in Workfront non sono dinamici. Il valore viene impostato da un amministratore e deve essere aggiornato quando si verificano modifiche nei tassi di cambio.
* Quando si crea un report per riflettere la valuta in un progetto, per impostazione predefinita tutti i report sono raggruppati in base alla valuta predefinita del progetto. Se si crea un report con più progetti con tassi di cambio diversi, tutti i raggruppamenti applicati al progetto riflettono il tasso di cambio predefinito a livello di sistema. Per ulteriori informazioni, vedere l&#39;articolo [Creare report di dati finanziari con tassi di cambio univoci](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configurare la valuta per un progetto

1. Vai al progetto in cui desideri modificare la valuta predefinita.

   >[!TIP]
   >
   >Verificare che il progetto non contenga già informazioni finanziarie. Ad esempio, accertati che al progetto non siano associati costi pianificati o effettivi.

1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi vai all&#39;area **Finanza**.
1. Fare clic su **Aggiungi** nel campo **Valuta** e selezionare la valuta che si desidera utilizzare come valuta predefinita per il progetto. Vengono visualizzate tutte le valute impostate dall’amministratore di Workfront per l’istanza di Workfront.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Condizionale) Se si seleziona una valuta diversa da quella predefinita impostata per il sistema Workfront, specificare il tasso per la valuta selezionata, in quanto si riferisce alla valuta impostata come valuta di base nel sistema.
1. Fai clic su **Salva modifiche**.
