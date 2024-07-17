---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Carica documenti e bozze da  [!DNL Adobe Workfront plugin]  a  [!DNL Creative Cloud]
description: Carica documenti e bozze da  [!DNL Adobe Workfront plugin]  a  [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
source-git-commit: 0ca335bf0db934d23f607d3f8ce7cfb67e629053
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Carica documenti e bozze da [!DNL Adobe Workfront plugin] a [!DNL Creative Cloud]

Puoi caricare i tuoi progetti come documenti per una rapida revisione e approvazione o semplicemente per archiviarli in [!DNL Adobe Workfront].

>[!NOTE]
>
>Il caricamento di documenti e bozze non è attualmente supportato in Premiere Pro e After Effects.


## Limitazioni del documento

Questa sezione descrive le limitazioni note del documento in [!DNL Workfront for Adobe Creative Cloud plugins].

### Le nuove versioni dei documenti accettano un solo file per il caricamento

Poiché i documenti [!DNL Workfront] non possono contenere più file, è necessario disabilitare alcune impostazioni per caricare nuove versioni dei documenti in Workfront.

>[!NOTE]
>
>Se devi generare più file, puoi invece creare una bozza. La nuova bozza non verrà associata al documento originale.



Per tornare a un singolo file in [!DNL InDesign]:

1. Aprire la finestra di dialogo **Imposta impostazioni file di esportazione**.

   ![](assets/file-export-settings.png)

1. Trova il Tipo di risorsa da esportare e regola le impostazioni come descritto di seguito:

   <table>
    <tr>
    <td><strong>PDF e PDF-PRINT</strong>
    </td>
    <td>Deselezionare <strong>Crea File PDF Separati</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Seleziona <strong>Intervalli</strong> e digita un numero di pagina. 
    <p>
    <strong>Nota</strong>: se desideri caricare il documento completo, devi creare una bozza. 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB e EPUB fisso</strong>
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
    <td><strong>JPG-</strong>
    </td>
    <td>Seleziona <strong>Intervalli</strong> e digita un numero di pagina. 
    <p>
    <strong>Nota</strong>: se desideri caricare il documento completo, devi creare una bozza. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Seleziona <strong>Intervalli</strong> e digita un numero di pagina. 
    <p>
    <strong>Nota</strong>: se desideri caricare il documento completo, devi creare una bozza. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Non sono necessari adeguamenti. 
    </td>
    </tr>
    </table>
