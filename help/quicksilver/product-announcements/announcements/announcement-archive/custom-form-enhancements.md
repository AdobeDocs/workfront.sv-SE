---
title: Förbättringar av anpassade formulär
description: Följande viktiga förbättringar har gjorts för hantering av anpassade formulär i version 22.2.
author: Luke
feature: Product Announcements, Custom Forms
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 0%

---

# Förbättringar av anpassade formulär

Följande viktiga förbättringar har gjorts för hantering av anpassade formulär i version 22.2.

## Lägg till resurswidgetar

Du kan bädda in bilder i dina anpassade formulär. På så sätt kan du kommunicera med anpassade formuläranvändare på ett mer interaktivt och visuellt sätt. Fler widgettyper kommer snart.

![Bild i anpassat formulär](assets/image-in-custom-form.png)

När ett anpassat formulär som innehåller en widget är kopplat till ett objekt kan användare som arbetar med objektet se det i följande områden:

* Objektets detaljområde (t.ex. för ett projekt, området Projektinformation) &#x200B;

  ![Bildinformation](assets/see-image-details-page.png)

* Rutan Redigera för objektet, om det har det nya Adobe Workfront-gränssnittet (t.ex. &#x200B; Redigera projekt och Redigera uppgift)

  ![Bildredigering](assets/image-see-in-edit.png)

Användarna kan för närvarande inte se widgeten i följande områden: &#x200B;

* Listor och rapporter
* Hem och sammanfattning
* Rutan Redigera för objektet, om det inte har det nya Adobe Workfront-gränssnittet (t.ex. rutan Redigera utgift)
* &#x200B; Workfront mobilapp

## Koppla ett anpassat formulär till flera objekttyper

Du kan koppla flera objekttyper till ett nytt anpassat formulär:

![Anpassade formulärobjekttyper](assets/new-custom-form-object-types.png)

Eller ett befintligt anpassat formulär:

![Lägg till objekttyp i formulär](assets/add-object-type-existing-form.png)

På så sätt kan du skapa ett anpassat formulär som kan användas i projekt, uppgifter, utgåvor och andra typer av objekt som kan användas i anpassade formulär.

Detta är särskilt användbart när du konverterar ett problem eller en uppgift eftersom du kan överföra ett anpassat formulär och dess data till det konverterade objektet. Du behöver inte längre skapa och underhålla exakta kopior av samma anpassade formulär för olika objekttyper. Lägg till det anpassade formuläret i projektet manuellt.

>[!INFO]
>
>**Exempel:**
>
>Någon skickar in en intern IT-förfrågan (utgåva) och ger information om vad som behövs i en bifogad anpassad blankett.
>
>Du konverterar ärendet till ett projekt för de användare som ska arbeta med det.
>
>Eftersom det anpassade formuläret som innehåller information om den som skickar in formuläret är kopplat till både utgåva och projektobjekttyper, överförs det anpassade formuläret och alla dessa detaljer till projektet under konverteringen.

>[!NOTE]
>
>När konverteringen sker måste det anpassade formuläret redan vara kopplat till den objekttyp som du konverterar till.

Tänk på följande när du skapar eller redigerar ett anpassat formulär med flera objekt:

* [Behörighetsalternativ för avsnittsbrytningar](#permission-options-for-section-breaks)
* [Beräknad kompatibilitet för anpassade fält](#calculated-custom-field-compatibility)
* [Varning om hur du tar bort en objekttyp från ett anpassat formulär](#caution-about-deleting-an-object-type-from-a-custom-form)

### Behörighetsalternativ för avsnittsbrytningar

Den uppsättning behörighetsalternativ för avsnittsbrytning som är tillgängliga för objekttyperna Utgåva, Aktivitet, Projekt och Användare har ett mer behörighetsalternativ än den uppsättning behörighetsalternativ som finns för alla andra objekttyper: Begränsad redigering.

![Avsnittsbrytning med begränsad redigering](assets/section-break-permissions-limited-edit.png)

De avsnittsbrytningsbehörigheter som är tillgängliga för alla andra objekttyper (Portfolio, Dokument, Program, Utgift, Företag, Iteration, Faktureringspost och Grupp) innehåller inte Begränsad redigering:

![Avsnittsbrytning utan begränsad redigering](assets/section-break-permissions-no-limited-edit.png)

I ett anpassat formulär som är associerat med objekttyper från båda dessa grupper använder systemet en gemensam uppsättning avsnittsbrytningsbehörigheter som fungerar för alla objekttyper. I stället för att använda behörighetsalternativet Begränsad redigering ersätter den här gemensamma uppsättningen behörighetsalternativet Redigera för behörighetsalternativet Begränsad redigering. Alternativet Redigera är kompatibelt med alla objekttyper.

När du associerar en objekttyp som använder andra behörighetsalternativ än de andra objekttyperna som redan finns i ett anpassat formulär, visas ett meddelande där du kan växla till den gemensamma uppsättningen behörighetsalternativ som används för formuläret. Den här ändringen gäller för alla fält, även om de inte är under en avsnittsbrytning.

### Beräknad kompatibilitet för anpassade fält

Om ett beräknat fält refererar till fält som är tillgängliga för användning med alla formulärets associerade objekttyper (till exempel {name}, {description} och {entryDate}, som är tillgängliga för flera objekttyper) i ett anpassat formulär med flera objekt, beräknas data korrekt, oavsett vilket objekt du kopplar det till.

Om du till exempel har ett formulär med flera objekt för projekt och utgåvor, och du lägger till ett beräkningsfält som innehåller uttrycket {name}, visas projektnamnet när du lägger till formuläret i ett projekt och aktivitetsnamnet där du lägger till formuläret i en uppgift.

Fält som inte är kompatibla med objektet kommer att visa N/A i formuläret.

>[!INFO]
>
>**Exempel:** I ett anpassat formulär som är associerat med aktivitetsobjekttypen skapar du ett beräknat anpassat fält som refererar till det inbyggda fältet Tilldelad: Namn, så att det kan visa namnet på den primära tilldelade personen när formuläret är kopplat till en uppgift:
>
>```
>Assigned To: Name{assignedTo}.{name}
>```
>
>Senare lägger du till objekttypen i det anpassade formuläret. Ett varningsmeddelande anger att projektobjekttypen inte är kompatibel med det beräknade anpassade fältet. Detta beror på att fältet Tilldelad till inte är tillgängligt för projekt.

När detta inträffar kan du göra något av följande:

* Ta bort ett av de två inkompatibla objekten från det anpassade formuläret, antingen objekttypen eller det refererade fältet.
* Behåll båda objekten och använd jokerteckensfiltervariabeln `$$OBJCODE` som ett villkor i ett IF-uttryck för att skapa två olika versioner av fältet I debitering. Detta gör att fältet kan fungera utan problem, oavsett vilken typ av objekt formuläret är kopplat till.

  I exemplet ovan finns det ett inbyggt fält för ägare (som automatiskt fylls i med namnet på den person som skapade projektet, såvida inte någon ändrar detta manuellt), även om det inte finns något inbyggt fält för Tilldelad: namn för projekt. I ditt anpassade avgiftsfält kan du använda `$$OBJCODE` så som visas nedan för att referera till fältet Ägare när det anpassade formuläret är kopplat till ett projekt, och fältet Tilldelad: Namn när formuläret är kopplat till en uppgift:

  ```
  IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
  ```

>[!NOTE]
>
>  Om du lägger till en objekttyp framför ett fältnamn refererar den till objektets överordnade objekt, så du kan inte använda `{project}.{name}` med ett projekt, men du kan använda den med en uppgift.


Mer information om variabler som `$$OBJCODE` finns i [Översikt över jokerteckensfiltervariabler](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### Varning om hur du tar bort en objekttyp från ett anpassat formulär

Du kan ta bort en objekttyp i ett anpassat formulär när som helst, men detta bör göras med försiktighet. Om användare redan har kopplat det anpassade formuläret till objekt av den typ som du vill ta bort och lagt till data i det, tas dessa data bort permanent när du tar bort den objekttypen i formuläret.

Det finns heller inget meddelandesystem för att varna personer som använder det anpassade formuläret om att det har tagits bort.

Mer information finns i [Ta bort ett anpassat fält eller en anpassad widget från systemet](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
