---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Ställ in ett korrektur med ett automatiserat arbetsflöde i [!DNL Workfront Proof]
description: Det här upprepas information som finns i Konfigurera korrektur i Workfront. Konsolidera här eller där. Kanske bättre här.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 0%

---

# Ställ in ett korrektur med ett automatiserat arbetsflöde i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Automatiserat arbetsflöde gör det enklare för er att hantera granskning och godkännande av innehåll när ni har komplexa granskningsprocesser, eller om ni skickar innehåll för granskning till samma grupper av personer regelbundet.

Du skapar korrekturet och sedan går det från scen till scen tills det är slutgiltigt godkänt. De berörda användarna meddelas när de behöver göra ett godkännande.

![stage_chart.png](assets/stages-diagram-350x81.png)

Du kan lägga till ett automatiskt arbetsflöde i ett korrektur när du överför dokumentet, eller efter att dokumentet har överförts.

## Skapa ett korrektur med automatiserat arbetsflöde

1. Börja skapa korrekturet.
1. I **[!UICONTROL Share]** avsnitt, klicka **[!UICONTROL Use Automated Workflow]**.

   Du kan avmarkera det här alternativet om du vill växla tillbaka till ett standardarbetsflöde.

1. (Valfritt) Om du vill använda en mall för automatiserat arbetsflöde som [!DNL Workfront] administratör konfigurerad och delad med dig, markera den i **[!UICONTROL Select a Workflow template]** nedrullningsbar meny.

   >[!NOTE]
   >
   >Din möjlighet att ändra mallen beror på mallinställningarna som konfigurerats av [!DNL Workfront] administratör. Om möjligheten att ändra mallen är inaktiverad kan bara mallens ägare ändra den.

1. Ange följande information för att konfigurera det första steget i det automatiserade arbetsflödet:

   * **[!UICONTROL Name]:** Scennamnet visas i arbetsflödesdiagrammet och inkluderas i e-postmeddelanden som skickas till granskarna.
   * **[!UICONTROL Deadline]:** Fältets funktionalitet varierar beroende på vilket alternativ du väljer i dialogrutan **[!UICONTROL Deadline calculated from]** nedrullningsbar lista.

   * **[!UICONTROL From proof creation]:** Välj slutdatum för korrekturet.
   * **[!UICONTROL From stage activation]:** Välj det antal arbetsdagar som ska läggas till på scenens aktiveringsdatum för att automatiskt ange en deadline för korrekturet.
   * **[!UICONTROL Activate stage]:** För varje steg i arbetsflödet kan du bestämma när det ska aktiveras. Följande alternativ är tillgängliga för den första fasen.

      * Vid korrekturskapande
      * Vid en viss tidpunkt och ett visst datum
      * Manuellt\

         Ytterligare alternativ är tillgängliga för efterföljande steg. Dessa alternativ kräver en överordnad scen. De är:
      * Efter att föregående tidsgräns har nåtts
      * Alla beslut godkänns eller godkänns med ändringar
      * Alla beslut godkänns
      * Alla beslut fattas
   * **[!UICONTROL Deadline calculated from]:** Det alternativ du väljer i den här listrutan påverkar vilka alternativ som är tillgängliga i **[!UICONTROL Deadline]** fält.

   * **[!UICONTROL Proof creation]:** I **[!UICONTROL Deadline]** markerar du deadlinedatum för korrekturet.

   * **[!UICONTROL Stage activation]:** I **[!UICONTROL Deadline]** ska du välja antalet arbetsdagar som ska läggas till på scenens aktiveringsdatum för att automatiskt ange en deadline för korrekturet.

   * **[!UICONTROL Lock stage]:** Välj när scenen kan låsas.
   * **[!UICONTROL Primary decision maker]:** Välj primär beslutsfattare på scenen. Beslutsfattare är bara tillgängliga i listrutan efter att du har lagt till granskare på scenen.
   * **[!UICONTROL Only one decision required]:** Välj det här alternativet om du vill att granskningen ska slutföras när en av beslutsfattarna fattar sitt beslut.\

      Det här alternativet är inte tillgängligt om du har angett en användare i **[!UICONTROL Primary decision maker]** nedrullningsbar meny.

   * **[!UICONTROL Private stage]:** När det här alternativet är markerat är kommentarer och beslut inte synliga för personer som inte har lagts till i det här steget eller som inte är tillsynsmyndigheter, administratörer eller faktureringsadministratörer i kontot


1. (Valfritt) Lägg till granskare på scenen.
1. Tänk på följande när du lägger till granskare:

   * En granskare kan bara läggas till i ett korrektur en gång. (Du kan inte lägga till samma person i mer än en fas i korrekturet.)
   * Granskare som läggs till på en privat scen kan bara se den scen de läggs till i korrekturet och kommentarerna som görs på den scenen.
   * Om du lägger till en användare på en scen får användaren som standard åtkomst till korrekturet från det att korrekturet skapas.\

      Systemadministratören kan konfigurera korrektursystemet för att hindra användare från att få åtkomst till korrekturet tills arbetsflödet går in i den fas där användaren lades till. Mer information finns i

1. (Valfritt) Klicka på **[!UICONTROL New stage]** och sedan upprepa steg 4 och steg 5 för att lägga till flera steg i det automatiserade arbetsflödet.
1. Fortsätt skapa korrekturet genom att ange nödvändig information i [!UICONTROL Organize] och [!UICONTROL More settings] i [!UICONTROL New Proof] sida, enligt beskrivning i

## Automatiserade arbetsflödesdiagram

När du ställer in arbetsflödet för ditt korrektur kommer du att se att ett diagram skapas. Alla steg som du lägger till i ditt korrektur visas i diagrammet, vilket tydligt anger beroendena mellan faserna. Privata faser markeras med en nyckelikon.

Diagrammet flyter, vilket betyder att det förblir synligt även om du rullar nedåt på sidan.

Om du inte behöver se diagrammet kan du dölja det (1).

![Diagram.png](assets/diagram-350x93.png)

## Lägga till en scen

Du kan lägga till ytterligare en fas i ett arbetsflöde som du skapar eller ändrar.

1. Om du lägger till en scen i ett befintligt korrektur går du till sidan med korrekturinformation, som beskrivs på [Hantera korrekturinformation i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. I **[!UICONTROL Workflow]** avsnitt, klicka **[!UICONTROL New stage]**.

1. Ange information för scenen som i steg 4 under [!UICONTROL Creating a Proof with an Automated Workflow] i den här artikeln.
1. Klicka **[!UICONTROL Add stage]** och sedan klicka **[!UICONTROL Done]**.

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
   * Bara dessa tre alternativ är tillgängliga för ditt första steg. De andra alternativen blir tillgängliga när du lägger till en andra fas; kräver du att du väljer en överordnad scen.
   * Efter att föregående deadline har nåtts (ett överordnat stadium måste plockas)
   * Alla beslut godkänns eller [!UICONTROL Approved with changes] (kräver val av överordnad fas)
   * Alla beslut är godkända (kräver att en överordnad fas väljs)
   * Alla beslut fattas (kräver val av överordnad fas)

* **[!UICONTROL Deadline]:** Du kan bestämma hur deadline ska beräknas för varje steg i ett arbetsflöde. Alternativen är:

   * Från korrekturskapande: I [!UICONTROL deadline] fält (9) kan du välja slutdatum för korrekturet.
   * Från och med scenaktiveringen: I [!UICONTROL deadline] väljer du hur många arbetsdagar som ska läggas till på scenens aktiveringsdatum för att automatiskt ange en deadline för korrekturet.

* **[!UICONTROL Lock]:** Det finns ett antal alternativ som avgör när en scen kan låsas. Alternativen är:

   * Manuellt lås
   * Aldrig
   * När nästa scen börjar
   * När alla beslut fattas

**[!UICONTROL Primary decision maker]**: Du satte den primära beslutsfattaren på scenen. De tillgängliga beslutsfattarna visas i listan först när du har lagt till granskarna på scenen.

>[!NOTE]
>
>Om du väljer en primär beslutsfattare är endast ett alternativ i det här skedet inte längre tillgängligt.

* **[!UICONTROL Only one decision required]**: Du kan aktivera det här alternativet på en scen. Detta innebär att översynen kommer att slutföras när en av beslutsfattarna fattar sitt beslut.
* **[!UICONTROL Privacy]:** Varje steg kan göras privat. Om en scen är privat visas inte kommentarerna och besluten för personer som inte har lagts till i den här fasen, eller som inte är tillsynsmyndigheter, administratörer eller faktureringsadministratörer i kontot. Mer information finns i [Översikt över automatiserat arbetsflöde](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

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



## Konvertera ett korrektur till ett automatiserat arbetsflöde

Du kan konvertera ett enkelt korrektur till ett automatiserat arbetsflöde.

1. Klicka på **[!UICONTROL Convert to Automated Workflow]** på sidan [!UICONTROL Proof details].
När korrekturet har omarbetats till automatiserat arbetsflöde är alla stadier aktiva, offentliga och deras [!UICONTROL Lock stage] är inställt på Manuell som standard. Alla steg finns kvar hos användarna och deras inställningar.

   * Aktiveringsfasen är inställd på Vid korrekturskapande i varje fas.
   * Deadline beräknad från alternativ är inställd på Korrekturskapande i varje fas.
   * Om endast ett beslutsalternativ valdes på det grundläggande beviset har alla faser det valt.
   * Om det finns grundläggande bevis [!UICONTROL Primary decision maker] markerades, ställs stadier med den mottagaren in på dem och alla andra har värdet Ingen.
   * Scennamnet ändras inte.

## Lägga till ytterligare en mall i ett befintligt automatiserat arbetsflöde

När ett grundläggande korrektur har konverterats till ett automatiserat arbetsflöde kan du lägga till ytterligare mall i det.

1. På sidan Korrekturinformation i avsnittet Arbetsflöde klickar du på **[!UICONTROL Add template].**

   * Mallinställningar avgör vad som kan göras med ett korrektur som den här mallen lades till i. Om mallen till exempel har [!UICONTROL Add a stage and Add people to stages] inaktiverade alternativ, knappar till [!UICONTROL add stage] och [!UICONTROL share proof] kommer inte att synas.
   * If [!UICONTROL Add a stage option] är inaktiverat i den angivna mallen när den har lagts till [!UICONTROL Add template] knappen inte visas.
   * När en person läggs till på en scen i en mall för automatiserat arbetsflöde, men redan finns på korrekturet, tas personen automatiskt bort från scenen om mallen används. Om ingen annan har lagts till i just det här steget visas följande fel eftersom systemet inte tillåter att en tom fas läggs till i arbetsflödet.

      ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
