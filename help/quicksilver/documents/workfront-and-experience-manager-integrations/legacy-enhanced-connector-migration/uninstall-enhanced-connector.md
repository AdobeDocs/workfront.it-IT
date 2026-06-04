---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Disinstallare il connettore avanzato di Workfront for Adobe Experience Manager
description: È necessario disinstallare il connettore avanzato Workfront con Adobe Experience Manager all’integrazione nativa più recente che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
TQID: https://experienceleague.adobe.com/CeCyF8zbwp4tVcxQebq0EdaJqagDyppVuCL6ilqEvJA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 260
ht-degree: 3%

---

# Disinstallare Workfront con il connettore avanzato di Adobe Experience Manager

È necessario disinstallare il connettore avanzato Workfront con Adobe Experience Manager all’integrazione nativa più recente che collega Workfront e Adobe Experience Manager Assets as a Cloud Service.

## Prerequisiti

* (Facoltativo) Se necessario, ripristina le modifiche apportate alla configurazione del firewall Workfront e alle impostazioni del dispatcher AEM.

## Disinstallare il connettore avanzato

1. Accedi e clona l’archivio AEM as a Cloud Service da Cloud Manager.

1. Apri l’archivio Git clonato nell’IDE che preferisci.

1. Estrarre il ramo in cui è installato il connettore avanzato.

1. Passa al seguente percorso e rimuovi il file zip del connettore avanzato:

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. Rimuovi la seguente dipendenza dal file pom.xml della directory principale del progetto.

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >Assicurati che la versione a cui si fa riferimento nel blocco di codice precedente, ovvero 1.8.0, rifletta la versione che viene disinstallata dal codice.

1. Rimuovi la seguente dipendenza dal file pom.xml del sottomodulo del progetto denominato **all**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. Rimuovi i seguenti elementi incorporati dal file pom.xml del sottomodulo del progetto denominato all.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (Condizionale) Rimuovi la configurazione dell’archivio dal file pom.xml della directory principale del progetto.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (Condizionale) Rimuovi la configurazione del server da settings.xml, presente nel seguente percorso ./cloudmanager/maven/settings.xml nella directory principale del progetto.&#39;

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. Eseguire il commit delle modifiche e inviare il codice all&#39;archivio Cloud Manager

1. Esegui la pipeline Cloud Manager per distribuire le modifiche nell’istanza di Cloud Services
