---
product-area: projects
navigation-topic: financials
title: Modificare la valuta del progetto
description: In qualità di Project Manager, puoi configurare un progetto in modo che utilizzi una valuta diversa da quella predefinita per il sistema Adobe Workfront. Questo consente di visualizzare le informazioni finanziarie sul progetto nella valuta desiderata durante il calcolo dei costi della manodopera e dei ricavi.
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: dc71072107ce80f6cb9033fcb17fe4ac74d5af18
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 7%

---

# Modificare la valuta del progetto

In qualità di Project Manager, puoi configurare un progetto in modo che utilizzi una valuta diversa da quella predefinita per il sistema Adobe Workfront. Questo consente di visualizzare le informazioni finanziarie sul progetto nella valuta desiderata durante il calcolo dei costi della manodopera e dei ricavi.

Prima di poter utilizzare valute alternative come descritto in questa sezione, l&#39;amministratore di Workfront deve innanzitutto abilitare e configurare più valute, come descritto nell&#39;articolo [Imposta tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi </td> 
  </tr> 
  <tr> 
   <td>Licenza di Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica accesso ai progetti</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Gestire le autorizzazioni per il progetto</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerazioni durante la modifica della valuta di un progetto in Workfront

* Non è possibile modificare la valuta di un progetto se sono presenti informazioni finanziarie nel progetto.
* I tassi vengono utilizzati per il costo della manodopera, il calcolo dei ricavi e la generazione di rapporti.
* Se non si specifica una valuta diversa per un progetto, Workfront presuppone che la valuta del progetto sia la valuta predefinita del sistema. Per informazioni sulla valuta predefinita a livello di sistema, vedere [Impostare i tassi di cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Per impostazione predefinita, tutti gli utenti con licenza completa hanno accesso alla visualizzazione delle valute e dei tassi di cambio. L&#39;amministratore di Workfront deve concedere un accesso amministrativo aggiuntivo per **Tassi di cambio** per consentire agli utenti di impostare tassi specifici sui progetti.
* I tassi di cambio in Workfront non sono dinamici. Il valore viene impostato da un amministratore e deve essere aggiornato quando si verificano modifiche nei tassi di cambio.
* Se le date di validità vengono applicate a una valuta e ai relativi tassi di cambio, il tasso di cambio potrebbe cambiare durante la durata del progetto. Per informazioni sui tassi di cambio con data di validità, vedere [Impostare i tassi di cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Quando si crea un report per riflettere la valuta in un progetto, per impostazione predefinita tutti i report sono raggruppati in base alla valuta predefinita del progetto. Se si crea un report con più progetti con tassi di cambio diversi, tutti i raggruppamenti applicati al progetto riflettono il tasso di cambio predefinito a livello di sistema. Per ulteriori informazioni, vedere l&#39;articolo [Creare report di dati finanziari con tassi di cambio univoci](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configurare la valuta per un progetto

1. Vai al progetto in cui desideri modificare la valuta predefinita.

   >[!TIP]
   >
   >Verificare che il progetto non contenga già informazioni finanziarie. Ad esempio, accertati che al progetto non siano associati costi pianificati o effettivi.

1. Fai clic su **Dettagli progetto** nel pannello a sinistra, quindi vai all&#39;area **Finanza**.
1. Fare clic su **Aggiungi** nel campo **Valuta** e selezionare la valuta che si desidera utilizzare come valuta predefinita per il progetto. Vengono visualizzate tutte le valute impostate dall’amministratore di Workfront per l’istanza di Workfront.

   ![Valuta nel progetto](assets/currency-on-project.png)

1. (Condizionale) Se si seleziona una valuta diversa da quella predefinita impostata per il sistema Workfront, specificare il tasso per la valuta selezionata, in quanto si riferisce alla valuta impostata come valuta di base nel sistema.

   >[!NOTE]
   >
   >Se per questo progetto è attivata l&#39;impostazione **Usa tassi di cambio validi per data dal sistema**, le sostituzioni dei tassi di cambio non sono consentite. Per ulteriori informazioni, vedere [Modifica progetti](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

1. Fai clic su **Salva modifiche**.
