---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Invia modifiche tasso ai progetti
description: Una scheda tariffa rappresenta l’accordo contrattuale con il cliente in cui vengono definite le tariffe orarie per le mansioni che completeranno il lavoro. In una scheda tariffa è possibile definire più tariffe di fatturazione per mansione, in base agli attributi.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 38441ec5ae6fd8cf5c79f939403d5966c5616c98
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 10%

---

# Modifiche della velocità push nei progetti

{{highlighted-preview-article-level}}

Quando una scheda tariffe è allegata a un progetto <!--or a staffing plan-->, è comunque possibile regolare le tariffe sulla scheda tariffe. Quindi, puoi facoltativamente inviare tali tariffe ai progetti <!--and staffing plans --> a cui è allegata la scheda delle tariffe. Se non esegui il push delle nuove tariffe, le tariffe originali rimangono sul progetto<!-- or staffing plan-->.

Per informazioni su come allegare una scheda tariffe a un progetto, vedere [Allegare una scheda tariffe a un progetto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità descritta in questo articolo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacchetto</td> 
   <td>Flusso di lavoro Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licenza</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Configurazioni del livello di accesso</td> 
   <td>Modifica accesso a [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Autorizzazioni sugli oggetti</td> 
   <td>Per modificare una scheda delle tariffe condivisa con te, devi disporre delle autorizzazioni di gestione per tale scheda.</td> 
  </tr> 
 </tbody> 
</table>

Per informazioni, consulta [Requisiti di accesso nella documentazione di Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifiche della velocità push nei progetti

{{step-1-to-setup}}

1. Nel pannello a sinistra, fai clic su [!UICONTROL **Classifica schede**].
1. Fare clic sul nome della scheda tariffe nell&#39;elenco Schede tariffe.
1. Nella schermata Rate Card > Job Roles and Rates (Scheda tariffa > Ruoli e tariffe), verifica che le tariffe siano corrette e modifica eventuali tariffe in base alle esigenze.
1. Fai clic su [!UICONTROL **Push changes**].
1. Nella finestra di dialogo [!UICONTROL **Applica a tutti i progetti**]<!--/staffing plans-->, tutti i progetti <!--and staffing plans --> che utilizzano questa scheda tariffe sono selezionati per impostazione predefinita. Se non si desidera che un progetto <!--or staffing plan --> applichi le modifiche della tariffa, è necessario deselezionarlo.
1. Fai clic su [!UICONTROL **Salva**].

   I nuovi tassi ora si riflettono sui progetti <!--and staffing plans --> che utilizzano la scheda dei tassi.