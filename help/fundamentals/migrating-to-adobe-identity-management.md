---
title: 移轉至Adobe Identity Management
description: 本教學課程將協助您將Marketo Engage訂閱和使用者移轉至Adobe Admin Console。
role: Admin
level: Intermediate, Experienced
recommendations: noDisplay, noCatalog
last-substantial-update: 2024-07-26T00:00:00Z
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: dcfffa299cbcfef489f5b618fae29f745b878d26
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# 移轉至Adobe Identity Management

Adobe正改善您管理Adobe Marketo Engage訂閱和使用者的方式。 我們將您的Marketo Engage訂閱和使用者移轉至Adobe Admin Console，為您的組織帶來更高的生產力。

本教學課程將協助您導覽移轉，讓您能夠在一個集中的位置開始為使用者管理Adobe Marketo Engage及其他Adobe帳戶和產品。 移轉是必要的，且不會影響您的行銷工作流程、內容、整合或資產。

## Marketo Engage管理員的移轉前檢查清單 {#pre-migration-checklist-for-marketo-engage-administrators}

為確保您的組織能夠將Adobe Marketo Engage移轉至Adobe Admin Console，我們建議您遵循下列檢查清單以管理即將進行的變更。

### 1.識別您的系統管理員和IT團隊，並討論他們可能需要採取的行動 {#identify-your-system-administrators}

* 如果您不確定組織中的哪些系統管理員，請聯絡您的Adobe帳戶團隊，或聯絡Adobe支援`marketocares@marketo.com`。

* 確認您的Marketo Engage訂閱將移轉至的Adobe Admin Console (或Adobe組織)。 您可能有適用於[Dynamic Chat](/help/dynamic-chat/dynamic-chat-overview.md){target="_blank"}的Adobe Admin Console，這是Marketo Engage中的原生交談自動化工具。 Marketo Engage訂閱必須部署在與Dynamic Chat相同的組織中。

* 請與您的IT團隊合作，將所有Adobe網域加入允許清單（列於本文頂端[） ](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"}，以防止移轉至Adobe身分識別後Marketo Engage存取中斷。

* **選擇性：** [在使用者移轉前實作單一登入(SSO)](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete){target="_blank"}。

  >[!NOTE]
  >
  >Marketo Engage支援的SSO與Adobe Admin Console SSO之間有所差異。 因此，您可能需要實作組態的變更。

* **選擇性：**&#x200B;在使用者移轉之前，自訂[想要的最長工作階段存留期](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}，讓Marketo Engage使用者保持驗證狀態。

* 在[範例電子郵件區段](#announce-the-migration-timeline)中瞭解如何與您的系統管理員通訊。

### 2.熟悉移轉至Adobe Identity的變更與影響 {#familiarize-yourself-with-the-changes}

在以下影片中，Marketo Engage產品管理團隊會逐步引導您瞭解移轉歷程和期望。

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?t=170/?quality=12&learn=on){transcript=true}

若需Marketo Engage管理員有關此主題的更多說明，請參閱下列說明文章：

* [使用者設定檢查清單](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Adobe Identity Management概觀](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [瞭解Marketo訂閱和使用者移轉至Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [使用移轉主控台移轉至Adobe Identity](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [瞭解如何使用Adobe Admin Console](https://helpx.adobe.com/tw/enterprise/using/admin-console.html){target="_blank"}

### 3.宣佈內部團隊所需的移轉時間表及準備工作 {#announce-the-migration-timeline}

* 在排程後，在您的Marketo Engage管理員和使用者的行事曆上標示移轉日期。

   * 您可以在&#x200B;**管理員** > **移轉主控台** > **預先移轉**&#x200B;中修改移轉日期，以更符合您的內部時間表。 深入瞭解重新排程及[修改移轉日期](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}的限制。

* **傳送電子郵件給您的系統管理員**

以下是傳送給管理員的範例電子郵件。 通常您的IT部門會管理您所有的Adobe授權。

+++ 傳送給系統管理員的範例電子郵件

**主旨：需要支援 — 將Marketo Engage訂閱移轉到Adobe Admin Console**

親愛的`[IT Administrator/NAME]`：

我們的Marketo Engage訂閱即將移轉至Adobe Identity Management系統。 `[Marketing Operation team]`需要您的協助，以在開始移轉使用者前完成一些必要的步驟，將對Marketo Engage使用者的影響降至最低。

`1.`確認組織是否已在Adobe Admin Console中管理其他Adobe產品，以及Marketo Engage是否會移轉至相同主控台。

* Marketo Engage訂閱必須與Dynamic Chat位於相同的組織中，這是與Marketo Engage整合的原生交談自動化工具。

* 如果您對Admin Console有任何疑問，請聯絡Adobe支援： `marketocares@marketo.com`並抄送我們。

`2.`留意來自Adobe且主旨列為「管理Adobe Marketo Engage `[Package Tier]`的使用者存取權所需的動作」的電子郵件。 已在Admin Console上布建Marketo Engage授權後傳送此電子郵件。 只有系統管理員會收到這封電子郵件。 收到請立即通知我們。

* Adobe可能會向Admin Console的系統管理員您尋求同意，以自動將使用者移轉至我們組織的現有主控台。 在主題為「管理使用者對Adobe Marketo Engage `[Package Tier]`的存取權所需的動作」的電子郵件中，按一下「開始使用」按鈕以導覽至同意頁面。

`3.`移轉之後，Marketo Engage會從experience.adobe.com傳送至Adobe Experience Cloud。 請將所有Adobe網域加入允許清單，將[列於本文頂端](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"}，以防止我們的Marketo Engage存取中斷。

`4.` **選用：**&#x200B;在Adobe Admin Console中設定SSO （單一登入）。

* 為了協助使用SSO登入Adobe身分的使用者日後能順利使用SSO，請在使用者移轉前協助Adobe Admin Console設定SSO。

`5.` **選用：**&#x200B;在Adobe Admin Console中設定較長的[工作階段存留期上限](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}。

* 為避免使用者必須經常登入，請在「進階設定」中使用更長的持續時間來自訂工作階段存留期。

感謝您在此轉換過程中的合作。 完成上述步驟後請通知我，以便我繼續進行移轉。

祝順心，

`[Your Name]`

+++

* **傳送電子郵件給Marketo Engage使用者**

以下是範例電子郵件，適用於&#x200B;**不**&#x200B;擁有管理員許可權的Marketo Engage使用者。

+++ 宣告即將進行移轉的電子郵件範例

**主旨：重要更新 — 將Marketo Engage訂閱移轉到Adobe Admin Console**

親愛的Marketo Engage使用者：

我們有一份有關我們Marketo Engage執行個體以及如何登入的重要公告。 Adobe正在將Marketo Engage訂閱和使用者移至Adobe Admin Console，以便我們將其所有產品管理集中在一個位置。 這不會影響行銷工作流程、內容、整合或資產。

**金鑰詳細資料：**

* **移轉日期**： `[Specify the scheduled date - please find this in Marketo Engage under Admin > Migration Console > Pre-migration]`

* **計時**：移轉從我們訂閱的當地時間午夜左右開始。

* **影響**：使用者移轉期間不會遺失產品存取權。 如果您在帳戶移轉時登入，系統會在您登出後於數分鐘內提示您在移轉後使用Adobe身分識別重新登入。

* **優點**：使用單一Marketo Engage身分識別(Adobe ID或Adobe Federated ID (SSO))，驗證Adobe和其他Adobe產品。

**您需要執行的動作：**

`1.` **準備**：您必須進行電子郵件驗證，才能移轉至Adobe身分識別。

i.您已收到包含連結的電子郵件驗證要求電子郵件（3天有效）。 如果您的連結已過期，您可以按一下「我的設定檔」圖示，然後導覽至&#x200B;**我的帳戶** > **帳戶設定** > **重新傳送驗證**，從Marketo Engage中重新傳送驗證電子郵件。

二、 電子郵件驗證成功需要有效的使用者工作階段。 請先使用身分提供者(IdP) URL登入您的Marketo Engage訂閱。

`2.` **上線**：您的使用者帳戶移轉後，您將會收到Adobe的電子郵件，說明登入方法變更。

i.按一下「接受邀請」按鈕並使用Adobe身分登入以接受新的邀請。

二、 在Adobe登入頁面上，請使用現有的Adobe ID登入。

三、 您必須先登入Marketo Engage執行個體，才能在您要導覽的engage-xx.marketo.com網域上使用先前已建立書籤的URL。

`3.` **連絡人**：若您在帳戶移轉後有任何問題或需要協助，或帳戶尚未移轉且無法存取Marketo Engage，請連絡Marketo Engage移轉團隊，地址為`[your internal contact email/phone]`。

感謝您在此轉換過程中的合作。 感謝您對確保系統安全的理解與承諾。

祝順心，

`[Your Name]`

+++
