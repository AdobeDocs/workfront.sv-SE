---
title: Förbättrad resurshantering i tredje kvartalet 2024
description: Förbättrad resurshantering i tredje kvartalet 2024
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 3a56518ecbcb85b443284402d0e273d6a8485fb2
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Förbättrad resurshantering i tredje kvartalet 2024

Den här sidan beskriver alla resurshanteringsförbättringar som gjorts i den tredje utgåvan av kvartal 2024 i förhandsvisningsmiljön. Dessa förbättringar kommer att göras tillgängliga i produktionsmiljön i den tredje utgåvan av kvartal 2024.

En lista över alla ändringar som är tillgängliga vid den här tidpunkten i den tredje utgåvan av kvartal 2024 finns på [Översikt över utgåvan för tredje kvartalet 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).

## Tidsgränsen återspeglas nu i arbetsbelastningsutjämnaren

>[!NOTE]
>
>Förhandsversion: 6 juni 2024; Produktion för snabb release: Med version 24.6 (20 juni 2024); Produktion för kvartalsvis release: Med version 24.7 (juli 2024)

För att smidigt justera arbete när den primära tilldelaren för en aktivitet har en schemalagd tid inaktiverad, omfördelar nu arbetsbelastningsutjämnaren timmar till både den primära och den sekundära användaren när projekttidslinjen beräknas om. (Den här funktionen är bara tillgänglig om Workfront-administratören har aktiverat inställningen för användartid av i inställningsområdet för att ta hänsyn till användarens ledig tid.)

Tidigare allokerades inte timmarna om när tidslinjen räknades om.

Mer information finns i [Hantera användarallokeringar i Utjämning av arbetsbelastning](/help/quicksilver/resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
