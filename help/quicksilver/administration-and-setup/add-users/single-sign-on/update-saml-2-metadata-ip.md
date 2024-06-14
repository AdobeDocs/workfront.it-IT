---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Aggiornamento dei metadati SAML 2.0 nel provider di identità
description: Puoi aggiornare i metadati SAML 2.0 nel provider di identità.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# Aggiornamento dei metadati SAML 2.0 nel provider di identità

{{important-admin-console-onboard}}

Nelle sezioni seguenti viene descritto come aggiornare i metadati SAML (Security Assertion Markup Language) 2.0 quando si utilizza Active Directory Federation Services (ADFS) come provider di identità.

## Requisiti di accesso

+++ Espandi per visualizzare i requisiti di accesso per la funzionalità in questo articolo.

Per eseguire i passaggi descritti in questo articolo, è necessario disporre dei seguenti diritti di accesso:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">piano Adobe Workfront</td> 
   <td>Qualsiasi</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenza Adobe Workfront</td> 
   <td>Piano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurazioni del livello di accesso</td> 
   <td> <p>Devi essere un amministratore di Workfront.</p> <p><b>NOTA</b>: se ancora non disponi dell’accesso, chiedi all’amministratore di Workfront se ha impostato restrizioni aggiuntive nel tuo livello di accesso. Per informazioni su come un amministratore di Workfront può modificare il tuo livello di accesso, consulta <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creare o modificare livelli di accesso personalizzati</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Utilizzare ADFS come provider di identità

È possibile aggiornare i metadati ADFS prima di Adobe Workfront, aggiornando il certificato SAML 2.0 o dopo. Se scegli di aggiornare i metadati ADFS prima di Workfront che aggiorni il certificato SAML 2.0, sono necessari passaggi aggiuntivi.

* [Aggiornare i metadati ADFS](#update-your-adfs-metadata)
* [Forza l&#39;aggiornamento dei metadati ADFS](#force-your-adfs-metadata-to-update)

### Aggiornare i metadati ADFS {#update-your-adfs-metadata}

Per impostare l&#39;aggiornamento automatico dei metadati ADFS, completare i passaggi descritti in questa sezione.

Per impostazione predefinita, ADFS è configurato per verificare automaticamente la disponibilità di aggiornamenti per tutti i metadati di attendibilità del componente. Tuttavia, l&#39;impostazione predefinita è impostata per il polling solo ogni 24 ore. È possibile modificare questo valore con i comandi di powershell.

1. Accedere al server ADFS e aprire ADFS Management Console.
1. Nel pannello a sinistra, espandi **ADFS 2.0** quindi espandi **Relazioni di affidabilità.**

1. Fai clic su **Trust relying party** cartella.
1. Seleziona l’attendibilità del componente configurata in precedenza per l’utilizzo con Workfront, quindi nel pannello di destra fai clic su **Aggiorna da metadati federativi**.
1. (Condizionale) Se questa opzione è disabilitata (il che significa che l&#39;attendibilità del componente è stata configurata in precedenza utilizzando un file di metadati), completare le operazioni seguenti.

   1. Fai clic su **Menu principale** icona ![](assets/main-menu-icon.png) nell’angolo superiore destro di Adobe Workfront, quindi fai clic su **Configurazione** ![](assets/gear-icon-settings.png).

   1. Clic **Sistema** > **Single Sign-On (SSO)**.

   1. Clic **Modifica impostazioni.**
   1. Clic **Modifica configurazione**, quindi seleziona **SAML 2.0** nel **Tipo** elenco a discesa.

   1. Copia il **URL metadati**, che dovrebbe essere simile a quanto segue:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Nel server ADFS fare clic con il pulsante destro del mouse sull&#39;attendibilità del componente configurata in precedenza, quindi scegliere **Proprietà.**
   1. Fai clic su **Monitorare** , quindi incolla l&#39;URL copiato da Workfront in **URL metadati federazione del componente** campo.

   1. Seleziona le opzioni per **Monitora componente** e **Aggiorna automaticamente componente**.

   1. Clic **OK.**
   1. Selezionare l&#39;attendibilità del componente precedentemente configurato per l&#39;utilizzo con Workfront, quindi nel pannello di destra fare clic su **Aggiornamento dai metadati federativi.**

1. Clic **OK** ignorare il messaggio relativo a parte del contenuto dei metadati federativi non supportati da ADFS 2.0.
1. Apri **Moduli Windows Powershell.**
1. Dopo il caricamento di tutti i moduli, eseguire il comando seguente in PowerShell:

   `Get-ADFSProperties`

1. Cerca il valore accanto a **Intervallo di monitoraggio.**

   Sarà un numero che rappresenta il numero di minuti tra un sondaggio e l&#39;altro. Il valore predefinito è 1440 (1440 minuti = 24 ore).

1. Impostare un nuovo valore eseguendo il comando seguente in powershell:

   `Set-ADFSProperties -MonitoringInterval 1`

   L&#39;intervallo di monitoraggio cambia da 24 ore a ogni minuto. Puoi modificare il valore 1 con un altro più grande se desideri che venga eseguito il polling meno frequentemente.

1. Per verificare che ciò funzioni correttamente, utilizza **Visualizzatore eventi** per cercare le informazioni seguenti nei registri ADFS2.0:

   **ID evento 156 e 157**

### Forza l&#39;aggiornamento dei metadati ADFS {#force-your-adfs-metadata-to-update}

Per aggiornare i metadati ADFS, completare i passaggi descritti nella sezione seguente.

Per forzare lo scambio di metadati tra Workfront e il provider SAML 2.0 quando si utilizza Active Directory Federation Services (ADFS):

>[!NOTE]
>
>Alcune di queste modifiche potrebbero dover essere effettuate dal reparto IT.

1. Accedere al server ADFS e aprire **Console di gestione ADFS**.
1. Nel pannello a sinistra, espandi **ADFS 2.0**, quindi espandi **Relazioni di attendibilità**.

1. Fai clic su **Trust relying party** cartella.
1. Seleziona l’attendibilità del componente configurata in precedenza per l’utilizzo con Workfront, quindi nel pannello di destra fai clic su **Aggiorna da metadati federativi**.

   Se questa opzione è disattivata e non può essere selezionata, completare le operazioni seguenti:

   L&#39;opzione è disattivata solo quando l&#39;attendibilità del componente è stata configurata in precedenza utilizzando un file di metadati.

   1. In Workfront, nell’area Setup (Configura), copia il file **URL metadati** dalla schermata di installazione di Workfront Single Sign-On.

      Per accedere alle informazioni per **URL metadati**:

      1. Clic **Configurazione** vicino all’angolo superiore destro di Adobe Workfront sulla barra di navigazione globale.
      1. Fai clic su > **Sistema** > **Single Sign-On (SSO)**.
      1. Clic **Modifica impostazioni.**
      1. Clic **Modifica configurazione**, quindi seleziona **SAML 2.0** nel **Tipo** elenco a discesa.
      1. Copia il **URL metadati**, che dovrebbe essere simile a quanto segue:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Nel server ADFS fare clic con il pulsante destro del mouse sull&#39;attendibilità del componente configurata in precedenza, quindi scegliere **Proprietà.**
   1. Fai clic su **Monitorare** , quindi incolla l&#39;URL copiato da Workfront in **URL metadati federazione del componente** campo.
   1. Seleziona le opzioni per **Monitora componente** e **Aggiorna automaticamente componente**.
   1. Clic **OK**.
   1. Seleziona l’attendibilità del componente configurata in precedenza per l’utilizzo con Workfront, quindi nel pannello di destra fai clic su **Aggiornamento dai metadati federativi.**

1. Clic **OK** ignorare il messaggio relativo a parte del contenuto dei metadati federativi non supportati da ADFS 2.0.
1. Clic **Aggiorna** per completare l&#39;aggiornamento dei metadati federativi.

Utenti autorizzati ad accedere a Workfront tramite la schermata di accesso nativa utilizzando le credenziali di accesso di Workfront (questa può essere configurata dalla pagina del profilo di ciascun utente in **Accesso** sezione ) possono effettuare l&#39;accesso con il proprio nome utente e password Workfront passando al seguente URL: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Utilizzo di altri provider di identità

Quando utilizzi provider di identità diversi da ADFS (ad esempio Ping, Okta o Centrify), devi ricaricare i metadati di Workfront nel provider di identità.

Per ulteriori informazioni su come ottenere un nuovo URL di metadati di Workfront, vedi [Aggiornare i metadati ADFS](#update-your-adfs-metadata).

Per ulteriori informazioni sull&#39;utilizzo di Active Directory Federation Services (ADFS) con SAML 2.0 in Workfront, vedere [Configurare Adobe Workfront con SAML 2.0 utilizzando ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
