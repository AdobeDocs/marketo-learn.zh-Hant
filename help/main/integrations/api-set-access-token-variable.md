---
title: Marketo如何API影片 — 如何在變數中設定存取權杖
description: 瞭解如何設定Postman應用程式，以及如何運用變數將資料儲存至變數，以利重複使用。
feature: REST API
role: Admin, Developer
level: Experienced
doc-type: Technical Video
duration: 772
last-substantial-update: 2024-08-06T00:00:00.000Z
jira: KT-15548
exl-id: 4da86ed6-1072-4e0e-a648-16587badaeb3
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: dca84292-69e9-4116-a575-667d31fa060d
    internal-label: APIs
subfeature_v2:
  - id: cf1396d8-ab85-4e93-b35d-d9b573024abf
    internal-label: REST APIs
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 4768ecb20d4d9c70452ae084256928261f3a80eb
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 27%
---
# API 說明 - 如何在變數中設定存取權杖

了解如何設定 Postman 應用程式並利用變數將資料儲存到變數中以便重複使用。 也會瞭解如何進行第一個Marketo Engage REST API呼叫以取得存取權杖。

>[!PREREQUISITES]
>
>在開始播放此影片之前，請先以AOI角色建立僅API使用者名稱，並建立Launchpad服務。 請依照下列文章中的步驟操作：
>
>* [建立僅限API的使用者角色](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user-role){target="_blank"}
>
>* [建立僅限API的使用者](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user){target="_blank"}
>
>* [建立自訂服務以搭配REST API使用](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api){target="_blank"}

此影片中使用的&#x200B;**參考：**

* Marketo驗證端點： `{{{}base_url{}}}/identity/oauth/token?grant_type=client_credentials&client_id={{{}client_id{}}}&client_secret={{{}client_secret{}}}`

* 用於從回應內文中抓取access_token的JS指令碼（放置在指令碼：標籤下方）：

```
var jsonData = pm.response.json();
pm.environment.set("access_token", jsonData.access_token);
```

* [Marketo Engage開發人員檔案](https://experienceleague.adobe.com/zh-hant/docs/marketo-developer/marketo/rest/authentication){target="_blank"}

>[!VIDEO](https://video.tv.adobe.com/v/3453994/?captions=chi_hant&learn=on)
