---
title: 記錄CRM同步錯誤，以輕鬆進行疑難排解
description: 瞭解如何使用CRM同步處理錯誤的記錄來調查CRM同步處理問題，並讓它持續順暢地執行。
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
exl-id: 3b7e6127-28fd-4dce-915d-5af9bcce984b
source-git-commit: 681d390ce5ab336a7e24cc63256659a492288517
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 記錄CRM同步錯誤，以輕鬆進行疑難排解

身為Marketo Engage管理員，檢查執行個體是否與CRM同步應該是您[每日常式](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}的關鍵部分。 雖然[通知區段](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html?lang=zh-Hant){target="_blank"} (在Marketo Engage介面的右上角找到)是您開始尋找和調查頻繁同步問題的地方，但有一個專業秘訣可幫助您以有條理的方式管理執行個體的健康狀況。 AdobeMarketo Champion (2019-2022)，Amy Goldfine建議管理員使用者保留CRM同步錯誤的記錄，以便更輕鬆進行疑難排解。

![同步處理錯誤索引標籤的熒幕擷圖](/help/tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## 為什麼要保留CRM同步處理錯誤的記錄？

透過記錄CRM同步錯誤，Marketo Engage管理員可以與CRM管理員一起檢閱問題和趨勢，以修正根本原因。 請依照下列步驟，記錄您執行個體的CRM同步問題。

## 如何保留CRM同步處理錯誤的記錄

開始之前，請先下載[CRM同步錯誤記錄檔範本](/help/tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx)。

**步驟1：**&#x200B;移至Marketo Engage中的&#x200B;*[!UICONTROL 管理員]區段*。 在「*[!UICONTROL 整合]*」下，根據您使用的[!DNL CRM]，按一下「*[!DNL Salesforce]*」、「*[!DNL Microsoft Dynamics]*」或「*[!DNL Veeva]*」，然後按一下「*[!UICONTROL 同步錯誤]*」索引標籤。

**步驟2：**&#x200B;您可以透過[!UICONTROL 篩選器]面板[&#128279;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html?lang=zh-Hant#filter-sync-errors){target="_blank"}，選擇將錯誤的記錄匯出為 [!DNL CSV] 檔案。 如果您只有幾個小時，直接從&#x200B;*[!UICONTROL 同步處理錯誤]*&#x200B;索引標籤複製並貼上會是很好的方法。

**步驟3：**&#x200B;記下發生錯誤的日期。

**步驟4：**&#x200B;輸入受該錯誤影響的人員記錄數目。 (有時您的CRM只會擲回一個人的錯誤。 有時會有許多人同時發生相同錯誤。)

**步驟5：**&#x200B;記下受錯誤影響之個人的電子郵件地址。 這可讓您輕鬆參考並與CRM管理員討論錯誤。

**步驟6：**&#x200B;將連結貼到該人員的[!DNL Marketo Engage]和[!UICONTROL CRM銷售機會/連絡人]記錄中的人員記錄。

**步驟7：**&#x200B;在最後一欄，貼上錯誤的實際文字。

## 接下來呢？

**識別錯誤碼：**&#x200B;若要瞭解錯誤碼，請查閱開發人員檔案[回應層級錯誤碼表格](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"}中的說明，並尋找解決錯誤的典型後續步驟。

## 作者

**Amy Goldfine**\
AdobeMarketo王(2019-2022)
*創始人， MarketingOpsAdvice.com*

![Amy Goldfine](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**趙子楣**
*Adobe的採用與保留行銷經理*

![趙子楣](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
