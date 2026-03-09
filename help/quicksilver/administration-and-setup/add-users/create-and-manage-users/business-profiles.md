---
title: Panoramica dei profili aziendali
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: add-users-to-workfront
description: I profili aziendali sono un modello di autorizzazioni avanzato che consente a clienti come le agenzie di gestire in modo efficiente l’accesso degli utenti e garantire un controllo preciso sulle autorizzazioni a livello di gruppo. In un profilo di business, gli utenti dispongono di autorizzazioni distinte per gli oggetti specifici del gruppo. È inoltre possibile condividere oggetti aggiuntivi direttamente con il profilo aziendale.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
exl-id: 7f62de33-e544-4be9-8dcf-03a2e09e8a05
source-git-commit: 1389c6a1f41a14bafd6b70e2e079e40d22d47b07
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 0%

---

# Panoramica dei profili aziendali

<span class="preview">Le informazioni contenute in questa pagina si riferiscono a funzionalità non ancora generalmente disponibili. È disponibile solo nell&#39;ambiente di anteprima per clienti specifici.</span>

I profili aziendali sono un modello di autorizzazioni avanzato che consente a clienti come le agenzie di gestire in modo efficiente l’accesso degli utenti e garantire un controllo preciso sulle autorizzazioni a livello di gruppo. In un profilo di business, gli utenti dispongono di autorizzazioni distinte per gli oggetti specifici del gruppo. È inoltre possibile condividere oggetti aggiuntivi direttamente con il profilo aziendale.

Un profilo di business per un utente è simile a quello di un utente con un ruolo specifico in un gruppo, ad esempio un controllore finanziario o un project manager, e che riceve le autorizzazioni associate a tale ruolo per il gruppo specificato. Il profilo business può essere temporaneo, consentendo le autorizzazioni per un periodo di tempo impostato per scadere e mantenendo le restrizioni sui dati per il gruppo o l’agenzia.

L&#39;amministratore di sistema di Workfront:

* Crea i livelli di accesso e definisce i campi con restrizioni in base alle esigenze
* Aggiorna il profilo utente con il gruppo e il livello di accesso per tale gruppo (questo è il profilo aziendale)
* Definisce le date di validità per il profilo di business in base alle esigenze
* Assegna modelli di layout ai livelli di accesso

Qualsiasi utente che ha accesso alla condivisione di oggetti può condividerli con il profilo aziendale e tutti gli utenti con il profilo visualizzeranno l’oggetto.

## Esempio di profilo aziendale

>[!BEGINSHADEBOX]

Sam ha bisogno di un accesso diverso ai progetti per l&#39;Agenzia A e l&#39;Agenzia B. Entrambe le agenzie sono configurate come gruppi in Workfront. (Per informazioni sui gruppi, consulta Panoramica sui gruppi).

Per l&#39;Agenzia A, Sam svolge il ruolo di controllore finanziario e ha bisogno dell&#39;accesso per visualizzare tutti i campi finanziari dei suoi progetti. Per l&#39;Agenzia B, Sam svolge il ruolo di project manager e deve gestire le attività e i problemi, ma non deve essere in grado di visualizzare le informazioni finanziarie.

L&#39;amministratore di sistema Workfront crea nuovi livelli di accesso denominati Financial Controller e Project Manager. A questi livelli di accesso viene concesso l&#39;accesso corretto per i dati finanziari. L&#39;amministratore apre quindi il profilo utente di Sam e seleziona &quot;Agenzia A&quot; come gruppo con il livello di accesso &quot;Controller finanziario&quot; per creare il primo profilo business, e &quot;Agenzia B&quot; come gruppo con il livello di accesso &quot;Project Manager&quot; per creare il secondo profilo business.

Una volta impostati i profili aziendali, quando Sam accede all’elenco dei progetti, vengono visualizzati tutti i progetti per l’Agenzia A e l’Agenzia B (insieme a tutti gli altri progetti che Sam ha creato o a cui è stato concesso l’autorizzazione). I campi finanziari dei progetti dell&#39;Agenzia A sono visibili a Sam sia nella vista a elenco che nei dettagli del progetto, ma i campi finanziari dei progetti dell&#39;Agenzia B sono nascosti. Vengono visualizzati i nomi dei campi, ma i dati dei campi sono vuoti.

Se altri utenti di una delle due agenzie condividono dei progetti con i profili aziendali &quot;Financial Controller - Agency A&quot; o &quot;Project Manager - Agency B&quot;, tali progetti sono visibili a Sam. I campi finanziari dei progetti dell&#39;Agenzia B rimarranno sempre nascosti perché sono definiti nel livello di accesso.

>[!ENDSHADEBOX]

## Come vengono definiti i profili aziendali

L’amministratore di sistema di Adobe Workfront è responsabile della definizione di tutte le aree di un profilo di business.

### Crea livello di accesso

L&#39;amministratore di sistema di Workfront crea il livello di accesso con l&#39;accesso necessario e definisce i campi con restrizioni in base alle esigenze.

Per ulteriori informazioni, vedere [Creare e modificare livelli di accesso personalizzati](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Aggiungi profilo business all&#39;utente

L’amministratore di sistema di Workfront aggiunge il profilo business a un profilo utente selezionando un gruppo e un livello di accesso. La combinazione dei due crea il profilo aziendale. Ogni gruppo può essere utilizzato in un solo profilo aziendale per utente. <!--how does this combine with more than one access level per group. As far as I can see a business profile is one level and one group-->

Il profilo business può avere più di un livello di accesso per gruppo. Il livello con l&#39;accesso più alto ha la precedenza.

L’amministratore può assegnare date di validità a un profilo aziendale, in modo che l’accesso dell’utente scada in una data futura. Le date di inizio e di fine indicano quando l’utente inizia e termina a tenere il profilo in quel gruppo. L’utilizzo di date di validità per terminare l’accesso invece di eliminare il profilo consente di riattivarlo in futuro.

Più profili aziendali sono consentiti per un utente.

<!--image?-->

Per ulteriori informazioni, vedere [Modificare il profilo di un utente](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). <!--may be separate article now since it's not in the profile-->

### Assegna modelli di layout al livello di accesso

L’amministratore di sistema Workfront può facoltativamente assegnare un modello di layout al livello di accesso, per garantire che gli utenti con il profilo di business correlato visualizzino informazioni e azioni pertinenti in base al loro ruolo all’interno del sistema.

Per ulteriori informazioni, vedere [Assegnare gli utenti a un modello di layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

## Funzionamento dei profili aziendali

Quando un profilo di business viene aggiunto a un utente, le autorizzazioni nella combinazione del gruppo e del livello di accesso determinano ciò che l’utente vedrà in Workfront.

### Layout Workfront

Quando il gruppo nel profilo business è associato a un progetto, viene applicato il modello di layout per il livello di accesso nel profilo business. Tutti gli utenti con il profilo business visualizzeranno le voci di menu, la home page e gli altri elementi di layout inclusi nel modello. Il modello di layout del profilo di business ha la precedenza su un modello di layout assegnato all’utente.

Se il profilo di business dispone di più livelli di accesso con lo stesso gruppo, i modelli di layout per entrambi i livelli di accesso vengono combinati. Vengono visualizzati tutti gli elementi di layout disponibili. Se una voce di menu è visualizzata in un modello ma è nascosta in un altro, verrà visualizzata. Solo gli elementi nascosti in tutti i modelli per il profilo business sono nascosti.

Nelle situazioni in cui gli stessi elementi vengono visualizzati in più modelli di layout ma l’ordine degli elementi è diverso (ad esempio la navigazione a sinistra o i pin), viene utilizzato l’ordine del modello del livello di accesso elencato per primo nel profilo aziendale.

### Progetti e altri oggetti condivisi

Quando un progetto è associato a un gruppo, un utente con un profilo di business per tale gruppo può visualizzarlo. La visibilità dei campi nel progetto si basa sul livello di accesso nel profilo aziendale. Se al gruppo vengono assegnati più livelli di accesso nel profilo aziendale dell’utente, si applica il livello con autorizzazioni più elevate.

Ad esempio, un utente ha due profili aziendali: il primo fornisce l’accesso al controllore finanziario per un gruppo (per visualizzare i campi per contabilità) e il secondo fornisce l’accesso al project manager in un gruppo diverso (dove i campi per contabilità non devono essere visualizzati).

L’utente vedrà i progetti per entrambi i gruppi nell’elenco di tutti i progetti. Sia nella vista a elenco che nei dettagli del progetto, l’utente visualizzava i dati finanziari solo per il primo gruppo. I campi di finanziamento sui progetti del secondo gruppo sarebbero vuoti.

Qualsiasi utente con accesso alla condivisione di oggetti può condividere tali oggetti con un profilo aziendale. Tutti gli utenti assegnati al profilo avranno le autorizzazioni specificate per l’oggetto. Tuttavia, se l’accesso è limitato nel livello di accesso assegnato dall’amministratore nel profilo aziendale, il livello di accesso ha la precedenza sulle autorizzazioni assegnate nella condivisione. Ad esempio, se il livello di accesso non consente la creazione di attività, l’utente non può aggiungere attività a un progetto, anche se dispone delle autorizzazioni di gestione per un progetto condiviso con il profilo aziendale.

Se a un utente viene assegnato un profilo business dopo che un oggetto è già stato condiviso con il profilo, l’utente vedrà l’oggetto con l’accesso specificato.

Quando un profilo di business ha più livelli di accesso, quello con la maggiore quantità di accesso ha la precedenza.

Per informazioni sulla condivisione, vedere [Condividere un oggetto](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Per informazioni sulla collaborazione tra i livelli di accesso e le autorizzazioni, vedere [Panoramica sui livelli di accesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

## Considerazioni sui profili aziendali

* Non è necessario che un utente sia membro di un gruppo per ottenere un profilo di business per tale gruppo.
* Il livello di accesso nel profilo aziendale può solo aggiornare il livello di accesso &quot;base&quot; di un utente. Il profilo business non può rimuovere le autorizzazioni del livello di accesso di base.
* Negli elenchi di oggetti e nei report, l’utente dispone di tutte le autorizzazioni disponibili in tutti i profili aziendali assegnati ai vari gruppi, uniti al relativo livello di accesso di base. Nelle altre pagine, l’utente dispone delle autorizzazioni del livello di accesso di base.
* Quando un gruppo viene eliminato da Workfront, tutti i profili di business assegnati a quel gruppo vengono rimossi dagli utenti associati.
* Se un livello di accesso fa parte di un profilo aziendale e si elimina il livello di accesso, viene richiesto di scegliere un nuovo livello di accesso da utilizzare.
* Gli aggiornamenti ai profili aziendali vengono tracciati nei registri di audit di Workfront. Per ulteriori informazioni, consulta Panoramica dei registri di audit.
