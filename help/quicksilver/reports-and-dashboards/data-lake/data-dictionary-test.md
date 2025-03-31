---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Creazione di un account di lettura per Snowflake
description: Per accedere ai dati di Data Connect, è necessario innanzitutto creare un account lettore Snowflake.
author: Courtney
feature: Reports and Dashboards
hide: true
hidefromtoc: true
source-git-commit: a42c13804b0463af27bac6f9166bc6e3c41d3fda
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 8%

---


# Test

## Livelli di accesso

<table>
  <thead>
    <tr>
        <th>Nome entità Workfront</th>
        <th>Riferimenti interfaccia</th>
        <th>Riferimento API | Etichetta</th>
        <th>Visualizzazioni Data Lake</th>
    </tr>
  </thead>
 <tr>
        <td>Livello di accesso</td>
         <td>Livello di accesso</td>
        <td>ACSLVL | Livello d'Accesso</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong>Campo relazioni</strong> <br>
         ACCESSLEVELID (self): Self<br>
         APPGLOBALID: non una relazione; utilizzato per scopi interni dell'applicazione<br>
         LASTUPDATEDBYID: USER_CURRENT | ID UTENTE<br>
         LEGACYACCESSLEVELID: non una relazione; utilizzato per scopi interni dell'applicazione<br>
         OBJID: ID dell'oggetto identificato nel campo OBJCODE <br>
         SYSID: non una relazione. Utilizzato per applicazioni interne.</td>
    </tr>
</table>

## Livelli di accesso

<table>
  <thead>
    <tr>
        <th>Nome entità Workfront</th>
        <th>Riferimenti interfaccia</th>
        <th>Riferimento API | Etichetta</th>
        <th>Visualizzazioni Data Lake</th>
    </tr>
  </thead>
 <tr>
        <td>Livello di accesso</td>
         <td>Livello di accesso</td>
        <td>ACSLVL | Livello d'Accesso</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
    </tr>
     <tr>
     <tr>
         <td colspan="4"><strong>Campo relazioni</strong> <br>
         <ul>
            <li>ACCESSLEVELID (self): Self</li>
            <li>APPGLOBALID: non una relazione; utilizzato per scopi di applicazione interni</li>
            <li>LASTUPDATEDBYID: USER_CURRENT | USERID</li>
            <li>LEGACYACCESSLEVELID: non una relazione; utilizzato per scopi interni all'applicazione</li>
            <li>OBJID: ID dell'oggetto identificato nel campo OBJCODE.</li>
            <li>SYSID: non una relazione. Utilizzato per applicazioni interne.</li>
        </ul>
    </tr>
</table>