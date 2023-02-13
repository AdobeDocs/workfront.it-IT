---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configura [!DNL Workfront Proof] e-mail per evitare filtri anti-spam
description: "Il filtro antispam del tuo client di posta elettronica svolge un ruolo importante: proteggervi dalle e-mail di spam fastidiose e possibilmente dannose. Ma, se non hai le impostazioni corrette nel filtro dello spam, ti può impedire di vedere la seguente importante [!DNL Workfront Proof] e-mail: notifiche e-mail a prova di e-mail, newsletter e comunicazioni speciali."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Configura [!DNL Workfront Proof] e-mail per evitare filtri anti-spam

>[!IMPORTANT]
>
>Questo articolo fa riferimento alla funzionalità del prodotto standalone [!DNL Workfront Proof]. Per informazioni sulle prove all&#39;interno [!DNL Adobe Workfront], vedi [Copertura](../../../review-and-approve-work/proofing/proofing.md).

Il filtro posta indesiderata del tuo client e-mail svolge uno scopo importante: proteggervi dalle e-mail di spam fastidiose e possibilmente dannose. Ma, se non hai le impostazioni corrette nel filtro dello spam, ti può impedire di vedere la seguente importante [!DNL Workfront Proof] e-mail: notifiche e-mail, newsletter e comunicazioni speciali a prova.

Per assicurarti che il tuo [!DNL Workfront Proof] Le e-mail vengono sempre indirizzate alla tua casella in entrata invece che alla cartella spam. Aggiungi quanto segue all’inserire nell&#39;elenco Consentiti:

* [!DNL Workfront Proof] server di posta elettronica: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi e-mail (ad esempio, notification@proofhq.com)

Per ulteriori informazioni sugli URL da aggiungere al tuo inserire nell&#39;elenco Consentiti, vedi [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) nell&#39;articolo [Configurare l’inserire nell&#39;elenco Consentiti del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi e-mail

A seconda del tipo di client e-mail, potrebbe essere necessario aggiungere [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi e-mail a uno dei seguenti per impedire che il filtro posta indesiderata instradi le tue e-mail nella cartella posta indesiderata in futuro:

* Elenco contatti
* Le [!UICONTROL Mittenti sicuri] elenco
* Un filtro creato per inviare e-mail da tali indirizzi alla casella in entrata

Potrebbe inoltre essere necessario rimuovere eventuali [!DNL Workfront Proof] e-mail dalla cartella spam e controlla se uno dei &quot;[!UICONTROL da]&quot; gli indirizzi si trovano nell&#39;elenco degli indirizzi bloccati. Questa pagina della guida elenca i [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi e mostra come aggiungerli al filtro posta indesiderata nei seguenti client e-mail:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Se hai domande su una procedura descritta qui, controlla l&#39;aiuto del tuo client di posta elettronica.

Per ulteriori informazioni, consulta [Configurare le impostazioni di posta indesiderata per i client e-mail comuni](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## La [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi e-mail da copiare

Per assicurarti che il tuo [!DNL Workfront Proof] le e-mail raggiungono la tua casella in entrata, dovrai aggiungere due [!DNL Workfront Proof] indirizzi e-mail separatamente dal filtro posta indesiderata del cliente e-mail:

* l&#39;indirizzo generale di sostegno, [!DNL support@proofhq.com]da cui [!DNL Workfront Proof] invia molte comunicazioni e-mail
* Indirizzo di notifica da cui [!DNL Workfront Proof] invia e-mail di notifica della bozza al creatore della bozza e ai revisori con collegamenti alla bozza. Può trattarsi di un indirizzo generale, notification@support.proofhq.com o di un indirizzo specifico se si dispone di un sottodominio personalizzato o di un dominio di etichetta bianca.

Per aggiungere [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi al filtro del client di posta elettronica:

1. Copia il generale [!DNL Workfront Proof] supporto &quot;[!UICONTROL da]&quot; indirizzo e-mail (support@proofhq.com) e incollalo nel campo indicato per il client e-mail.
1. Copia il file appropriato tra i seguenti [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi e-mail e incollali SEPARATAMENTE nel campo indicato per il client e-mail:

   * notification@support.proofhq.com se NON disponi di un sottodominio personalizzato o di un dominio con etichetta bianca
   * notification@yoursubdomain.proofhq.com se disponi di un sottodominio personalizzato; sostituisci il nome del sottodominio in questo indirizzo
   * notification@yoursubdomain.yourdomain.com se si dispone di un dominio di etichetta bianca; sostituisci il nome del sottodominio e il nome di dominio in questo indirizzo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
