---
content-type: overview
product-area: projects
keywords: återkommande,återkomma,återkommer
navigation-topic: manage-tasks
title: Översikt över återkommande uppgifter
description: Översikt över återkommande uppgifter
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Översikt över återkommande uppgifter

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

Du kan skapa återkommande aktiviteter för aktiviteter som du måste upprepa som en del av ett enda projekt.

I den här artikeln beskrivs information och överväganden om hur du skapar och redigerar återkommande uppgifter.

Mer information om hur du skapar återkommande aktiviteter i Adobe Workfront finns i [Skapa återkommande aktiviteter](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## Översikt över återkommande uppgifter och överväganden

Du kan välja att skapa återkommande uppgifter för att ange upprepningsbart arbete under ett projekts livslängd.

Exempel: under ett IT-projekt behöver programvara med jämna mellanrum säkerhetskopieras. Om du skapar en återkommande uppgift för den här aktiviteten går det snabbare att ställa in flera enskilda uppgifter.

Tänk på följande när du skapar återkommande uppgifter i Workfront:

* Du kan inte lägga till återkommande uppgifter i en mall.
* Du kan inte lägga till en upprepningsfrekvens till en befintlig uppgift.
* Återkommande uppgifter visas som underaktiviteter eller underordnade för huvudförekomsten som visas som överordnad uppgift.
* Du kan inte bifoga ett godkännande till en överordnad återkommande uppgift.
* Workfront överför de flesta fält som du uppdaterar för den överordnade upprepningen när du skapar den till de underordnade uppgifterna. Följande fält överförs inte till de underordnade uppgifterna när de skapas:

   * Aktivitetsbegränsningen för de underordnade aktiviteterna ändras automatiskt till:

      * Måste starta på för projekt som planeras från startdatum.
      * Måste vara aktiverat för projekt som är planerade från slutförandedatum.

   * Dokument som är kopplade till det överordnade objektet överförs inte till de underordnade.

* Följande ändringar sker för den överordnade aktiviteten när du har angett att uppgiften är återkommande:

   * Fältet Varaktighet har bytt namn till Varaktighet per förekomst för den överordnade aktiviteten. Den behåller längden för de underordnade aktiviteterna.
   * Status är inaktiverad för den överordnade aktiviteten och ställs automatiskt in på Nytt för de underordnade. Den överordnade aktiviteten slutförs automatiskt och statusen uppdateras till Fullständig när alla underordnade har slutförts.
   * De enda varaktighetstyperna som är tillgängliga för återkommande uppgifter är:

      * Enkel
      * Ansträngningsstyrd
* Varaktighet och Planerade timmar som anges för en ny återkommande aktivitet är Varaktighet och Planerade timmar för varje förekomst. Den överordnade aktivitetens varaktighet är tiden mellan det planerade startdatumet för den första aktiviteten och det planerade slutförandedatumet för den senaste aktiviteten. Den överordnade uppgiftens planerade timmar är det totala antalet planerade timmar från alla förekomster.

## Att tänka på vid redigering av återkommande uppgifter

Vissa ändringar som du gör i en återkommande överordnad aktivitet kanske inte uppdateras för alla befintliga förekomster. Underordnade aktiviteter som visar förloppet eller har uppdaterats individuellt uppdateras inte när du uppdaterar det överordnade objektet. Workfront anser att en uppgift visar förloppet i följande situationer:

* Status uppdateras och aktiviteten är inte längre Ny
* Uppgiftens Procent färdigt är högre än noll
* Aktiviteten har överordnade relationer

I följande tabell visas om ändringar som gjorts i den överordnade utlösaren uppdateras på de underordnade objekt som inte har redigerats individuellt eller om förloppet visas:

| Fält som har uppdaterats för den överordnade aktiviteten | Uppdateringar överförs till oredigerade underordnade eller underordnade utan att några framsteg registreras |
|---|---|
| Återkommande frekvens* | ✔ |
| Uppdrag | ✔ |
| Namn | ✔ |
| Beskrivning | ✔ |
| Prioritet | ✔ |
| Varaktighet | ✔ |
| Planerade timmar | ✔ |
| Kostnadstyp | ✔ |
| Intäktstyp | ✔ |
| Resursutjämning | ✔ |
| Levelingfördröjning | ✔ |
| Aktivitetsbegränsning | Uppdaterar inte underordnade |
| Bifoga eller ta bort anpassad Forms | Uppdaterar inte underordnade |
| Varaktighetstyp | Uppdaterar inte underordnade |
| Anpassad formulärinformation | Uppdaterar inte underordnade |

{style="table-layout:auto"}

&#42; Följande scenarier finns när du uppdaterar upprepningsfrekvensen för en överordnad aktivitet:

* Om du ändrar upprepningsfrekvensen för en befintlig överordnad uppgift, tas de befintliga underuppgifterna bort och ersätts med nya underaktiviteter som följer den nya upprepningsfrekvensen om de inte visar några förlopp och om du inte har uppdaterat dem manuellt.
* Om du ändrar upprepningsfrekvensen för en befintlig överordnad uppgift tas inte underaktiviteter som visar förloppet bort. Dessa uppgifter anses vara åtskilda från upprepningen vid den här tidpunkten.

&#42;&#42; tilldelningar som görs för den överordnade aktiviteten tillämpas på alla underaktiviteter i upprepningen. Alla ändringar som görs i tilldelningen för den överordnade aktiviteten åsidosätter eventuella enskilda tilldelningar för underaktiviteten. Om aktiviteten visar förlopp ändras inte uppdraget.

 
