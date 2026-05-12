---
title: 使用檔案開發執行個體治理指南
description: 瞭解如何建立強大的程式，用於建立和維護您的Marketo Engage執行個體的檔案和變更記錄。 這不僅可節省團隊分享知識的時間，也可提升執行個體的健全度和效率。
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00.000Z
jira: KT-14103
thumbnail: KT-14103.jpeg
index: true
exl-id: 4313b54a-1848-4684-b037-7a7795dd01ec
TQID: https://experienceleague.adobe.com/t1TtyyanSwdY8cE3hEkLLOqIW2GpEvFUS1I4LGpUnKM
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0f8ea3988fd586ccbd4b414b3558f6e5f36882bf
workflow-type: tm+mt
source-wordcount: 959
ht-degree: 1%

---

# 使用檔案開發執行個體治理指南

當您進入舊版[!DNL Marketo Engage]執行個體時，經常會面臨缺乏最新功能與技術檔案的挑戰。 身為管理員，建立准則以確保適當的執行個體治理是您不可忽視的核心責任。 在您於已建立的Marketo Engage執行個體中工作時，[提高效率是重要策略之一](https://nation.marketo.com/t5/champion-program-blogs/3-tips-to-increase-your-efficiency-in-an-inherited-instance/ba-p/247582)。

此逐步教學課程來源為[!DNL Adobe Marketo Champion] (2018) Nick Hajdin，將引導您完成此程式，概述您的執行個體設定、記錄您的主要作業計畫，並維護[!DNL changelog]以強制執行嚴格的治理政策。

## 為何要為繼承的執行個體開發執行個體治理指南和檔案？

詳細檔案和[!DNL changelog]對於有效管理您的[!DNL Marketo Engage]執行個體並傳授知識而言至關重要。 持續追蹤您在執行個體設定期間所做的變更和決定，有助於您：

1. 以可擴充的方式更輕鬆地訓練內部使用者。
2. 在[!DNL Marketo Engage]中長期更有效地建置。
3. 維持執行個體的健康與衛生，以節省您花費數小時探索電子郵件、[稽核軌跡](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/audit-trail/audit-trail-overview.html)及[活動記錄](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.html)以取得內容的時間。
4. 如果您的團隊遇到任何人員流動，請節省將[!DNL Marketo Engage]知識轉移給新[!DNL Marketo Engage]管理員的時間。

## [!DNL Marketo Engage]治理指南101

治理指南是執行個體設定和系統設計要求的真實來源。 建議納入本檔案的重要資訊包括：

* 方案/資料夾結構
* 使用者和角色許可權
* 通訊限制
* 治理標準
* 授與使用者對平台的存取權之前的內部使用者訓練

## 如何為您的[!DNL Marketo Engage]執行個體開發及維護治理指南

### 步驟1：識別您目前的治理指南和檔案狀態

* **我找不到任何繼承執行個體的檔案：**&#x200B;如果您最近啟動了一個新角色，但找不到任何繼承執行個體的檔案，請&#x200B;**移至步驟2**，開始使用我們提供的可下載範本。
* **我有檔案檔案：**&#x200B;恭喜，這是好兆頭！ 請務必檢閱其相關性，以檢視上次進行變更的時間。 如果您的團隊成員未主動維護更新，建議您重新整理，並教育內部使用者如何使其保持最新狀態。

### 步驟2：識別要包含在您的[!DNL Marketo Engage]檔案與[!DNL Changelogs]中的元素

格式因雲端型平台和共用檔案而異。 您可以設計符合組織需求的格式。 [這裡有簡單的檔案與變更記錄檔Excel範本](/help/tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx)，涵蓋您可以開始使用的重要元素。 這些功能包括：

* 文件
   * 計畫範本名稱
   * 管道
   * 建立日期
   * 建立者
   * 計畫的目的
   * 狀態
   * 方案範本的連結
   * 備註
* Changelog
   * 計畫範本名稱
   * 變更日期
   * 更新者
   * 更新的目的
   * 變更前的體驗（包含連結/熒幕擷取畫面）
   * 變更後的體驗（包含連結/熒幕擷取畫面）
   * 方案的URL

### 步驟3：識別並記錄主要作業程式的目前狀態

首先，找出在訂閱層級具有影響的主要作業方案。 範例包括資料管理行銷活動、銷售機會生命週期、銷售機會評分、[!DNL CRM]同步和傳遞能力。

對於每個已識別的作業方案，記錄其目前狀態。 其中包括有關方案目的、設定、相關智慧行銷活動，以及與其他工具整合（如果適用）的詳細資訊。

### 步驟4：強制[!DNL Changelog]維護

下一步是為您的[!DNL Marketo Engage]執行個體建立嚴格的治理政策，要求「[!DNL Changelog]維護」。 此原則可確保完整記錄整個執行處理中對作業程式所做的任何更新。

教育您的團隊這些檔案的重要性，以及如何正確存取和更新它們。 指派維護變更記錄的責任可能會有所幫助，因此一些指定的行銷作業團隊成員或管理員會一致地記錄變更並提供簽章。

### 步驟5：集中處理檔案

建立中央位置或存放庫，以儲存與您的[!DNL Marketo Engage]執行個體相關的所有檔案。 這可以是共用磁碟機、專用資料夾或雲端系統。

### 步驟6：定期檢閱和更新

排程定期審查您的檔案，以確保它保持準確和最新。 在繁忙的時刻很容易被忽略。 主動設定行事曆上的提醒，以確保您的團隊定期進行更新，以反映作業程式中的任何變更或最佳化。

## 接下來呢？

開始下載此[簡單範本](/help/tutorial-inherited-instance/_assets/downloads/Adobe_Marketo_Engage_Inherited_Instance_Documentation-Changlog.xlsx)。

請依照上述步驟開發您的治理指南和檔案。 處理此程式時，請謹記下列經驗法則：

**更新您現有的檔案：**
讓您的檔案保持在最新狀態非常重要。 如果在過去3年內未修改檔案，請預留時間在稽核執行個體時修訂檔案。

**共用與訓練：**
與相關團隊成員分享您的檔案和[!DNL changelog]，並教育他們如何更新這些記錄。

**定期檢閱：**&#x200B;預先排程整年檢閱和維護時間，以包含任何新變更、最佳化或調整。

維護您的Marketo Engage執行個體全面且最新的檔案，長遠而言可節省您的時間與精力，並可促進有效的執行個體管理。

### 作者

**Nick Hajdin**
[!DNL Adobe Marketo Champion] (2018)
*[!DNL Digital Technology Senior Manager at Accenture]*

![Nick Hajdin](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Nicholas_Hajdin.png){width="30%"}

**趙子楣**
*Adobe採用與保留行銷經理*

![趙子楣](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width=30%}
