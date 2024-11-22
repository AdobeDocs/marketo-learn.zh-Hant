---
title: Marketo如何API影片 — 如何在變數中設定存取權杖
description: 瞭解如何設定Postman應用程式，以及如何運用變數將資料儲存至變數，以利重複使用。
feature: REST API
role: Admin, Developer
level: Advanced
doc-type: Technical Video
duration: 772
last-substantial-update: 2024-08-06T00:00:00Z
jira: KT-15548
exl-id: 4da86ed6-1072-4e0e-a648-16587badaeb3
source-git-commit: a3ef8abe1a0928b4119c334ecb96c7e18d63803d
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 24%

---

# API說明 — 如何在變數中設定存取權杖

了解如何設定 Postman 應用程式並利用變數將資料儲存到變數中以便重複使用。您也會了解如何進行首次 Marketo Engage REST API 呼叫以取得存取權杖。

>[!PREREQUISITES]
>
>在開始播放此影片之前，請先以AOI角色建立僅API使用者名稱，並建立Launchpad服務。 請依照下列文章中的步驟操作：
>
>* [建立僅限API的使用者角色](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user-role){target="_blank"}
>
>* [建立僅限API的使用者](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user){target="_blank"}
>
>* [建立自訂服務以搭配REST API使用](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api){target="_blank"}

此影片中使用的&#x200B;**參考：**

* Marketo驗證端點： `{{{}base_url{}}}/identity/oauth/token?grant_type=client_credentials&client_id={{{}client_id{}}}&client_secret={{{}client_secret{}}}`

* 用於從回應內文中抓取access_token的JS指令碼（放置在指令碼：標籤下方）：

```
var jsonData = pm.response.json();
pm.environment.set("access_token", jsonData.access_token);
```

* [Marketo Engage開發人員檔案](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}

>[!VIDEO](https://video.tv.adobe.com/v/3429275/?learn=on)
