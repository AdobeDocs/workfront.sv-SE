---
title: Översikt över formulärdesignern
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan utforma ett anpassat formulär som användare kan bifoga till ett Workfront-objekt. Användare som arbetar med objektet kan fylla i det anpassade formuläret för att ge information om objektet.
author: Courtney / Lisa
feature: System Setup and Administration
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: ad04b732adac345bc015bb290dfd12898bb0a604
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Översikt över formulärdesignern

Du kan använda den nya formulärdesignern för att utforma ett anpassat formulär som användare kan koppla till ett Workfront-objekt. Användare som arbetar med objektet kan fylla i det anpassade formuläret för att ge information om objektet.

Den nya formulärdesignern har en ny arbetsyteliknande arbetsyta som gör att du kan visa fälten, arbetsytan och fältinställningarna samtidigt. Du kan också dra och släppa fält i avsnitten när du utformar formuläret.

<!-- add screenshot when field settings empty state is ready -->

## Hur man kommer åt den nya formulärdesignern

Det finns en ny knapp längst upp i både den nya formulärdesignern och den äldre formulärbyggaren. Du kan använda den här knappen för att växla mellan det äldre verktyget och det nya designverktyget.

![Växla till ny formulärdesigner](assets/switch-views.png)

## Nya funktioner som är tillgängliga för formulärdesignern

Med den nya formulärdesignern har vi lagt till möjligheten att

* **Kopiera ett fält**: Nu kan du kopiera befintliga fält genom att klicka på ikonen Kopiera på fälten direkt från arbetsytan.

* **Ändra storlek för beskrivande text**: Du kan nu tilldela små, medelstora eller stora storlekar till beskrivande textfält. Du kan också använda dem på samma rad med andra fält.

* **Använd ett standardavsnitt**: Om den som har skapat formuläret inte har lagt till något avsnitt överst i formuläret visas nu standardavsnittet på arbetsytan, så att användare kan justera behörigheten för fält som inte har något anpassat avsnitt tilldelat.

  >[!NOTE]
  >
  >Standardavsnittet är inte synligt i objekt när formuläret har kopplats till objektet.

## Funktioner kommer snart

Följande är för närvarande inte tillgängligt i formulärdesignern, men kommer snart att läggas till:

* Visa/hoppa över logik

* Filter för typsnittsfält

>[!IMPORTANT]
>
>De befintliga konfigurationerna för logik- och typsnittsfilter påverkas inte när du arbetar med den nya formulärdesignern.

### Visa/hoppa över logik

Även om du ännu inte kan lägga till visnings-/hopplogik när du utformar ett nytt anpassat formulär, kan du visa befintlig visnings-/hopplogik i formulär som skapats i det äldre formulärbyggaren.

Ikoner i ett fält i formulärdesignern anger att logik används i fältet.

The ![Visningslogik för målfält](assets/display-logic-bottom-left.png) ikonen längst ned till vänster betyder att fältet är målfält för visningslogik (om ett visst val görs i formuläret visas det här fältet). The ![Definiera ikon för visningslogik](assets/display-logic-bottom-right.png) -ikonen längst ned till höger betyder att fältet används för att definiera visningslogik (ett specifikt val eller värde i det här fältet visar målfältet).

The ![Hoppa över logik för målfält](assets/skip-logic-bottom-left.png) ikonen längst ned till vänster betyder att fältet är målfält för hopplogik (om ett visst val görs i formuläret, hoppar formuläret framför det här fältet). The ![Definiera ikon för hopplogik](assets/skip-logic-bottom-right.png) ikonen längst ned till höger betyder att fältet används för att definiera hopplogik (en specifik markering eller ett värde i det här fältet hoppar över andra fält och går direkt till målfältet).

![Logic icons](assets/logic-icons-3.png)

Om du markerar ett fält med tillämpad logik visas de befintliga logikreglerna i fältinställningarna.

![Logikregler](assets/form-designer-view-only-logic.png)

## Funktioner som tagits bort från formulärdesignern

Vi har tagit bort följande funktioner från formulärdesignern:


* Formulärinställningar, Formulärdelning, Flikar för fältdelning

   * Formulärinställningarna är nu tillgängliga längst upp på arbetsytan

   * Huvudfliken Formulärdelning och underfliken Fältdelning

  >[!NOTE]
  >
  >Du kan styra formulär- och fältdelning via Konfigurera > Anpassad Forms > Forms eller fliken Fält.

* Spåra fältändringar i uppdateringsflöden
  >[!NOTE]
  >
  >Du hittar detta i Inställningar > Gränssnitt > Uppdatera feeds
