---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Konfigurera ett korrektur med ett automatiserat arbetsflöde i  [!DNL Workfront Proof]
description: Det här upprepas information som finns i Konfigurera korrektur i Workfront. Konsolidera här eller där. Kanske bättre här.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 0%

---

# Konfigurera ett korrektur med ett automatiserat arbetsflöde i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Automatiserat arbetsflöde gör det enklare för er att hantera granskning och godkännande av innehåll när ni har komplexa granskningsprocesser, eller om ni skickar innehåll för granskning till samma grupper av personer regelbundet.

Du skapar korrekturet och sedan går det från scen till scen tills det är slutgiltigt godkänt. De berörda användarna meddelas när de behöver göra ett godkännande.

![stage_chart.png](assets/stages-diagram-350x81.png)

Du kan lägga till ett automatiskt arbetsflöde i ett korrektur när du överför dokumentet, eller efter att dokumentet har överförts.

## Skapa ett korrektur med automatiserat arbetsflöde

1. Börja skapa korrekturet.
1. Klicka på **[!UICONTROL Use Automated Workflow]** i avsnittet **[!UICONTROL Share]**.

   Du kan avmarkera det här alternativet om du vill växla tillbaka till ett standardarbetsflöde.

1. (Valfritt) Om du vill använda en mall för automatiserat arbetsflöde som din [!DNL Workfront]-administratör har konfigurerat och delat med dig, markerar du den i listrutan **[!UICONTROL Select a Workflow template]**.

   >[!NOTE]
   >
   >Din möjlighet att ändra mallen beror på mallinställningarna som konfigurerats av administratören för [!DNL Workfront]. Om möjligheten att ändra mallen är inaktiverad kan bara mallens ägare ändra den.

1. Ange följande information för att konfigurera det första steget i det automatiserade arbetsflödet:

   * **[!UICONTROL Name]:** Scennamnet visas i arbetsflödesdiagrammet och inkluderas i e-postmeddelanden som skickas till granskare.
   * **[!UICONTROL Deadline]:** Funktionerna för det här fältet varierar beroende på vilket alternativ du väljer i listrutan **[!UICONTROL Deadline calculated from]**.

   * **[!UICONTROL From proof creation]:** Välj slutdatum för korrekturet.
   * **[!UICONTROL From stage activation]:** Välj det antal arbetsdagar som ska läggas till i scenens aktiveringsdatum för att automatiskt ange en deadline för korrekturet.
   * **[!UICONTROL Activate stage]:** För varje steg i arbetsflödet kan du bestämma när det ska aktiveras. Följande alternativ är tillgängliga för den första fasen.

      * Vid korrekturskapande
      * Vid en viss tidpunkt och ett visst datum
      * Manuellt\

        Ytterligare alternativ är tillgängliga för efterföljande steg. Dessa alternativ kräver en överordnad scen. De är:
      * Efter att föregående tidsgräns har nåtts
      * Alla beslut godkänns eller godkänns med ändringar
      * Alla beslut godkänns
      * Alla beslut fattas
   * **[!UICONTROL Deadline calculated from]:** Det alternativ du väljer i den här listrutan påverkar vilka alternativ som är tillgängliga i fältet **[!UICONTROL Deadline]**.

   * **[!UICONTROL Proof creation]:** I fältet **[!UICONTROL Deadline]** väljer du korrekturens deadline.

   * **[!UICONTROL Stage activation]:** I fältet **[!UICONTROL Deadline]** väljer du det antal arbetsdagar som ska läggas till i scenens aktiveringsdatum för att automatiskt ange en deadline för korrekturet.

   * **[!UICONTROL Lock stage]:** Välj när scenen kan låsas.
   * **[!UICONTROL Primary decision maker]:** Välj den primära beslutsfattaren på scenen. Beslutsfattare är bara tillgängliga i listrutan efter att du har lagt till granskare på scenen.
   * **[!UICONTROL Only one decision required]:** Välj det här alternativet om du vill att granskningen ska slutföras efter att en av beslutsfattarna har fattat sitt beslut.\

     Det här alternativet är inte tillgängligt om du har angett en användare i listrutan **[!UICONTROL Primary decision maker]**.

   * **[!UICONTROL Private stage]:** När det här alternativet är markerat är kommentarer och beslut inte synliga för personer som inte har lagts till på den här scenen eller som inte är tillsynsansvariga, administratörer eller faktureringsadministratörer i kontot


1. (Valfritt) Lägg till granskare på scenen.
1. Tänk på följande när du lägger till granskare:

   * En granskare kan bara läggas till i ett korrektur en gång. (Du kan inte lägga till samma person i mer än en fas i korrekturet.)
   * Granskare som läggs till på en privat scen kan bara se den scen de läggs till i korrekturet och kommentarerna som görs på den scenen.
   * Om du lägger till en användare på en scen får användaren som standard åtkomst till korrekturet från det att korrekturet skapas.\

     Systemadministratören kan konfigurera korrektursystemet för att hindra användare från att få åtkomst till korrekturet tills arbetsflödet går in i den fas där användaren lades till. Mer information finns i

1. (Valfritt) Klicka på **[!UICONTROL New stage]** och upprepa sedan steg 4 och steg 5 för att lägga till flera steg i det automatiserade arbetsflödet.
1. Fortsätt skapa korrekturet genom att ange nödvändig information i avsnitten [!UICONTROL Organize] och [!UICONTROL More settings] på sidan [!UICONTROL New Proof] enligt beskrivningen i

## Automatiserade arbetsflödesdiagram

När du ställer in arbetsflödet för ditt korrektur kommer du att se att ett diagram skapas. Alla steg som du lägger till i ditt korrektur visas i diagrammet, vilket tydligt anger beroendena mellan faserna. Privata faser markeras med en nyckelikon.

Diagrammet flyter, vilket betyder att det förblir synligt även om du rullar nedåt på sidan.

Om du inte behöver se diagrammet kan du dölja det (1).

![Diagram.png](assets/diagram-350x93.png)

## Lägga till en scen

Du kan lägga till ytterligare en fas i ett arbetsflöde som du skapar eller ändrar.

1. Om du lägger till en scen i ett befintligt korrektur går du till sidan Korrekturinformation, som beskrivs i [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Klicka på **[!UICONTROL New stage]** i avsnittet **[!UICONTROL Workflow]**.

1. Ange information för scenen som i steg 4 under avsnittet [!UICONTROL Creating a Proof with an Automated Workflow] i den här artikeln.
1. Klicka på **[!UICONTROL Add stage]** och sedan på **[!UICONTROL Done]**.

## Ta bort en scen

1. Klicka på papperskorgsikonen i det övre högra hörnet på scenen (1).\
   Ikonen visas när du hovrar över scenen.\
   ![deleting_a_stage.png](assets/deleting-a-stage-350x250.png)

## Sceninställningar

* **[!UICONTROL Stage name]**: Visas i arbetsflödesdiagrammet och inkluderas i e-postmeddelanden som skickas till granskare.
* **[!UICONTROL Activate stage]**: För varje steg i arbetsflödet kan du bestämma när det ska aktiveras. Följande alternativ är tillgängliga för den första fasen:

   * Vid korrekturskapande
   * Vid en viss tidpunkt och ett visst datum
   * Manuellt
   * Bara dessa tre alternativ är tillgängliga för ditt första steg. De andra alternativen blir tillgängliga när du lägger till en andra fas. De kräver att du väljer en överordnad scen.
   * Efter att föregående deadline har nåtts (ett överordnat stadium måste plockas)
   * Alla beslut är godkända eller [!UICONTROL Approved with changes] (kräver att en överordnad fas väljs)
   * Alla beslut är godkända (kräver att en överordnad fas väljs)
   * Alla beslut fattas (kräver att en överordnad fas väljs)

* **[!UICONTROL Deadline]:** Du kan bestämma hur deadline ska beräknas för varje steg i ett arbetsflöde. Alternativen är:

   * Från det att korrekturet skapas: I fältet [!UICONTROL deadline] (9) kan du välja slutdatum för korrekturet.
   * Från scenaktivering: I listrutan [!UICONTROL deadline] väljer du det antal arbetsdagar som ska läggas till i scenens aktiveringsdatum för att automatiskt ange en tidsgräns för korrekturet.

* **[!UICONTROL Lock]:** Det finns ett antal alternativ som avgör när en scen kan låsas. Alternativen är:

   * Manuellt lås
   * Aldrig
   * När nästa scen börjar
   * När alla beslut fattas

**[!UICONTROL Primary decision maker]**: Du ställer in den primära beslutsfattaren på scenen. De tillgängliga beslutsfattarna visas i listan först när du har lagt till granskarna på scenen.

>[!NOTE]
>
>Om du väljer en primär beslutsfattare är endast ett alternativ i det här skedet inte längre tillgängligt.

* **[!UICONTROL Only one decision required]**: Du kan aktivera det här alternativet på en scen. Detta innebär att översynen kommer att slutföras när en av beslutsfattarna fattar sitt beslut.
* **[!UICONTROL Privacy]:** Varje fas kan göras privat. Om en scen är privat visas inte kommentarerna och besluten för personer som inte har lagts till i den här fasen, eller som inte är tillsynsmyndigheter, administratörer eller faktureringsadministratörer i kontot. Mer information finns i [Översikt över automatiserat arbetsflöde](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Lägga till granskare på en scen

1. Ange ett kontaktnamn eller en e-postadress i fältet längst ned på varje fas.
1. Klicka på den gröna plusikonen för att lägga till dem.
1. Ange rollen för korrekturet.
1. Ange e-postavisering.
1. När du ställer in det första steget kan du också ändra korrekturets ägare.

   >[!NOTE]
   >
   >* En granskare kan bara läggas till i ett korrektur en gång. Du kan inte lägga till samma person i mer än en fas i korrekturet.
   >* Granskare som inte har lagts till på en privat scen kan inte se scenen på det korrektur eller de kommentarer som har gjorts på den scenen.


## Konvertera korrektur till automatiserat arbetsflöde

Du kan konvertera ett enkelt korrektur till ett automatiserat arbetsflöde.

1. Klicka på **[!UICONTROL Convert to Automated Workflow]** på sidan [!UICONTROL Proof details].
När korrekturet har omarbetats till automatiserat arbetsflöde är alla stadier aktiva, offentliga och deras [!UICONTROL Lock stage]-alternativ är inställt på Manuellt som standard. Alla faser finns kvar hos användarna och deras inställningar.

   * Aktiveringsfasen är inställd på Vid korrekturskapande i varje fas.
   * Deadline beräknad från alternativ är inställd på Korrekturskapande i varje fas.
   * Om endast ett beslutsalternativ valdes på det grundläggande beviset har alla faser det valt.
   * Om inget grundläggande korrektur [!UICONTROL Primary decision maker] valdes ställs faserna med den mottagaren in på dem och alla andra har värdet Ingen.
   * Scennamnet ändras inte.

## Lägga till ytterligare en mall i ett befintligt automatiserat arbetsflöde

När ett grundläggande korrektur har konverterats till ett automatiserat arbetsflöde kan du lägga till ytterligare mall i det.

1. Klicka på **[!UICONTROL Add template]i avsnittet Arbetsflöde på sidan Korrekturinformation.**

   * Mallinställningar avgör vad som kan göras med ett korrektur som den här mallen lades till i. Om mallen till exempel har [!UICONTROL Add a stage and Add people to stages]-alternativen inaktiverade visas inte knapparna till [!UICONTROL add stage] och [!UICONTROL share proof].
   * Om [!UICONTROL Add a stage option] är inaktiverat i den angivna mallen visas inte knappen [!UICONTROL Add template] när du har lagt till den.
   * När en person läggs till på en scen i en mall för automatiserat arbetsflöde, men redan finns på korrekturet, tas personen automatiskt bort från scenen om mallen används. Om ingen annan har lagts till i just det här steget visas följande fel eftersom systemet inte tillåter att en tom fas läggs till i arbetsflödet.

     ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
