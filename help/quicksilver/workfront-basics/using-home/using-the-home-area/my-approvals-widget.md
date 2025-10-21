---
product-area: home
navigation-topic: use-the-home-area
title: Gestire le approvazioni con il widget Le mie approvazioni
description: Il widget Approvazioni personali visualizza tutte le approvazioni in sospeso, assegnate, delegate e inviate in un'unica posizione. Qui puoi filtrare e organizzare le approvazioni, prendere decisioni e delegare le approvazioni in base alle esigenze.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 4981d9adb2cae53e30f13aa2a7aa6857befbf3ca
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 5%

---

# Gestire le approvazioni con il widget Le mie approvazioni

Il widget Approvazioni personali visualizza tutte le approvazioni in sospeso, assegnate, delegate e inviate in un&#39;unica posizione. Qui puoi filtrare e organizzare le approvazioni, prendere decisioni e delegare le approvazioni in base alle esigenze.

Il widget Approvazioni personali supporta le approvazioni dai seguenti oggetti Workfront:

* Attività
* Problemi
* Progetti
* Documenti
* Bozze
* Pianificazione delle richieste di record
* Schede orario

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacchetto Adobe Workfront</td> 
   <td> <p>Qualsiasi</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td> 
   <p>Collaboratore o versione successiva</p>
   <p>Revisione o successiva</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Accesso di visualizzazione o accesso successivo agli oggetti associati alle approvazioni</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorizzazioni oggetto</td> 
   <td> <p>Visualizza o autorizzazioni superiori per gli oggetti associati alle approvazioni</p></td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Approva il lavoro dal widget Le mie approvazioni

1. Fai clic sull&#39;icona **[!UICONTROL Main Menu]** ![Main Menu](assets/main-menu-icon.png) nell&#39;angolo superiore destro, quindi fai clic su **[!UICONTROL Home]**.
1. (Condizionale) Fai clic su **Personalizza** per aggiungere il widget **Le mie approvazioni**.
1. (Condizionale) Fai clic sul menu a discesa **Filtro**, quindi seleziona **Tutti** per visualizzare le approvazioni assegnate e delegate all&#39;utente.

   >[!NOTE]
   >
   >Le approvazioni assegnate a Ruoli o Gruppi non vengono visualizzate nella Home. Le approvazioni assegnate ai team vengono visualizzate nel widget Approvazioni personali per ogni membro del team.


1. Seleziona l’elemento in cui desideri prendere una decisione di approvazione.

   ![Widget approvazioni personali](assets/my-approvals-widget.png)

1. Fai clic su una delle opzioni disponibili quando prendi una decisione di approvazione nel pannello a destra. Le seguenti opzioni vengono visualizzate nell&#39;angolo superiore destro della pagina, a seconda del tipo di elemento che si sta approvando:

   <table>
   <tr>
      <td>
      <p><strong>Accesso</strong></p>
      </td>
      <td>
      <p><strong>Elementi di lavoro</strong></p>
      </td>
      <td>
      <p><strong>Documenti</strong></p>
      </td>
      <td>
      <p><strong>Bozze</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>Concedi</li>
      <li>Ignora</li>
      </ul>
      Se necessario, è possibile regolare il livello di accesso nel menu a discesa <b>Modifica accesso</b>.
      </td>
      <td>
         <ul>
         <li>Approvazione</li>
         <li>Rifiuta</li>
         </ul>
      Per lasciare un commento associato alla decisione, fai clic sul menu a discesa nel pulsante di decisione.
      </td>
      <td>
   Assegnato come approvatore
         <ul>
         <li>Approvazione</li>
         <li>Approva con modifiche</li>
         <li>Azioni da intraprendere</li>
         </ul>
   Assegnato come revisore
         <ul>
         <li>Completa la revisione</li>
         </ul>
      Le opzioni in questa colonna si applicano solo alle approvazioni unificate. Le approvazioni di documenti legacy vengono visualizzate come le approvazioni di elementi di lavoro. 
      </td>
      <td>
         <ul>
         <li>Vai alla bozza</li>
         </ul>
         La decisione viene presa nel visualizzatore bozze. Per informazioni sulla revisione di una bozza, vedi <a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Verifica delle bozze in Adobe Workfront</a>.
      </td>
   </tr>
   </table>

Dopo aver preso una decisione, l&#39;approvazione viene rimossa dal widget Approvazione personale.