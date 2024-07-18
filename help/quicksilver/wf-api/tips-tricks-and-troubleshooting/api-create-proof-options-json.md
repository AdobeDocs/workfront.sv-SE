---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Lägg in avancerade korrekturfunktioner med Adobe Workfront API
description: Lägg in avancerade korrekturfunktioner med Adobe Workfront API
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# Lägg till avancerade korrekturalternativ när du skapar ett korrektur via Adobe Workfront API

När du skapar ett korrektur i Workfront API kan du lägga till avancerade alternativ för korrektur.

Använd något av följande arbetsflöden för att lägga till korrekturalternativ i ett korrektur med API:

* (Rekommenderas) Skapa ett enkelt korrektur med Workfront API och lägg sedan till avancerade korrekturalternativ till korrekturet med API:t för Korrektur på HQ

* Skapa ett korrektur med avancerade korrekturalternativ med JSON i Workfront API

## Skapa ett korrektur med API:erna Workfront och ProofHQ (rekommenderas) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

I det här avsnittet beskrivs hur du skapar ett korrektur med avancerade alternativ för korrektur via Workfront API, med en kombination av API:erna för Workfront och Korrektur på HQ.

API:t ProofHQ innehåller en rad åtgärder som inte är tillgängliga för korrektur i Workfront API. Genom att använda dessa åtgärder kan du ändra eller konfigurera korrekturet med större precision än vad som finns i Workfront API.

En översikt över API:t för Korrektur för högdagrar finns i [Översikt över högdagrar](../../proofhq-api/general/overview.md). Du kan även läsa [Korrektur för HQ-dokumentation](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* Workfront API är ett REST-fyllt API. API:t ProofHQ är ett SOAP API.
>* Korrektur som har skapats i API:t ProofHQ länkas inte automatiskt till Workfront. Därför rekommenderar vi att du skapar korrektur i Workfront API innan du uppdaterar dem med API:t ProofHQ.
>

### Skapa ett korrektur med avancerade korrekturfunktioner

1. Skapa ett korrektur med åtgärden `Document createProof` i Workfront API.

   >[!NOTE]
   >
   >När du skapar korrekturet anger du `{}` som värde för parametern `advancedProofingOptions`.

1. När korrekturet har skapats använder du API:t för Korrektur för att lägga till avancerade alternativ.

### Exempel

I det här avsnittet visas några exempeluppdateringar som du kan göra med API:t för Korrektur för högdagrar.

**Exempel:**

* [Ett korrektur kan hämtas, har ett meddelande och delas offentligt](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [Uppdatera en fas så att den inte är privat, inte obligatorisk och endast kräver ett godkännande](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Lägg till två mottagare i ett korrektur utan primär beslutsfattare](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**Ett korrektur kan hämtas, har ett meddelande och delas offentligt**

Dokumentation för den här slutpunkten finns på sidan [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html).

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**Uppdatera en fas så att den inte är privat, inte obligatorisk och endast kräver ett godkännande**

Dokumentation för den här slutpunkten finns på sidan [ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) .

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**Lägg till två mottagare i ett korrektur utan primär beslutsfattare**

Dokumentation för den här slutpunkten finns på sidan [ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html).

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Skapa ett korrektur med JSON i Workfront API

I det här avsnittet beskrivs hur du skapar ett korrektur med avancerade korrekturalternativ via Workfront API, med JSON som parametervärde i Workfront API

### Skapa ett korrektur med avancerade korrekturfunktioner

Du kan skapa korrektur med Workfront API genom att använda åtgärden `Document createProof`. Den här åtgärden accepterar parametern `advancedProofingOptions` som har värdetypen `string`. Om du vill inkludera avancerade korrekturalternativ i `createProof`-åtgärden måste du ange alternativen i parametern `advancedProofingOptions` i JSON-format.

>[!NOTE]
>
>Det kan vara svårt att förutsäga vilka fält som ska inkluderas i din avancerade korrekturinställningsalternativ för JSON. Du kanske vill granska organisationens nätverksdata samtidigt som du använder avancerad korrektur i Workfront och basera din JSON på de fält och värden som din organisation vanligtvis använder.
>
>Eftersom dessa fält kan vara svåra att förutse rekommenderar vi att du skapar ett korrektur med Workfront API och sedan uppdaterar det med API:t för Korrektur på HQ. Mer information finns i [Skapa ett korrektur med API:erna Workfront och ProofHQ (rekommenderas)](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) i den här artikeln

### Exempel

I det här exemplet visas fält och formatering som du kan använda när du skapar JSON för parametern `advancedProofingOptions`. JSON-filen `advancedProofingOptions` kan ha fler eller färre fält än vad som visas här.

**Exempel:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
