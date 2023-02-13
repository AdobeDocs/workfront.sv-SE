---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Förbättrad projektledning
description: Den här sidan beskriver alla projekthanteringsförbättringar som gjorts i version 20.3 till produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 10 augusti 2020.
author: Luke
feature: Product Announcements
exl-id: acde4cf2-a755-4e77-9469-f5152991dd34
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 20.3 Förbättrad projektledning

Den här sidan beskriver alla projekthanteringsförbättringar som gjorts i version 20.3 till produktionsmiljön. Dessa förbättringar gjordes tillgängliga i produktionsmiljön den 10 augusti 2020.

En lista över alla ändringar som är tillgängliga i version 20.3 finns i [20.3 versionsöversikt](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Anpassad fältformatering i listor

>[!NOTE]
>
>Den här funktionen stöds endast i den nya Adobe Workfront-upplevelsen. Den är tillgänglig för vissa listor i Adobe Workfront Classic, men stöds inte i Adobe Workfront Classic.

Nu när systemadministratören skapar anpassade formulärfält som är konfigurerade för formatering kan du formatera text i de fält där du använder dem mest: i listor i hela Workfront. I stället för att gå in i området Detaljer och formatera text i det anpassade formuläret kan du klicka på ett fält i en lista och använda Fet, Kursiv och Understruken för text där.

Observera att den här funktionen bara är tillgänglig i de uppdaterade listorna. Mer information om uppdaterade listor finns i [Kom igång med listor i Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Information om hur en Workfront-administratör skapar textfält med formatering finns i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Uppdaterat utseende och känsla för flera globala rubriker

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen

De globala områdena Projekt, Portfolio, Program och Mallar har nu ett uppdaterat sidhuvud som bättre utnyttjar utrymmet på skärmen. Den här uppdateringen ger mer utrymme för den information du arbetar med och som du behöver fokusera på.

Länken Mallar från projektområdet har tagits bort. Du kan fortfarande öppna området Mallar från huvudmenyn.

## Ny redigeringsprojektruta

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen

Som en del av att uppdatera utseendet och känslan i den nya Workfront-upplevelsen har vi gjort om projektrutan Redigera. Du kan öppna den nya rutan Redigera projekt från ett enskilt projekt eller när du redigerar ett enskilt projekt från en lista.

Förutom ett uppdaterat utseende och en uppdaterad känsla finns följande förbättringar i rutan Redigera projekt:

* Anpassa layoutmallen en gång och återge anpassningarna både på sidan Detaljer och i rutan Redigera objekt.
* Enskilda anpassade formulärnamn finns nu på den vänstra panelen i rutan Redigera projekt, och du kan snabbt komma åt de olika formulären därifrån.
* Kommentarsfunktionen tas bort från redigeringsprojektskärmen för att eliminera redundans med uppdateringsavsnittet.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the new Edit Box box, see "New Edit Object box" (NEW ARTICLE, LINK LATER!!).</p>
-->

Mer information om den nya rutan Redigera projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

## Ny sammanfattningspanel och förbättringar av uppdateringarna för dokumentlistan

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen

Den nya panelen Sammanfattning till höger om dokumentlistan är nu tillgänglig med en förbättrad design i den nya Workfront-upplevelsen. Panelen innehåller samma åtgärder och information som finns på panelen till höger när du markerar ett dokument i Workfront Classic, inklusive dokumentinformation, uppdateringar, anpassad Forms, godkännanden och dokumentversioner.

Vissa åtgärder är inte tillgängliga just nu, men kommer att läggas till i en framtida version. Bland dessa åtgärder finns korrekturarbetsflödet.

Mer information finns i [Sammanfattning av dokumentöversikt](../../../documents/managing-documents/summary-for-documents.md).

## Förbättringar i dokumentinformation

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i den nya Adobe Workfront-upplevelsen

Sök efter följande förbättringar på sidan Dokumentinformation:

* Nya versionsalternativ har flyttats till en listruta nära den vänstra panelen, vilket ger enklare åtkomst.
* Ikonen för öppet korrektur har ändrats till en etikett för öppet korrektur, vilket gör det enklare att se på sidan.
* Större miniatyrbild för förhandsgranskning så att du enkelt kan identifiera dokumentet
* Ikonen Global redigering har lagts till, vilket ger dig möjlighet att redigera flera fält samtidigt.

Mer information finns i [Översikt över dokumentinformation](../../../documents/managing-documents/document-details-overview.md).

## För administratörer: Ange projektinställningar på gruppnivå

>[!NOTE]
>
>Den här funktionen är för närvarande inte tillgänglig för de flesta kunder i kluster 1, 2, 3 och 5. Den här sidan uppdateras när funktionaliteten återställs för alla kunder.

För att ge gruppadministratörerna mer självbestämmande och för att göra det möjligt att anpassa arbetsflödena på gruppnivå kan du nu definiera dina projektinställningar på gruppnivå för grupper som du administrerar. När du skapar ett projekt börjar gruppens inställningar gälla före systemets.

Alla projektinställningar kan anpassas på gruppnivå, förutom för tidslinjeberäkningar och anpassade kvartal.

Mer information om inställningar för gruppprojekt finns i [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

## Nytt för administratörer: Skapa anpassade formulärfält där användarna kan formatera text

I ett anpassat formulär kan du nu skapa fält som innehåller textformateringsknappar. När användare skriver i dessa fält kan de markera och ordna texten med fet stil, kursiv stil och understrykning. Den höga teckengränsen på 15 000 tillåter mycket text och formatering.

Mer information finns i Skapa ett anpassat formulär i den nya Workfront-upplevelsen.

## Nytt för administratörer: Skapa både ett internt namn och en etikett som användaren vänder sig till för ett eget formulärfält

Om du vill ha större flexibilitet när det gäller etiketter och ommärkning av anpassade formulärfält kan du nu skapa en intern *name* för ett fält utöver användaren *label* du har använt. Detta ger dig frihet att ändra den fältetikett som visas för användarna utan att ändra fältnamnet som visas i systemet.

Tidigare visades etiketten både ovanför fältet för användare och användes av systemet för att identifiera fältet. Om du ändrade etiketten för användare så fungerade inte fältet som det var när det användes, eftersom systemet inte längre kunde identifiera det.

Mer information finns i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

