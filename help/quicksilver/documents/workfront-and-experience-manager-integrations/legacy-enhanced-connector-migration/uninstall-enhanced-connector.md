---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Avinstallera den utökade Workfront for Adobe Experience Manager-anslutningen
description: Du måste avinstallera Workfront med Adobe Experience Manager förbättrade anslutning till den senaste inbyggda integreringen som kopplar Workfront och Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 9673009f12509b5e7051ee91e142d311f333f215
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Avinstallera Workfront med Adobe Experience Manager förbättrad anslutning

Du måste avinstallera Workfront med Adobe Experience Manager förbättrade anslutning till den senaste inbyggda integreringen som kopplar Workfront och Adobe Experience Manager Assets as a Cloud Service.

## Förutsättningar

* (Valfritt) Om det behövs kan du återställa ändringar som gjorts i Workfront brandväggskonfiguration och AEM.

## Avinstallera den förbättrade anslutningen

1. Kom åt och klona din AEM as a Cloud Service-databas från Cloud Manager.

1. Öppna din klonade Git-databas i den utvecklingsmiljö du väljer.

1. Checka ut den gren där den utökade anslutningen är installerad.

1. Navigera till följande sökväg och ta bort den förbättrade ZIP-filen för kopplingen:

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. Ta bort följande beroende från filen pom.xml i projektets rot.

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
   >Kontrollera att den version som refereras i ovanstående kodblock, dvs. 1.8.0, återspeglar den version som avinstalleras från koden.

1. Ta bort följande beroende från filen pom.xml i projektets undermodul med namnet **all**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. Ta bort följande inbäddade från filen pom.xml i projektets undermodul med namnet all.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (Villkorligt) Ta bort databaskonfigurationen från filen pom.xml i projektets rot.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (Villkorligt) Ta bort serverkonfigurationen från settings.xml, som finns i följande sökväg./cloudmanager/maven/settings.xml in the project root.&#39;

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

1. Genomför ändringarna och skicka koden till Cloud Manager-databasen

1. Kör Cloud Manager pipeline för att distribuera ändringarna på din Cloud Services-instans
