---
content-type: api
product-area: user-management
navigation-topic: general-api
title: Inaktivera en användare via API
description: Inaktivera en användare via API
author: John
feature: Workfront API
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Inaktivera en användare via API

När en användare lämnar organisationen kan du inaktivera användaren, göra Adobe Workfront-licensen tillgänglig för en annan användare och förhindra att de oavsiktligt tilldelas arbete. Genom att inaktivera en användare bevarar du användarens arbetshistorik, inklusive arbetsuppgifterna och kopplingen till anteckningar, timmar och dokument.

Mer information om hur du inaktiverar en användare finns i &quot; [Inaktivera eller återaktivera en användare](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Mer information om hur du använder Core API finns i [Grunderna i API](../../wf-api/general/api-basics.md).

Så här inaktiverar du en användare via API:

1. Generera en API-nyckel med följande API-begäran:

```
<domain>.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. Leta reda på GUID för användaren som du vill inaktivera.

   1. Använd följande API-begäran för att hämta GUID för alla användare i systemet. Observera att **isActive** fältvisning **true** för användare som är aktiva och **false** för användare som har inaktiverats:

```
<domain>`.my.workfront.com/attask/api/v7.0/USER/search?fields=isActive
```

1. Leta reda på GUID för användaren som du vill inaktivera med hjälp av följande **PUT** begäran om att ändra användarens **isActive** fältvärde till **false**:

```
<domain>`.my.workfront.com/attask/api/v7.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. Svaret visar att **isActive** fältvärdet har ändrats från **true** till **false** som anger att användaren har inaktiverats:

<!-- [Copy](javascript:void(0);) -->
<pre></pre>
