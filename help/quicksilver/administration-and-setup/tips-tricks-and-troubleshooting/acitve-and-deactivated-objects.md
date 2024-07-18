---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Aktiva och inaktiverade objekt
description: Som  [!DNL Adobe Workfront] administratör kan du aktivera eller inaktivera objekt i systemet. Vi rekommenderar att du aldrig tar bort objekt som du kan inaktivera. Du bör helt enkelt inaktivera objektet för att förhindra framtida användning och ta bort det från listrutorna för andra objekt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a0617270-e233-4ebe-a5ee-8df7a8a85823
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 0%

---

# Aktiva och inaktiverade objekt

Som [!DNL Adobe Workfront]-administratör kan du aktivera eller inaktivera objekt i systemet. Vi rekommenderar att du aldrig tar bort objekt som du kan inaktivera. Du bör helt enkelt inaktivera objektet för att förhindra framtida användning och ta bort det från listrutorna för andra objekt.

Om du till exempel vill se en viss [!UICONTROL Hour Type] måste [!UICONTROL Hour Type] vara aktiv. En inaktiv eller inaktiverad [!UICONTROL Hour Type] visas inte i den nedrullningsbara menyn [!UICONTROL Hour Type], men finns kvar i systemet för att behålla den historiska posten oförändrad där denna [!UICONTROL Hour Type] kan ha använts tidigare.

Termen &quot;Aktiv&quot; används för att identifiera om vissa objekt är aktiverade i systemet. I det här sammanhanget används &quot;Aktiv&quot; för följande objekt:

## E-postaviseringar

Du kan aktivera e-postmeddelanden så att vissa åtgärder kan aktivera e-postmeddelanden för alla användare.

Mer information om hur du aktiverar eller inaktiverar e-postmeddelanden finns i [Konfigurera händelsemeddelanden för alla i systemet](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Timtyper

Du kan aktivera timtyper så att de kan väljas av användare vid loggningstid.

Mer information om hur du aktiverar eller inaktiverar timtyper finns i [Hantera timtyper](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Portfolio

En portfölj måste vara aktiv för att kunna visas i formuläret [!UICONTROL New Project (Business Case)].

Du kan aktivera en portfölj när du redigerar den.

Mer information om hur du redigerar portföljer finns i [Skapa en portfölj](../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

## Program

Ett program måste vara aktivt för att kunna visas i fältet [!UICONTROL Program] för ett projekt.

Du kan aktivera ett program medan du redigerar programmet.

Mer information om hur du redigerar program finns i [Skapa ett program](../../manage-work/portfolios/create-and-manage-programs/create-program.md).

## Mallar

En mall måste vara aktiv för att kunna visas i mallfältet för ett projekt.

Du kan göra en mall aktiv när du redigerar mallen.

Mer information om hur du redigerar mallar finns i [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Godkännandeprocesser

En godkännandeprocess måste vara aktiv för att kunna visas i fältet [!UICONTROL Approval Process] för ett projekt, en aktivitet eller en utgåva.

Du kan aktivera en godkännandeprocess medan du redigerar godkännandeprocessen.

Mer information om hur du redigerar godkännandeprocesser finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Milstolpbanor

En milstolpe-sökväg måste vara aktiv för att kunna visas i fältet [!UICONTROL Milestone Path] för ett projekt.

Du kan göra en milstolpe-bana aktiv när du redigerar milstolpen.

Mer information om hur du redigerar milstolpebanor finns i [Skapa en milstolpebana](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

## Egna formulär

Ett anpassat formulär måste vara aktivt för att kunna visas i fältet [!UICONTROL Custom Form] för ett annat objekt.

Du kan aktivera ett anpassat formulär när du redigerar det anpassade formuläret.

Mer information om hur du redigerar anpassade formulär och en lista över objekt som du kan associera dem med finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Företag

Ett företag måste vara aktivt för att kunna visas i fältet [!UICONTROL Company] för ett projekt, en användare eller en mall.

Du kan göra ett företag aktivt när du redigerar företaget.

Mer information finns i [Skapa och redigera företag](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Användare

En användare måste vara aktiv för att kunna visas i ett type-ahead-fält för alla andra objekt när han eller hon gör uppdrag eller delar dem.

Du kan inaktivera användare från användarsidan eller när du redigerar en användare.

Mer information om hur du inaktiverar användare finns i [Inaktivera eller återaktivera en användare](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

>[!IMPORTANT]
>
>Om din organisation har anslutit sig till [!DNL Adobe Business Platform] måste du inaktivera användare via [!UICONTROL Adobe Admin Console].
>
>Instruktioner om hur du inaktiverar en användare i [!UICONTROL Adobe Admin Console] finns i avsnittet Ta bort användare i artikeln [Hantera användare individuellt](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) eller kontakta [!UICONTROL Adobe Admin Console]-administratören.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till [!DNL Adobe Business Platform] finns i [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Team

Ett team måste vara aktivt för att kunna visas i alla typografiska framfält för alla andra objekt när du gör uppdrag eller delar dem.

Du kan inaktivera team när du redigerar ett team.

Mer information om hur du inaktiverar team finns i [Inaktivera ett team](../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md).

## Jobbroller

En jobbroll måste vara aktiv för att kunna visas i ett type-ahead-fält för alla andra objekt när du gör tilldelningar eller delar dem.

Du kan inaktivera jobbroller när du redigerar dem.

Mer information om hur du inaktiverar jobbroller finns i [Inaktivera jobbroller](../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).
