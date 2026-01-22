---
title: 遷移至 Adobe Identity Management
description: 本教學課程將協助您將 Marketo Engage 訂閱和使用者遷移至 Adobe Admin Console。
role: Admin
level: Intermediate, Experienced
recommendations: noDisplay, noCatalog
last-substantial-update: 2024-07-26T00:00:00Z
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: dcfffa299cbcfef489f5b618fae29f745b878d26
workflow-type: ht
source-wordcount: '1250'
ht-degree: 100%

---

# 遷移至 Adobe Identity Management

Adobe 正在改善管理 Adobe Marketo Engage 訂閱和使用者的方式。我們將您的 Adobe Marketo Engage 訂閱和使用者遷移至 Adobe Admin Console，為您的組織提供更高的生產力。

本教學課程將協助您完成遷移流程，讓您能夠在中央的位置開始為使用者管理 Adobe Marketo Engage 及其他 Adobe 帳戶和產品。遷移有其必要性，並且不會影響您的行銷工作流程、內容、整合或資產。

## Adobe Marketo Engage 管理員的遷移前檢查清單 {#pre-migration-checklist-for-marketo-engage-administrators}

為了確保您的組織能夠將 Adobe Marketo Engage 遷移至 Adobe Admin Console，我們建議您遵循下列檢查清單，以便管理即將進行的變更。

### &#x200B;1. 確認您的系統管理員和 IT 團隊，並討論他們可能需要採取哪些行動 {#identify-your-system-administrators}

* 如果您不確定組織中的系統管理員是誰，請聯絡您的 Adobe 帳戶團隊，或聯絡 Adobe 支援`marketocares@marketo.com`。

* 確認您的 Adobe Marketo Engage 訂閱將遷移至哪個 Adobe Admin Console (或 Adobe 組織)。您可能具備適用於 [Dynamic Chat](/help/dynamic-chat/dynamic-chat-overview.md){target="_blank"} 的 Adobe Admin Console，這是 Adobe Marketo Engage 中的原生交談自動化工具。Adobe Marketo Engage 訂閱必須與 Dynamic Chat 部署在同一個組織中。

* 請與您的 IT 團隊合作，將[列於本文頂端](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"}的所有 Adobe 網域加入允許清單，以防止遷移至 Adobe Identity 後中斷 Adobe Marketo Engage 存取。

* **選用：** [在使用者遷移前實施單一登入 (SSO)](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete){target="_blank"}。

  >[!NOTE]
  >
  >Adobe Marketo Engage 支援的 SSO 與 Adobe Admin Console SSO 之間有所差異。因此，您可能需要實施設定的變更。

* **選用：**&#x200B;在使用者遷移前，自訂讓 Adobe Marketo Engage 使用者保持登入狀態的[最長工作階段時限](https://helpx.adobe.com/tw/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}。

* 請參閱[範例電子郵件區段](#announce-the-migration-timeline)，了解如何與您的系統管理員溝通。

### &#x200B;2. 熟悉遷移至 Adobe Identity 的變更與影響 {#familiarize-yourself-with-the-changes}

在下列影片中，Adobe Marketo Engage 產品管理團隊會為您逐步示範遷移歷程和預期情況。

>[!VIDEO](https://video.tv.adobe.com/v/3432367/?captions=chi_hant&t=170/?quality=12&learn=on){transcript=true}

如需此主題有關 Adobe Marketo Engage 管理員的詳細說明，請參閱下列說明文章：

* [使用者設定檢查清單](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Adobe Identity Management 概觀](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [了解 Marketo 訂閱和使用者移轉至 Adobe Admin Console](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [透過遷移主控台移轉至 Adobe Identity](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [了解如何使用 Adobe Admin Console](https://helpx.adobe.com/tw/enterprise/using/admin-console.html){target="_blank"}

### &#x200B;3. 向內部團隊公告遷移時間表及所需的準備工作 {#announce-the-migration-timeline}

* 排程後，在您的 Adobe Marketo Engage 管理員和使用者的行事曆上標示遷移日期。

   * 您可以在&#x200B;**「管理員」**>**「遷移主控台」**>**「遷移前」**&#x200B;中修改遷移日期，以便配合您內部的時間表。進一步瞭解重新排程及[修改遷移日期](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}的限制。

* **寄送電子郵件給您的系統管理員**

以下是寄送給管理員的範例電子郵件。一般來說，您的 IT 部門會管理您所有的 Adobe 授權。

+++ 寄送給系統管理員的電子郵件範例

**主旨：需要支援 — 將 Adobe Marketo Engage 訂閱遷移至 Adobe Admin Console**

`[IT Administrator/NAME]` 您好：

我們的 Adobe Marketo Engage 訂閱即將遷移至 Adobe 身分管理系統。`[Marketing Operation team]`需要您的協助，以便在開始遷移使用者之前先完成一些必要步驟，以便盡量減少對 Adobe Marketo Engage 使用者的影響。

`1.`請確認組織是否已在 Adobe Admin Console 中管理其他 Adobe 產品，以及 Adobe Marketo Engage 是否將遷移至相同的主控台。

* Adobe Marketo Engage 訂閱必須位於與 Dynamic Chat 相同的組織中，這是與 Adobe Marketo Engage 整合的原生交談自動化工具。

* 如果您對 Admin Console 有任何疑問，請聯絡 Adobe 支援 (`marketocares@marketo.com`)，並將副本寄送給我們。

`2.`請留意來自 Adobe 的電子郵件，主旨為「須採取動作來管理 Adobe Marketo Engage `[Package Tier]` 的使用者存取權」。此電子郵件於 Adobe Marketo Engage 授權已佈建至我們的 Admin Console 後寄送。只有系統管理員會收到此電子郵件。請於收到後立即通知我們。

* Adobe 可能會徵求您 (Admin Console 系統管理員) 的同意，以便將使用者自動遷移至我們組織的現有主控台。在主旨為「須採取動作來管理 Adobe Marketo Engage `[Package Tier]` 使用者存取權」的電子郵件中，按一下「開始使用」按鈕以導覽至同意頁面。

`3.`遷移完成後，Adobe Marketo Engage 的服務位置會由 experience.adobe.com 遷移至 Adobe Experience Cloud。請將所有 Adobe 網域 ([列於本文頂端](https://experienceleague.adobe.com/zh-hant/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"}) 加入允許清單，以避免中斷 Adobe Marketo Engage 存取。

`4.` **選用：**&#x200B;在 Adobe Admin Console 中設定 SSO (單一登入)。

* 為了協助日後使用 SSO 登入其 Adobe Identity 的使用者能順利使用，請在遷移使用者前協助完成 Adobe Admin Console 的 SSO 設定。

`5.` **選用：**&#x200B;在 Adobe Admin Console 中設定較長的[最大工作階段時限](https://helpx.adobe.com/tw/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}。

* 為避免使用者經常需要登入，請在「進階設定」中將工作階段時限自訂為較長的持續時間。

感謝您在此轉變過程中的合作。當您完成上述步驟後請通知我，以便繼續進行遷移。

謹致

`[Your Name]`

+++

* **寄送電子郵件給 Adobe Marketo Engage 使用者**

以下為範例電子郵件，適用於&#x200B;**沒有**&#x200B;管理員權限的 Adobe Marketo Engage 使用者。

+++ 公告即將進行遷移的範例電子郵件

**主旨：重要更新 — 將 Adobe Marketo Engage 訂閱遷移至 Adobe Admin Console**

Adobe Marketo Engage 的使用者您好：

有一則關於我們的 Adobe Marketo Engage 執行個體以及您將如何登入的重要公告。Adobe 正將 Adobe Marketo Engage 訂閱和使用者遷移至 Adobe Admin Console，以便我們將其所有產品管理集中於同一個位置。這不會影響行銷工作流程、內容、整合或資產。

**重要詳細資料：**

* **遷移日期**：`[Specify the scheduled date - please find this in Marketo Engage under Admin > Migration Console > Pre-migration]`

* **時間**：我們的訂閱大約於當地時間午夜開始進行遷移。

* **影響**：使用者遷移期間，不會喪失產品存取權。若您在帳戶遷移期間已登入，系統會在遷移完成後的數分鐘內將您登出，並提示使用 Adobe Identity 重新登入。

* **優點**：使用單一 Adobe 身分識別，Adobe ID 或 Federated ID (SSO) 皆可，即可驗證 Adobe Marketo Engage 和其他 Adobe 產品。

**您需要執行的動作：**

`1.` **準備**：您必須進行電子郵件驗證，才能遷移至 Adobe Identity。

i. 您已收到「電子郵件驗證請求」的電子郵件，其中包含一個連結 (有效期限為 3 天)。如果您的連結已過期，您可以從 Adobe Marketo Engage 中重新寄送驗證電子郵件，請按一下「我的設定檔」圖示，然後導覽至&#x200B;**「我的帳戶」**>**「帳戶設定」**>**「重新寄送驗證」**。

ii. 使用者工作階段必須是有效狀態，才能成功完成電子郵件驗證。請先使用身分識別提供者 (IdP) URL 登入您的 Adobe Marketo Engage 訂閱。

`2.` **上線**：您的使用者帳戶遷移完成後，您將會收到來自 Adobe 的電子郵件，說明登入方法的變更。

i. 按一下「接受邀請」按鈕，並使用 Adobe Identity 登入，以便接受新的邀請。

ii. 在 Adobe 登入頁面上，請使用現有的 Adobe ID 登入。

iii. 您必須先登入 Adobe Marketo Engage 執行個體，才能導覽至先前在 engage-xx.marketo.com 網域上已建立書籤的任何 URL。

`3.` **聯絡方式**：若您在帳戶遷移完成後有任何疑問或需要協助，或您的帳戶尚未遷移但您無法存取 Adobe Marketo Engage，請聯絡 Adobe Marketo Engage 遷移團隊，電子郵件地址為：`[your internal contact email/phone]`。

感謝您在此轉變過程中的合作。感謝您理解並致力於確保我們系統的安全。

謹致

`[Your Name]`

+++
