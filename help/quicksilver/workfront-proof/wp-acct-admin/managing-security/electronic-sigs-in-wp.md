---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Informazioni sulle firme elettroniche in [!DNL Workfront Proof]
description: Le firme elettroniche consentono di migliorare la sicurezza delle bozze e di rispettare gli standard di settore come ISO.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Informazioni sulle firme elettroniche in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Questo articolo fa riferimento alle funzionalità nel prodotto autonomo [!DNL Workfront Proof]. Per informazioni sulla verifica all&#39;interno di [!DNL Adobe Workfront], vedere [Verifica](../../../review-and-approve-work/proofing/proofing.md).

Le firme elettroniche consentono di migliorare la sicurezza delle bozze e di rispettare gli standard di settore come ISO.

Questa impostazione può essere resa obbligatoria o non obbligatoria a livello di account. Se è obbligatorio per impostazione predefinita, viene abilitato su tutte le bozze create nel tuo account e non può essere disabilitato a livello di bozza. Se questa impostazione non è obbligatoria per impostazione predefinita, potrai abilitarla o disabilitarla a livello di bozza.

Per ulteriori informazioni, consulta .

Quando l&#39;impostazione della firma elettronica è abilitata su una bozza, un riquadro di firma elettronica richiede a qualsiasi revisore che decide sulla bozza di fornire la propria e-mail e password.

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## Firme elettroniche nella pagina [!UICONTROL Dettagli bozza]

Se un revisore decide selezionando la propria decisione nella pagina [!UICONTROL Dettagli bozza] (1), verrà visualizzata una finestra a comparsa [!UICONTROL Firma elettronica] in cui viene richiesto di immettere i propri dettagli (2) e di confermare la propria decisione (3).

Nel pop-up verrà visualizzato il set di messaggi predefinito (se presente) e al revisore verrà richiesto di inserire l’e-mail e la password.

Se il revisore decide di prendere una decisione a partire da tale livello, la finestra a comparsa [!UICONTROL Firma elettronica] verrà visualizzata nel visualizzatore di bozze e nella pagina [!UICONTROL Dettagli bozza].

![Firma_Elettronica_-_Dettagli_Bozza.png](assets/electronic-signature---proof-details-350x146.png)

![Firma_Elettronica_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

Se l&#39;opzione [!UICONTROL Single Sign-On] è abilitata nella bozza, i dettagli dell&#39;e-mail e della password non verranno visualizzati nel pop-up [!UICONTROL Firma elettronica] quando si prende una decisione.

Al contrario, dopo aver fatto clic sul pulsante [!UICONTROL Conferma] (4) in questa finestra a comparsa, il revisore verrà reindirizzato alla pagina [!UICONTROL Single Sign-On].

Dopo aver immesso le credenziali SSO, il revisore verrà automaticamente reindirizzato alla pagina [!UICONTROL Dettagli bozza] (o nuovamente al [!UICONTROL Visualizzatore bozze] se la decisione viene presa da lì).

![Firma_Elettronica_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> Se la decisione è firmata elettronicamente, l&#39;icona **[!UICONTROL firma]** (5) viene visualizzata accanto alla decisione nella sezione [!UICONTROL Flusso di lavoro] nella pagina [!UICONTROL Dettagli bozza]. Se la decisione non viene modificata dal revisore, ma da un’altra persona che dispone dei diritti di modifica sulla bozza, a tale persona non verrà richiesto di firmare elettronicamente la decisione e non ci sarà alcuna icona di firma accanto alla decisione (6).

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)Per informazioni sul Single Sign-On, vedere [Single Sign-On in Workfront Proof](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

Per informazioni sulla pagina Dettagli bozza, vedere [Gestione dei dettagli bozza in [!DNL Workfront] Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
