---
title: 移轉至AdobeIdentity Management
description: 說明即將推出。
role: User
level: Beginner
hide: true
hidefromtoc: true
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: fe760c2fc53b96d5c176de377730bce2e89dbc74
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 0%

---

# 移轉至AdobeIdentity Management

Adobe可強化您管理Adobe Marketo Engage訂閱和使用者的方式。 我們將您的Marketo Engage訂閱和使用者移轉至Adobe Admin Console，為您和您的組織帶來更高的生產力。

本教學課程可讓您導覽移轉，以便在集中位置管理Adobe Marketo Engage以及使用者的其他Adobe帳戶和產品。 移轉是必要的，且不會影響您的行銷工作流程、內容、整合或資產。

## 給Marketo Engage管理員的移轉前檢查清單 {#pre-migration-checklist-for-marketo-engage-administrators}

為確保您的組織能夠將Adobe Marketo Engage移轉至Adobe Admin Console，我們建議您遵循下列檢查清單來管理即將進行的變更。

### 1.識別您的系統管理員，並討論他們可能需要採取的動作 {#identify-your-system-administrators}

* 如果您不確定組織中的哪些系統管理員，請聯絡您的Adobe帳戶團隊，或聯絡Adobe支援`marketocares@marketo.com`。

* 確認您的Marketo Engage訂閱將移轉至的Adobe Admin Console (或Adobe組織)。  Marketo Engage訂閱必須部署在與Dynamic Chat相同的組織中，這是與Marketo Engage整合的原生交談自動化工具。
  `TBD LINK TO https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete`

* 在[範例電子郵件區段](#announce-the-migration-timeline)中進一步瞭解如何與系統管理員通訊。

### 2.熟悉移轉至「Adobe身分」的變更與影響 {#familiarize-yourself-with-the-changes}

在以下影片中，Marketo Engage產品管理團隊會逐步引導您瞭解移轉歷程和期望。

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?quality=12&learn=on){transcript=true}

在下列說明文章中，可以找到更多適用於Marketo Engage管理員的有關此主題的說明：

* [使用者設定檢查清單](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [AdobeIdentity Management概觀](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [瞭解Marketo訂閱和使用者移轉至Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [使用移轉主控台移轉至Adobe身分識別](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [瞭解如何使用Adobe Admin Console](https://helpx.adobe.com/tw/enterprise/using/admin-console.html){target="_blank"}

### 3.宣佈內部團隊所需的移轉時間表及準備工作 {#announce-the-migration-timeline}

* 在排程後，在您的Marketo Engage管理員和使用者的行事曆上標示移轉日期。

您可以在&#x200B;**管理員** > **移轉主控台** > **移轉前**&#x200B;修改移轉日期，以更符合內部時間表。 深入瞭解重新排程及[修改移轉日期](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}的限制。

* 傳送電子郵件以與系統管理員通訊。

以下是傳送給系統管理員的範例電子郵件。 通常您的IT部門會管理您所有的Adobe授權。

`---------------------------------------------------`

**主旨：需要支援 — 將Marketo Engage訂閱移轉到Adobe Admin Console**

親愛的`[IT Administrator/NAME]`：

我們的Marketo Engage訂閱即將移轉至AdobeIdentity Management系統。 `[Marketing Operation team]`需要您的協助以在使用者移轉開始前完成一些必要的步驟，以將對Marketo Engage使用者的影響降至最低。

`1.`確認組織是否已在Adobe Admin Console中管理其他Adobe產品，以及Marketo Engage是否會移轉至相同主控台。

* 請注意，Marketo Engage訂閱必須與Dynamic Chat位於相同的組織中，這是與Marketo Engage整合的原生交談自動化工具。

* 如果您對將新增Marketo Engage的Admin Console有任何疑慮或疑問，請透過`marketocares@marketo.com`聯絡支援團隊，並將我們加入您的通訊中。

`2.`在Adobe中尋找主旨列為「管理Adobe Marketo Engage `[Package Tier]`的使用者存取權所需的動作」的電子郵件。 已在Admin Console上布建Marketo Engage授權後傳送此電子郵件。 只有系統管理員會收到這封電子郵件。 收到請立即通知我們。

* Adobe可能會向您(身為Admin Console的系統管理員)尋求同意，以自動將使用者移轉至我們組織的現有主控台。 在主題為「管理使用者對Adobe Marketo Engage `[Package Tier]`的存取權所需的動作」的電子郵件中，按一下「開始使用」按鈕以導覽至同意頁面。

`3.` **選用：**&#x200B;在Adobe Admin Console上設定SSO （單一登入）。

* 為了讓我們的使用者能透過SSO登入Adobe識別碼，我們要求您在使用者移轉發生之前，協助Adobe Admin Console設定SSO。
感謝您在此轉換過程中的合作。 完成這些步驟後請通知我，以便我可以繼續使用Marketo Engage進行使用者移轉。
祝順心，

`[Your Name]`

`---------------------------------------------------`

* 傳送電子郵件給Marketo Engage使用者。

以下是範例電子郵件，可用來向沒有管理員許可權的Marketo Engage使用者宣告即將進行的移轉。

`---------------------------------------------------`

**主旨：重要更新 — 將Marketo Engage訂閱移轉到Adobe Admin Console**

親愛的Marketo Engage使用者：

我們有一份有關我們Marketo Engage執行個體以及如何登入的重要公告。 Adobe正在將Marketo Engage訂閱和使用者移至Adobe Admin Console，讓他們的客戶能夠將其所有產品管理集中到一個地方。 這不會影響行銷工作流程、內容、整合或資產。

金鑰詳細資料：

* 移轉日期： [指定排定的日期 — 請在&#x200B;**管理** > **移轉主控台** > **預先移轉**]&#x200B;底下的Marketo Engage中找到此專案

* 時間：移轉從我們訂閱的當地時間午夜開始。

* 影響：使用者移轉期間不會遺失產品存取權。 如果您在移轉帳號時登入，系統會在您登出，並在移轉後幾分鐘內提示您使用Adobe身分識別重新登入。

* 優點：使用單一Adobe身分識別(Adobe ID或AdobeFederated ID(SSO))，驗證Marketo Engage和其他Adobe產品。

您需要執行的動作：

`1.`準備：您必須進行電子郵件驗證，才能移轉至Adobe身分識別。

i.您已收到包含連結的電子郵件驗證要求電子郵件（3天有效）。 如果您的連結已過期，您可以前往&#x200B;**管理員** > **我的帳戶** > **帳戶設定**，然後按一下&#x200B;**重新傳送驗證**，以重新傳送驗證電子郵件。
二、 電子郵件驗證成功需要有效的使用者工作階段。 請先使用您的身分提供者(IdP) URL登入您的Marketo Engage訂閱。

`2.`上線：您的使用者帳戶移轉後，您將會收到Adobe的電子郵件，說明登入方法變更。

i.按一下[接受邀請]按鈕並使用Adobe識別登入以接受新的邀請。
二、 在Adobe登入頁面上，請使用現有的Adobe ID登入。

`3.`連絡人：如果您在帳戶移轉後有任何問題或需要協助，或帳戶尚未移轉且無法存取Marketo Engage，請透過`[your internal contact email/phone]`聯絡Marketo Engage移轉團隊。

感謝您在此轉換過程中的合作。 感謝您對確保系統安全的理解與承諾。

祝您使用愉快，

`[Your Name]`

`---------------------------------------------------`
