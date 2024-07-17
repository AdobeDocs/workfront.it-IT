---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Configura  [!DNL Workfront Proof]  e-mail per evitare filtri anti-spam
description: "Il filtro spam del client di posta elettronica ha uno scopo importante: proteggerti da e-mail spam fastidiose e potenzialmente dannose. Tuttavia, se non disponi delle impostazioni corrette nel filtro anti-spam, puoi evitare di visualizzare le seguenti [!DNL Workfront Proof] e-mail importanti: notifiche e-mail relative alla bozza, newsletter e comunicazioni speciali."
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
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Il filtro anti-spam del client di posta elettronica ha uno scopo importante: proteggerti da e-mail spam fastidiose e potenzialmente dannose. Tuttavia, se non disponi delle impostazioni corrette nel filtro anti-spam, puoi evitare di visualizzare le [!DNL Workfront Proof] e-mail importanti seguenti: notifiche e-mail relative alle bozze, newsletter e comunicazioni speciali.

Per assicurarsi che le e-mail di [!DNL Workfront Proof] siano sempre instradate alla cartella Posta in arrivo anziché alla cartella di posta indesiderata, è necessario aggiungere quanto segue al inserisco nell&#39;elenco Consentiti di:

* Server di posta [!DNL Workfront Proof]: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi e-mail (ad esempio, notification@proofhq.com)

Per ulteriori informazioni sugli URL da aggiungere al inserisco nell&#39;elenco Consentiti di URL, vedere [Configurare il inserisco nell&#39;elenco Consentiti di del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) nell&#39;articolo [Configurare il inserisco nell&#39;elenco Consentiti di del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi e-mail

A seconda del tipo di client di posta elettronica, potrebbe essere necessario aggiungere gli indirizzi di posta elettronica [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; a uno dei seguenti per evitare che il filtro anti-spam instradi le e-mail nella cartella di posta indesiderata in futuro:

* Elenco contatti
* Il tuo elenco [!UICONTROL Mittenti attendibili]
* Un filtro creato per inviare e-mail da tali indirizzi alla tua casella in entrata

Potrebbe inoltre essere necessario rimuovere [!DNL Workfront Proof] e-mail esistenti dalla cartella di posta indesiderata e verificare se gli indirizzi &quot;[!UICONTROL from]&quot; sono inclusi nell&#39;elenco indirizzi bloccati. In questa pagina della Guida sono elencati gli indirizzi [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; e viene illustrato come aggiungerli al filtro anti-spam nei seguenti client di posta elettronica:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>In caso di domande su una procedura qui descritta, consulta l’Aiuto del cliente e-mail.

Per ulteriori informazioni, vedere [Configurare le impostazioni di posta indesiderata per i client di posta elettronica comuni](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## Gli indirizzi e-mail [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; da copiare

Per assicurarsi che le e-mail di [!DNL Workfront Proof] raggiungano la tua casella in entrata, dovrai aggiungere separatamente due indirizzi e-mail di [!DNL Workfront Proof] al filtro di posta indesiderata del client di posta elettronica:

* L&#39;indirizzo del supporto generale, [!DNL support@proofhq.com], da cui [!DNL Workfront Proof] invia molte comunicazioni e-mail
* Un indirizzo di notifica da cui [!DNL Workfront Proof] invia le e-mail di notifica della bozza al creatore della bozza e ai revisori con i collegamenti alla bozza. Potrebbe trattarsi di un indirizzo generale, notification@support.proofhq.com, o di un indirizzo specifico se disponi di un sottodominio personalizzato o di un dominio con etichetta bianca.

Per aggiungere gli indirizzi [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; al filtro del client di posta elettronica:

1. Copiare l&#39;indirizzo di posta elettronica del supporto [!DNL Workfront Proof] generale &quot;[!UICONTROL from]&quot; (support@proofhq.com) e incollarlo nel campo indicato per il client di posta elettronica.
1. Copia uno dei seguenti [!DNL Workfront Proof] &quot;[!UICONTROL da]&quot; indirizzi di posta elettronica e incollali SEPARATAMENTE nel campo indicato per il client di posta elettronica:

   * notification@support.proofhq.com se NON disponi di un sottodominio personalizzato o di un dominio con etichetta bianca
   * notification@yoursubdomain.proofhq.com se disponi di un sottodominio personalizzato; sostituisci il nome del sottodominio in questo indirizzo
   * notification@yoursubdomain.yourdomain.com se disponi di un dominio con etichetta bianca; sostituisci il nome del sottodominio e del dominio in questo indirizzo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
