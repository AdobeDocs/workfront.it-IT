---
product-area: projects
navigation-topic: manage-tasks
title: Convertire un’attività in un progetto
description: Quando il completamento di un'attività di un progetto richiede una quantità di lavoro maggiore di quella pianificata in origine, è possibile convertirla in un progetto.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: b781687b175167784367a2fdec158d97fb3fd6a4
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 2%

---

# Convertire un’attività in un progetto

Quando il completamento di un&#39;attività di un progetto richiede una quantità di lavoro maggiore di quella pianificata in origine, è possibile convertirla in un progetto.

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
   <td> <p>Modifica accesso ad attività e progetti</p> <p>Accesso di visualizzazione o superiore ai modelli quando si converte in un progetto utilizzando un modello</p> <p>Nota: se non disponi ancora dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Gestire le autorizzazioni per un’attività</p> <p>Visualizzare le autorizzazioni su un modello, se si converte in un progetto utilizzando un modello</p> <p>Dopo aver creato il progetto, disporrai delle autorizzazioni di gestione per il progetto</p> <p>Per informazioni sulla richiesta di accesso aggiuntivo, vedere <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Richiedere l'accesso agli oggetti </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Per conoscere il piano, il tipo di licenza o l&#39;accesso di cui si dispone, contattare l&#39;amministratore di Workfront.

## Considerazioni sulla conversione di attività in progetti

* È possibile convertire un&#39;attività in un progetto vuoto o in un progetto utilizzando un modello.
* L&#39;attività originale viene eliminata.
* Tutte le sotto-attività, le Issues e le Note vengono riportate nel nuovo progetto.
* Documenti, versioni dei documenti e bozze vengono spostati nel nuovo progetto.
* Vengono mantenuti lo stato e la percentuale di completamento di tutte le attività secondarie e dei problemi.
* Gli utenti condivisi dell’attività diventano utenti condivisi nel progetto.
* La data di inizio del progetto viene impostata sulla data di inizio dell&#39;attività.
* Nella tabella seguente sono elencate le informazioni relative al progetto e l&#39;eventuale trasferimento dal modello o dall&#39;attività:

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>Descrizione</td> 
    <td> <p>Descrizione dell'attività trasferita al nuovo progetto. </p> <p> Se l'attività non è descritta, la descrizione del modello viene trasferita al progetto. </p> <p>Se il campo Descrizione è vuoto sia per l'attività che per il modello, il campo del progetto è vuoto. </p> </td> 
    </tr> 
    <tr> 
    <td>Stato</td> 
    <td> Stato predefinito selezionato per il gruppo nel modello. Se il modello non è associato al gruppo, lo stato del progetto viene impostato sullo stato predefinito impostato dall'amministratore di Workfront nell'area Preferenze progetto di Configura. Per informazioni, consulta <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Configurare le preferenze di progetto a livello di sistema</a>

  Esistono i seguenti scenari per aggiornare lo stato del progetto:
  <ul>
    <li> Se lo stato dell'attività è 'Nuovo', lo stato del progetto è impostato su 'Pianificazione'.</li>
    <li> Se lo stato dell'attività è "In corso", lo stato del progetto è "Corrente".</li>
    <li> Se lo stato dell'attività è 'Completato', lo stato del progetto è impostato su 'Completato'.</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>Priorità</td> 
    <td>Trasferisce dall'attività al progetto, oppure viene trasferito dal modello, se ne utilizzi uno nella conversione. </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>L’URL dell’attività viene trasferito al nuovo progetto. </p> <p> Se nell'attività non è specificato alcun URL, l'URL del modello viene trasferito al progetto. </p> <p>Se il campo URL è vuoto sia per il problema che per il modello, il campo è vuoto nel progetto. </p> </td> 
    </tr> 
    <tr> 
    <td>Tipo di condizione progetto</td> 
    <td>Trasferimenti dal modello.</td> 
    </tr> 
    <tr> 
    <td>Condizione progetto</td> 
    <td>Corrisponde alla preferenza predefinita a livello di sistema determinata dall'amministratore di Workfront nell'area Configura. Per informazioni, vedere <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">Impostare una condizione personalizzata come predefinita per i progetti</a>
    </td> 
    </tr> 
    <tr> 
    <td>Pianifica da</td> 
    <td>Trasferimenti dal modello.</td> 
    </tr> 
    <tr> 
    <td>Date progetto</td> 
    <td> 
      <ul> 
      <li> <p><b>Data inizio pianificata</b>: l'orario di lavoro più vicino basato sull'orario di lavoro della pianificazione del modello deve essere preselezionato, in base al fuso orario della pianificazione del modello. Questo campo è disattivato se il campo Pianifica da è impostato su Da completamento. </p> </li> 
      <li> <p><b>Data di completamento pianificata</b>: l'orario di lavoro più vicino basato sull'orario di lavoro della pianificazione del modello deve essere preselezionato, in base al fuso orario della pianificazione del modello. Questo campo è disattivato se il campo Pianifica da è impostato su Da inizio. </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>Portfolio</td> 
    <td>Trasferimenti dal modello. In caso contrario, il campo è vuoto.</td> 
    </tr> 
    <tr> 
    <td>Programma</td> 
    <td>Trasferimenti dal modello. In caso contrario, il campo è vuoto.</td> 
    </tr> 
    <tr> 
    <td>Gruppo</td> 
    <td><p> Esistono i seguenti scenari:</p>
      <ul><li>Se durante la conversione viene specificato un gruppo, questo diventerà il gruppo del progetto</li>
      <li>Se si converte in un progetto utilizzando un modello ed è presente un gruppo nel modello e durante la conversione non si specifica un gruppo, il gruppo del modello diventa il gruppo del nuovo progetto</li>
      <li> Se nel modello non è presente alcun gruppo e non si specifica un gruppo durante la conversione, il gruppo del progetto del problema originale diventa il gruppo del nuovo progetto</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>Azienda</td>    
    <td>  Trasferimenti dal modello. In caso contrario, il campo è vuoto.</td>

  </tr> 
    <tr> 
    <td>Proprietario progetto</td> 
    <td>Trasferimenti dal campo Proprietario modello nel modello. In caso contrario, viene impostato sull’utente connesso che sta eseguendo la conversione. </td> 
    </tr> 
    <tr> 
    <td>Sponsor del progetto</td> 
    <td>Trasferimenti dal campo Sponsor modello nel modello. In caso contrario, il campo è vuoto.</td> 
    </tr> 
    <tr> 
    <td>Responsabile risorse</td> 
    <td>Trasferimenti dal modello. In caso contrario, il campo è vuoto.</td> 
    </tr> 
    <tr> 
    <td>Impostazioni attività</td> 
    <td>Trasferisci dal modello.</td> 
    </tr> 
    <tr> 
    <td>Impostazioni problema</td> 
    <td>Trasferisci dal modello. </td> 
    </tr> 
    <tr> 
    <td>Accesso</td> 
    <td> <p>Trasferimenti dalla sezione Accesso del modello. </p> </td> 
    </tr> 
    <tr> 
    <td>Approvazioni</td> 
    <td>Trasferisci dal modello. Le approvazioni associate all'attività vengono rimosse durante la conversione. </td> 
    </tr> 
  </tbody> 
  </table>


## Convertire un’attività in un progetto

1. Passare all&#39;attività che si desidera convertire in un progetto.
1. Fai clic sull&#39;icona **Altro** ![](assets/more-icon.png), quindi **Converti in progetto**.
1. Scegliere una delle seguenti opzioni:

   * **Nuovo progetto**
   * Un modello nella sezione **Seleziona da modelli**

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Fai clic su **Continua** nella notifica visualizzata.
1. Nella casella **Converti in progetto** specificare quanto segue:

   * **Nome**: assegna un nome al progetto. Il nome predefinito è il nome dell&#39;attività.
   * (Facoltativo) **Descrizione**: descrivi lo scopo del progetto.
   * (Facoltativo e condizionale) Se hai selezionato di creare un progetto da un modello, aggiorna i campi disponibili nella finestra di dialogo **Converti in progetto**.

     Per ulteriori informazioni sulla modifica dei campi nei progetti, vedere [Modifica progetti](../../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Per aggiornare i campi nella sezione Dati finanziari della casella Converti in progetto, è necessario disporre dell&#39;accesso di modifica ai dati finanziari nel proprio livello di accesso. Se si dispone dell&#39;accesso di visualizzazione ai dati finanziari nel proprio livello di accesso, tutte le informazioni finanziarie del modello vengono trasferite al nuovo progetto e non è possibile modificarle durante la conversione del problema. Per informazioni, vedere [Concedere l&#39;accesso ai dati finanziari](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Condividere un modello](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Facoltativo) Aggiungi **Forms personalizzato** al nuovo progetto.

     >[!TIP]
     >
     >Se un modulo personalizzato con più oggetti allegato all&#39;attività è configurato per l&#39;utilizzo sia con le attività che con i progetti, tutte le informazioni salvate nel modulo vengono conservate al momento della conversione.
     >
     >
     >Se utilizzi un modello per la conversione e un modulo personalizzato allegato al modello contiene un campo personalizzato che si trova anche in un modulo personalizzato allegato all’attività, per il nuovo progetto viene utilizzato il valore del campo dell’attività. Tuttavia, se il campo personalizzato è vuoto nell’attività, viene utilizzato il valore del modello.

1. Fai clic su **Salva modifiche**.
