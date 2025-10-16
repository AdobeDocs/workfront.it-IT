---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configurare l’accesso ai blueprint
description: In qualità di amministratore di sistema, puoi consentire agli utenti di richiedere l’installazione di blueprint impostando una coda di richieste per archiviare le richieste. In questa posizione, puoi tenere traccia e aggiornare le richieste da un’unica posizione.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: 5fd855bec596926a4361fd07a1a763c7956e5e61
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Configurare l’accesso ai blueprint

Tutti gli utenti di [!DNL Adobe Workfront] possono sfogliare il catalogo di blueprint.

In qualità di amministratore di sistema, puoi:

* Aggiungi [!UICONTROL Blueprint] al menu principale nei modelli di layout e assegna il modello di layout a utenti o gruppi. Per ulteriori informazioni, vedere [Personalizzare il [!UICONTROL menu principale] utilizzando un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) e [Assegnare gli utenti a un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

  >[!NOTE]
  >
  >* Agli utenti ai quali non è stato assegnato un modello di layout verrà visualizzata l&#39;icona [!UICONTROL Blueprint] nel [!UICONTROL menu principale].
  >* Quando si crea un nuovo modello di layout, per impostazione predefinita l&#39;icona [!UICONTROL Blueprints] è inclusa nell&#39;elenco [!UICONTROL Elementi attivi] per il [!UICONTROL menu principale].


* Consenti agli utenti di richiedere l’installazione dei blueprint impostando una coda di richieste per archiviare le richieste. In questa posizione, puoi tenere traccia e aggiornare le richieste da un’unica posizione. Per ulteriori informazioni, attenersi alla procedura descritta di seguito.
* Installa i blueprint. Per informazioni, vedere [Installare una blueprint](../../administration-and-setup/blueprints/blueprints-install.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Piano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td>Amministratore Workfront </td> 
  </tr> 
 </tbody> 
</table>

Per ulteriori dettagli sulle informazioni contenute in questa tabella, vedere [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisiti {#prerequisites}

* Per archiviare le richieste blueprint è necessario utilizzare una coda di richieste esistente. Il progetto deve essere salvato come coda di richieste e deve essere nello stato [!UICONTROL Corrente].
* La coda di richieste deve essere pubblica. Nei dettagli della coda richieste, &quot;[!UICONTROL Chi può aggiungere richieste a questa coda?]&quot; deve essere impostato su **[!UICONTROL Chiunque]**.

>[!TIP]
>
>Se desideri creare una nuova coda di richieste per le richieste blueprint, devi generarla prima di configurare l’accesso ai blueprint. Per informazioni sulla creazione di una coda richieste, vedere [Creare una coda richieste](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Seleziona la coda di richieste per archiviare le richieste blueprint

Prima che gli utenti possano richiedere l’installazione dei blueprint, è necessario selezionare una coda di richieste per tali richieste. Fino a quando la coda di richieste non è definita, gli utenti possono solo sfogliare il catalogo blueprint.

{{step1-to-blueprints}}

1. Fai clic su **[!UICONTROL Configura richieste blueprint]** in alto a destra nella schermata del catalogo.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. Nella finestra di dialogo **[!UICONTROL Configura blueprint]**, inizia a digitare il nome di una coda di richieste attiva e selezionala quando viene visualizzata nei risultati della ricerca.

   >[!IMPORTANT]
   >
   >In questo elenco vengono visualizzate solo le code di richieste pubbliche. Per rendere pubblica la coda di richieste, vedi la sezione [Prerequisiti](#prerequisites) precedente.

   È stata impostata la preferenza per la coda di richieste ed è ora possibile richiedere l’installazione di blueprint.

   ![Configura coda richieste](assets/Blueprints_access_setup_request_queue.png)

1. (Facoltativo) Per apportare modifiche alla coda richieste effettiva, fare clic su **[!UICONTROL Modifica coda richieste]**.

   Il progetto della coda richieste viene aperto in una nuova scheda del browser e puoi aggiornarlo in base alle esigenze.

1. (Facoltativo) Se la coda di richieste contiene gruppi di argomenti o argomenti della coda, è possibile selezionarli dall&#39;elenco.
1. Per tornare al catalogo blueprint, fai clic su **[!UICONTROL Chiudi]**.

>[!NOTE]
>
>Quando installi una blueprint richiesta, devi modificare lo stato del problema in **[!UICONTROL Chiuso]** o **[!UICONTROL Risolto]** nella coda richieste in modo che il richiedente riceva una notifica. Per informazioni sull&#39;installazione di una blueprint, vedere [Installare una blueprint](../../administration-and-setup/blueprints/blueprints-install.md).
