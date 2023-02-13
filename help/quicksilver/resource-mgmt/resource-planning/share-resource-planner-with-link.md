---
product-area: resource-management
navigation-topic: resource-planning
title: Condividere la visualizzazione utente di Resource Planner con un collegamento
description: Adobe Workfront può generare un URL univoco per la visualizzazione utente del planner risorse che è possibile incorporare in un dashboard come pagina esterna oppure aprirlo separatamente in una nuova scheda del browser. È utile quando si condividono le informazioni del Planner risorse con utenti che potrebbero non avere accesso diretto all'area Risorse.
author: Alina
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# Condividere la visualizzazione utente di Resource Planner con un collegamento

Adobe Workfront può generare un URL univoco per la visualizzazione utente del planner risorse che è possibile incorporare in un dashboard come pagina esterna oppure aprirlo separatamente in una nuova scheda del browser. È utile quando si condividono le informazioni del Planner risorse con utenti che potrebbero non avere accesso diretto all&#39;area Risorse.

![](assets/rp-user-view-with-link-highlight-350x49.png)

## Requisiti di accesso

Devi disporre dei seguenti elementi:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront*</td> 
   <td> <p>Pro e superiore</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront*</td> 
   <td> <p>Piano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni a livello di accesso*</td> 
   <td> <p>Visualizza o un accesso più elevato a Gestione risorse, Progetti e Utenti</p> <p>Visualizzazione dell'accesso ai dati finanziari per visualizzare le informazioni sui costi </p> <p><b>NOTA</b> Se non disponi ancora dell’accesso, chiedi all’amministratore Workfront se ha impostato ulteriori restrizioni nel livello di accesso. Per informazioni su come un amministratore Workfront può modificare il livello di accesso, consulta <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per i progetti che desideri visualizzare nel Planner risorse</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedi <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l’accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per informazioni sul piano, il tipo di licenza o l&#39;accesso, contattare l&#39;amministratore Workfront.


Quando si genera l&#39;URL univoco per la visualizzazione utente del planner risorse, tenere presente quanto segue:

* Puoi ottenere un URL univoco solo per la visualizzazione utente. L’opzione per generare l’URL non esiste nelle visualizzazioni Progetto o Ruolo .
* Puoi condividere l’URL con altri utenti, inclusi gli utenti con licenza Work e Review.\
   Per visualizzare le informazioni nel Planner risorse dall&#39;URL condiviso con gli utenti, gli utenti devono disporre dell&#39;accesso per visualizzare gli altri utenti.
* Le seguenti informazioni vengono salvate quando condividi l’URL con altri utenti:

   * Il tipo di periodi di tempo (settimana, mese, trimestre).
   * I filtri applicati.
   * Tipo di visualizzazione (ore o FTE).

Per ottenere un URL univoco nella visualizzazione utente del planner risorse e condividerlo con altri utenti:

1. Fai clic sul pulsante **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo in alto a destra di Adobe Workfront.

1. Fai clic su **Risorsa**.
1. In , seleziona **Visualizza per utente**.
1. (Facoltativo) Selezionare l&#39;intervallo di tempo in base al quale visualizzare le informazioni nel Planner risorse. Seleziona una delle seguenti opzioni:

   * Settimana
   * Mese
   * Trimestre

1. (Facoltativo) Seleziona se desideri visualizzare le informazioni in base a **FTE** o **Ore**.\
   ![RP_hours_or_fte_in_user_view.png](assets/rp-hours-or-fte-in-user-view.png)

1. (Facoltativo) Applicare filtri al planner risorse.\
   Per informazioni sull’applicazione dei filtri, consulta [Filtrare le informazioni nel planner risorse](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

1. Fai clic sul pulsante **collegamento ipertestuale** icona.\
   ![RP_Storm_generate_URL_with_copy_URL_link.png](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. Fai clic su **Copia URL**.\
   In questo modo viene copiato negli Appunti l’URL univoco del planner risorse nella visualizzazione utente.

1. (Facoltativo) Effettua una delle seguenti operazioni:  

   * Incolla l’URL in un’altra applicazione per inviarlo a un altro utente.\
      Per visualizzare il Planner risorse nella visualizzazione Utente, l’utente deve aver effettuato l’accesso a Workfront.
   * Apri una nuova scheda o finestra del browser e incolla il collegamento copiato, quindi fai clic su Invio sulla tastiera per aprire il Planner risorse in una nuova scheda o finestra.
   * Effettua le seguenti operazioni:

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. Vai a **Reporting**>**Dashboard**>**Nuovo dashboard**>**Aggiungi pagina esterna.**

      1. Incolla il collegamento copiato negli Appunti nella **URL** campo .
      1. Fai clic su **Salva**, quindi **Salva e chiudi**.\
         In questo modo l’URL verrà incorporato nel dashboard e la visualizzazione Utente del Planner risorse verrà visualizzata in un dashboard separato.

1. (Facoltativo) Se l&#39;URL è stato incorporato in un dashboard, è consigliabile aggiungerlo a un modello di layout o condividerlo con altri utenti che potrebbero non avere accesso all&#39;area Gestione risorse.\
   Per informazioni sull’aggiunta di dashboard a un modello di layout, consulta [Creare e gestire modelli di layout](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) .\
   Per informazioni sulla condivisione delle dashboard, consulta [Condivisione di un dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) .\
   Quando si visualizza l&#39;URL condiviso, gli utenti possono visualizzare le informazioni con le impostazioni originariamente applicate al planner risorse. Per visualizzare l&#39;URL condiviso, è necessario aver effettuato l&#39;accesso a Workfront.\
   ![user_view_dashoard_from_unique_url.png](assets/user-view-dashoard-from-unique-url-350x85.png)
