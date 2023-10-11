---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Konfigurera eftersläpningen på en arbetsyta
description: Du kan välja att visa en eftersläpande kolumn på en anslagstavla i ett arbetsflöde och definiera en fråga för korten som hämtas till eftersläpningen i arbetsflödets kortlista.
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 4e5bff5ad62dce8766072e04e3a2b89371a90f03
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---

# Konfigurera eftersläpningen på en arbetsyta

>[!IMPORTANT]
>
>Arbetsflöden är bara tillgängliga för en viss kundgrupp.

Du kan välja att visa en eftersläpande kolumn på en anslagstavla i ett arbetsflöde och definiera en fråga för korten som hämtas till eftersläpningen i arbetsflödets kortlista.

>[!NOTE]
>
>Om du lägger till ett nytt kort i kolumnen för eftersläpning som inte matchar frågevillkoren, kommer kortet att försvinna från eftersläpningen när kortet uppdateras och kommer endast att vara tillgängligt i kortlistan. Du kan när som helst ändra frågan för att justera vilka kort som visas i kolumnen med eftersläpningar.

Eftersläpningskolumnen och frågan är inte tillgängliga på fristående anslagstavlor. Mer information om hur du lägger till en inloppskolumn på en fristående bräda finns i [Lägga till en inloppskolumn på en anslagstavla](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Konfigurera eftersläpningen på en arbetsyta

{{step1-to-boards}}

1. Öppna arbetsflödet som du vill arbeta i. Om du vill öppna ett arbetsflöde klickar du på [!UICONTROL **Visa arbetsflöde**].
1. Klicka på ett bord i arbetsflödet för att öppna det.
1. Klicka [!UICONTROL **Konfigurera**] till höger om ritytan för att öppna panelen Konfigurera.
1. Aktivera [!UICONTROL **Inkludera en kolumn för eftersläpning på den här ritytan**].

   Eftersläpningskolumnen läggs till till till vänster om anslagstavlan. Den är tom tills du använder en fråga.

1. Expandera [!UICONTROL **Eftersläpningsfråga**].

   >[!NOTE]
   >
   >En standardfråga kan redan tillämpas på eftersläpningen, som visar alla arbetsobjekt från kortlistan som har en status och statusen inte Fullständig.

1. Klicka [!UICONTROL **Lägg till villkor**] och klicka i fältet&quot;tom&quot;.
1. Markera fältet som du vill fråga efter.

   De fält du kan välja är standardfält på ett kort.

1. Välj frågemodifieraren.

   Modifieringsalternativen beror på vilka fält de kan användas på. Fältet &quot;namn&quot; har till exempel inte &quot;större än&quot; eller &quot;mindre än&quot; som modifieringsalternativ eftersom dessa modifierare bara gäller för tal.

1. Markera värdet.

   Värdet är inte tillgängligt när du använder &quot;exists&quot; eller &quot;not exists&quot; som modifierare.

   Om du t.ex. väljer &quot;Förfallodatum&quot; och &quot;finns&quot; visas kort med tilldelade förfallodatum. Kort utan förfallodatum dras inte in i efterloggen.

1. (Valfritt) Klicka på [!UICONTROL **Lägg till villkor**] om du vill lägga till ytterligare ett villkor i frågan.

   ![Eftersläpningsfråga](assets/backlog-query-wrkstrm-board.png)

1. (Valfritt) Klicka på [!UICONTROL **Skapa grupp**] om du vill lägga till en grupp villkor som är kopplade till det första villkoret med en OR-operator.
1. Klicka [!UICONTROL **Spara fråga**].

   Frågan används och kort som uppfyller villkoren visas i kolumnen med eftersläpningar.
