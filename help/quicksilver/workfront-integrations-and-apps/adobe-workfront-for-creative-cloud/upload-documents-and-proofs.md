---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Carica documenti e bozze dal [!DNL Adobe Workfront plugin] al [!DNL Creative Cloud]
description: Carica documenti e bozze dal [!DNL Adobe Workfront plugin] al [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
source-git-commit: 67952bf88a782595e13e559bfbc14ce1c622d432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Carica documenti e bozze dal [!DNL Adobe Workfront plugin] al [!DNL Creative Cloud]

Puoi caricare i tuoi progetti come documenti per una rapida revisione e approvazione o semplicemente per archiviarli in [!DNL Adobe Workfront].

>[!NOTE]
>
>Il caricamento di documenti e bozze non è attualmente supportato in Premiere Pro e After Effects.


## Limiti dei documenti

In questa sezione sono illustrate le limitazioni note per i documenti [!DNL Workfront for Adobe Creative Cloud plugins].

### Le nuove versioni del documento accettano un solo file per il caricamento

Perché [!DNL Workfront] i documenti non possono contenere più file. Per caricare nuove versioni dei documenti in Workfront è necessario disattivare alcune impostazioni.

>[!NOTE]
>
>Se è necessario generare più file, è invece possibile creare una bozza. La nuova bozza non verrà associata al documento originale.



Per ripristinare il passaggio a un singolo file in [!DNL InDesign]:

1. Apri **Imposta le impostazioni del file di esportazione** finestra di dialogo.

   ![](assets/file-export-settings.png)

1. Trova il tipo di risorsa da esportare e regola le impostazioni come descritto di seguito:

   <table>
    <tr>
    <td><strong>PDF e PDF-PRINT</strong>
    </td>
    <td>Deseleziona <strong>Creare file PDF separati</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Seleziona <strong>Intervalli</strong> e digitare un numero di pagina singolo. 
    <p>
    <strong>Nota</strong>: Se desideri caricare il documento completo, devi creare una bozza. 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB e EPUB-FIXED</strong>
    </td>
    <td>Non sono necessari adeguamenti.
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>Non sono necessari adeguamenti.
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>Seleziona <strong>Intervalli</strong> e digitare un numero di pagina singolo. 
    <p>
    <strong>Nota</strong>: Se desideri caricare il documento completo, devi creare una bozza. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Seleziona <strong>Intervalli</strong> e digitare un numero di pagina singolo. 
    <p>
    <strong>Nota</strong>: Se desideri caricare il documento completo, devi creare una bozza. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Non sono necessari adeguamenti. 
    </td>
    </tr>
    </table>
