---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Så här fungerar Workfront migrering till Adobe Admin Console
description: Så här fungerar Workfront produkt- och användarmigrering till Adobe Admin Console
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: 0a638b143d2de4b8ff2948e701ee90acbd1ab857
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 0%

---

# Så här fungerar Workfront migrering till Adobe Admin Console

Adobe förändrar hur du hanterar dina Adobe Workfront-användare och ökar produktiviteten för dig och din organisation. Som en del av den här ändringen migrerar Adobe din Workfront-instans och dina användare till Adobe Admin Console. Detta är en nödvändig migrering och påverkar inte rapporter, godkännandesökvägar, innehåll eller resurser. Det påverkar hur du hanterar användaråtkomst och hur användarna loggar in.

Mer information om hur du kan använda Adobe Admin Console för att hantera dina Adobe i hela organisationen finns i [Hantera användare i Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Vad är Changing?

Som en del av migreringen kommer din användarhantering att flyttas från Workfront till Adobe Admin Console med följande administrativa roller:

* **Systemadministratörer** är superanvändare med behörighet för alla administratörer. De tilldelar alla administrativa roller och hanterar användare för hela organisationen för alla produkter.

* **Produktprofiladministratörer (Workfront systemadministratörer)** hantera vilka användare i organisationen som får tillgång till Workfront.

* **Användare loggar in med Adobe-identitet.** När Adobe har migrerat befintliga användare till Adobe Admin Console loggar användare in på sina Workfront-instanser med sin nya Adobe-identitet, antingen ett Adobe ID- eller Adobe-Federated ID (SSO).

* **Det finns ingen förändring i hur du hanterar alla andra funktioner** i själva Workfront-programmet, inklusive hantering av funktioner, användarroller, arbetsytor, funktionalitet och beteende.

## Tidslinje för migreringsresa

Adobe migrerar din Workfront-instans till Adobe Admin Console först och migrerar sedan alla befintliga användare med verifierade e-postadresser. Om du är systemadministratör eller administratör för Workfront produktprofil (Workfront-systemadministratör) får du e-postmeddelanden som guidar dig genom migreringsresan. Här är en tidslinje för vad du kan förvänta dig:

### Workfront Migration to Adobe Admin Console Complete

Systemadministratörer får ett e-postmeddelande när Workfront migrering till Adobe Admin Console är klar. För närvarande kan systemadministratörer behöva slutföra några nödvändiga steg **innan användarmigreringen startar**, för att minimera påverkan för Workfront-användare.

* **Om dina Workfront-användare loggar in med enkel inloggning** måste du konfigurera enkel inloggning på Adobe Admin Console så att dina användare kan fortsätta logga in med enkel inloggning. Om dina Workfront-användare för närvarande inte använder enkel inloggning, men du vill konfigurera den på Adobe Admin Console, kan du göra det nu under migreringsresan.
* **Om du redan hanterar andra Adobe-produkter i din Adobe Admin Console** kan Adobe begära ditt samtycke för att automatiskt migrera användare till din befintliga konsol. Klicka på **Kom igång** i e-postmeddelandet för att navigera till sidan för godkännande.
* **Om du tidigare har tagit bort licenstypen för begärande** läggs den till i systemet. Inga användare tilldelas den här licenstypen, men det krävs för synkroniseringen mellan Workfront och Adobe Admin Console. Du behöver inte vidta någon åtgärd för den begärande licenstypen.

Användarhanteringen förändras inte just nu. Workfront-administratörer fortsätter att hantera användare i Workfront, och användare fortsätter att logga in med sitt Workfront ID eller SSO tills användarmigreringen är klar.

### Schemalägg användarmigrering

När systemadministratören har slutfört de krav som beskrivs i föregående avsnitt schemalägger Adobe automatiskt din användarmigrering i 30 dagar efter att dessa krav är klara och kommer att kommunicera med Workfront produktprofiladministratörer (Workfront-systemadministratörer) för att hantera användarmigreringen.

Workfront produktprofiladministratörer (Workfront systemadministratörer) kan:

* Få ett e-postmeddelande med startdatum för den schemalagda användarmigreringen (cirka 30 dagar efter att dessa krav är slutförda)
* Få tillgång till den utsedda Workfront-administratörskonsolen där de kan ändra migreringsdatumet

  >[!NOTE]
  >
  >På grund av migreringens komplexitet begränsas datumändringar till högst 30 dagar efter det schemalagda datumet. Kontakta supporten om du behöver ett senare datum.

* Få en påminnelse via e-post 1 dag före startdatumet för användarmigreringen

### Förbered användare för migreringsdagen

Som administratör för Workfront produktprofil (Workfront-systemadministratör) ansvarar du för att se till att alla användare är förberedda för migreringsdagen.

* Förbered alla användare för den kommande migreringen till Adobe Identity genom att meddela dem följande:

   * När användare migrerar får de ett e-postmeddelande från Adobe som meddelar dem om förändringen i det sätt de loggar in på Workfront. Användare kommer att uppmanas att acceptera en inbjudan att logga in med Adobe Identity för första gången, antingen genom att logga in med en befintlig Adobe ID eller genom att konfigurera en ny med samma e-postadress.

### Vad man kan förvänta sig på migreringsdagen

* **Migreringen av användare startar vid midnatt när kundens Workfront Datacenter är värd.**

* **Adobe migrerar automatiskt Workfront-administratörer först.** När Workfront-administratörer migreras till Adobe Identity får de rollen som Adobe-produktprofiladministratör (Workfront-systemadministratör). Befintliga roller som en användare kan ha innan migreringen påverkas inte.

  >[!NOTE]
  >
  >Åtkomsten till produkten kommer inte att gå förlorad under migreringen av användaren. Om en användare är inloggad under den tid användaren migreras påverkas inte. När de loggar in nästa gång måste de dock använda sin Adobe-identitet.



* **När användare migreras får de ett e-postmeddelande från Adobe som meddelar dem om ändringen av det sätt på vilket de loggar in på Workfront.** Användare kommer att uppmanas att acceptera en inbjudan att logga in med Adobe Identity för första gången, antingen genom att logga in med en befintlig Adobe ID eller genom att konfigurera en ny Adobe ID med samma e-postadress.

  Mer information om hur du loggar in på Workfront med en Adobe ID finns i [Logga in på Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Användarmigreringen är klar

Adobe kommer att meddela alla systemadministratörer och produktprofiladministratörer (Workfront systemadministratörer) via e-post när alla administratörer och användare har migrerats. Nu loggar alla Workfront-användare in på Workfront med Adobe Identity. Workfront systemadministratörer och produktprofiladministratörer (Workfront systemadministratörer) kan hantera användaråtkomst inom Adobe Admin Console. Om kunderna inte använder någon form av katalogsynkronisering i administratörskonsolen kan de fortsätta att hantera åtkomst till Workfront i Workfront-programmet.

## Få support

Om du har frågor eller funderingar följer du de steg som beskrivs i artikeln [Kontakta kundsupport](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




