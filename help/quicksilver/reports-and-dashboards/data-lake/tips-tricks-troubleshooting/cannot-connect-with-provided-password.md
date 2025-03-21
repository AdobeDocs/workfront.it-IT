---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Impossibile connettersi con la password fornita dallo strumento Power BI
description: Quando tenti di accedere a Data Connect dallo strumento Power BI, ricevi un errore di accesso.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 40050915153af6e1f70024461e193fb536d74e35
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---


# Lo strumento Power BI non può connettersi con la password fornita

## Problema

Quando tenti di accedere a Data Connect dallo strumento Power BI, viene visualizzato il seguente errore:

`Cannot connect from BI tool with provided password`

## Causa

Durante la creazione della connessione JDBC, Workfront fornisce una password temporanea per Data Connect.

Prima di accedere a Data Connect tramite Power BI, è necessario accedere utilizzando i dettagli di connessione forniti, aggiornare la password temporanea e quindi procedere con l&#39;accesso.


## Soluzione

Reimposta la password di connessione in Workfront, quindi crea una nuova password con il collegamento fornito nella finestra di dialogo Modifica connessione.

### Reimpostare la password di connessione in Workfront

1. Vai a Workfront > Configurazione > Sistema > Connessione dati.
1. Individuare e aprire la connessione dall&#39;elenco.
1. In **Reimposta password connessione**, selezionare la casella per confermare che si desidera reimpostare la password.
1. Fare clic su **Reimposta password connessione**.
   ![reimpostare la password di connessione](assets/reset-password.png)
1. Procedi alla sezione seguente.

### Crea una nuova password per la connessione

1. Copia l’URL e incollalo in una nuova scheda del browser.
1. In Workfront, copia e incolla il nome utente della connessione e la password predefinita nella nuova scheda del browser.
   ![copia url e password predefinita](assets/link-password.png)
1. Fai clic su **Accedi**.
1. Immettere una nuova password, quindi fare clic su **Invia**.
1. Vai allo strumento Power BI e accedi con la nuova password.

