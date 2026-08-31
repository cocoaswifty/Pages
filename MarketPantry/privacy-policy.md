---
layout: default
title: MarketPantry Privacy Policy
permalink: /MarketPantry/privacy-policy/
---

# MarketPantry Privacy Policy

Effective date: August 31, 2026

MarketPantry is an unofficial iOS client for browsing and participating in PTT. It is not operated, sponsored, endorsed, or owned by PTT. PTT names, content, and services belong to and are operated by their respective owners.

This policy explains what MarketPantry stores on your device, what its supporting services process, and which third parties receive data when you use particular features.

## Information Stored on Your Device

MarketPantry may store the following information locally:

- App settings, notification preferences, blacklists, whitelists, drafts, and saved-image URL metadata
- Your PTT account name and, if you choose to save it, your PTT password
- Optional image-host credentials that you enter
- Market-sentiment records derived from public PTT content, retained for up to 48 hours
- A random installation identifier and an App Attest key identifier used to secure remote-notification registration

Passwords, image-host credentials, the installation identifier, and the App Attest key identifier are stored using Apple Keychain where applicable. Preferences and lists are stored using Apple UserDefaults. Market-sentiment files are stored in the app's Application Support directory with iOS data protection. Author identifiers in local sentiment records are salted and hashed.

## PTT Account and Content

When you sign in, your credentials are sent directly from the app to PTT for authentication. MarketPantry's notification and sentiment server does not receive your PTT username or password.

PTT handles the accounts, articles, comments, replies, and other content that you read or submit. Your activity is subject to PTT's own rules, moderation, availability, and data practices.

MarketPantry also operates a background sentiment service that reads public discussion from the PTT Stock board using a separate service account. It stores public comment text, timestamps, and pseudonymized author identifiers for up to 30 days to calculate sentiment and detect alert conditions. Numeric minute-level sentiment features and generated alert records may be retained for up to 365 days for quality evaluation. This collection is not linked to your MarketPantry installation or PTT login.

## Remote Notifications and App Attest

Remote notifications are optional. If you enable them, MarketPantry sends the following data to its notification server:

- A random per-installation identifier
- Your APNs device token and whether it belongs to the sandbox or production environment
- Your App Attest key identifier, public key, security counter, and attestation or assertion data
- Registration status and limited push-delivery records, such as delivery time, APNs status code, and failure category

MarketPantry uses this information only to verify that requests come from a genuine app installation, register the device with Apple Push Notification service (APNs), prevent replay or device-ownership attacks, deliver requested sentiment alerts, and diagnose delivery failures. The server does not use the App Attest data to identify your PTT account.

Single-use App Attest challenges expire after about five minutes. An active push registration is retained while notifications remain enabled. After you disable notifications, inactive registration data, unused App Attest key records, and push-delivery logs are deleted after no more than 30 days. If APNs reports that an app installation is no longer registered, the same inactive-data schedule applies.

Disabling the notification switch asks the server to deactivate that installation. Removing the app without first disabling notifications may not immediately notify the server; APNs invalidation and the retention process described above are then used to remove inactive data.

Apple processes App Attest and APNs data under Apple's own privacy terms.

## Photos, Image Hosting, and On-Device Analysis

MarketPantry accesses a photo only after you choose it for an upload or saved-image feature.

- ImgBB and Catbox uploads are sent to the selected provider.
- Imgur uploads pass through a MarketPantry-operated upload relay and are then sent to Imgur.

The selected image, file metadata needed for the upload, and standard network information such as IP address may be processed by the relevant service. The resulting hosted image is subject to the image host's retention and privacy practices.

Saved-image text recognition and classification use Apple's Vision framework on your device. MarketPantry does not send those analysis results to its notification or sentiment server.

## Other Network Data and Third Parties

Depending on the features you use, MarketPantry may contact:

- PTT, for account authentication, boards, articles, comments, posts, and replies
- Apple App Attest and APNs, for app-integrity verification and remote notifications
- MarketPantry's sentiment, notification, and Imgur-relay services
- ImgBB, Imgur, or Catbox, when you choose to upload an image
- External websites that you choose to open from PTT content

These services and normal network infrastructure may process standard connection data such as IP address, request time, device or protocol information, and abuse-prevention signals. Their processing is governed by their own terms and privacy policies.

## User-Generated Content and Local Filtering

PTT contains user-generated content supplied by PTT users. PTT, not MarketPantry, operates and moderates that platform.

MarketPantry's blacklist and whitelist features only change how content is presented on your device. They do not delete, report, edit, or otherwise alter content on PTT. Objectionable or unlawful content should be handled through PTT's own rules and reporting or moderation mechanisms where available.

## What MarketPantry Does Not Do

MarketPantry does not:

- Sell personal data
- Use advertising or third-party analytics SDKs
- Track you across apps or websites
- Send your PTT password to MarketPantry's supporting servers
- Use notification identifiers for advertising or profiling
- Access your contacts, microphone, camera, or precise location

## Security

MarketPantry uses transport encryption, Apple App Attest, single-use challenges, assertion counters, device-ownership checks, iOS Keychain, and limited data retention to protect relevant information. No system can guarantee absolute security, but access is limited to what is needed to operate and secure the described features.

## Your Choices and Data Requests

You can decline photo selection, avoid third-party image uploads, choose not to save credentials, and keep remote notifications disabled. You can disable remote notifications in the app to deactivate the server registration.

For questions or requests concerning MarketPantry-operated server data, including deletion requests that cannot be completed through the app, contact:

cocoaswifty@gmail.com

## App Store Privacy Disclosure

MarketPantry's privacy manifest and App Store disclosures identify data categories used for app functionality, such as User ID, Other User Content, Photos or Videos, Device ID, and Other Diagnostic Data where applicable. MarketPantry does not use these categories for tracking or advertising. Data processed only on your device, such as local Vision analysis, is not collected by MarketPantry.

## Changes to This Policy

This policy may be updated when MarketPantry changes its features, data practices, service providers, or legal obligations. Updates will be posted on this page with a revised effective date.

---

# MarketPantry 隱私權政策

生效日期：2026 年 8 月 31 日

MarketPantry 是用來瀏覽與參與 PTT 的非官方 iOS 用戶端，並非由 PTT 營運、贊助、背書或持有。PTT 的名稱、內容與服務屬於並由其各自權利人營運。

本政策說明 MarketPantry 在裝置上儲存哪些資料、支援服務會處理哪些資料，以及你使用特定功能時哪些第三方會收到資料。

## 儲存在裝置上的資料

MarketPantry 可能在裝置本機保存：

- App 設定、通知偏好、黑白名單、草稿及收藏圖片網址中繼資料
- PTT 帳號名稱，以及你選擇保存的 PTT 密碼
- 你輸入的選用圖片託管服務憑證
- 由公開 PTT 內容產生、最多保留 48 小時的市場情緒資料
- 用於保護遠端通知註冊的隨機安裝識別碼與 App Attest key ID

密碼、圖片託管憑證、安裝識別碼及 App Attest key ID 會視用途使用 Apple Keychain 儲存；偏好與清單使用 Apple UserDefaults；市場情緒檔案存放在 App 的 Application Support 目錄並使用 iOS 資料保護。本機情緒資料中的作者識別資訊會先加鹽雜湊。

## PTT 帳號與內容

登入時，帳號密碼會由 App 直接傳送給 PTT 驗證。MarketPantry 的通知與情緒伺服器不會收到你的 PTT 帳號或密碼。

你閱讀或提交的文章、推文、回覆與其他內容由 PTT 處理，並受 PTT 自身規則、審核、服務可用性及資料政策約束。

MarketPantry 另有背景情緒服務，使用獨立服務帳號讀取 PTT Stock 看板的公開討論。為計算情緒與判斷通知條件，伺服器會保存公開推文內容、時間及假名化的作者識別碼，最長 30 天；每分鐘數值型情緒特徵與產生的警報紀錄可保留最長 365 天，用於品質評估。這些公開討論資料不會連結到你的 MarketPantry 安裝或 PTT 登入。

## 遠端通知與 App Attest

遠端通知是選用功能。啟用後，MarketPantry 會將以下資料傳送至通知伺服器：

- 每次安裝隨機產生的識別碼
- APNs device token，以及 sandbox 或 production 環境資訊
- App Attest key ID、公鑰、安全 counter、attestation 或 assertion 資料
- 註冊狀態及有限的推播傳送紀錄，例如時間、APNs 狀態碼與失敗類別

這些資料只用於確認請求來自正版 App 安裝、向 Apple Push Notification service（APNs）註冊裝置、防止重播或裝置所有權攻擊、傳送你要求的情緒通知，以及診斷傳送失敗。伺服器不會使用 App Attest 資料辨識你的 PTT 帳號。

一次性 App Attest challenge 約五分鐘後失效。通知保持啟用期間，伺服器會保留有效註冊；關閉通知後，已停用的註冊資料、未再使用的 App Attest key 紀錄與推播傳送 log 會在最長 30 天後刪除。若 APNs 回報該安裝已失效，也適用相同的停用資料保留期限。

關閉通知開關時，App 會要求伺服器停用該安裝。若未先關閉通知就移除 App，伺服器可能無法立刻得知；此時會依 APNs 失效回報及上述保留流程移除停用資料。

Apple 會依其自身隱私條款處理 App Attest 與 APNs 資料。

## 照片、圖片託管與裝置端分析

只有在你主動選擇圖片進行上傳或使用收藏圖片功能時，MarketPantry 才會存取該圖片。

- ImgBB 與 Catbox 上傳會傳送至你選擇的服務。
- Imgur 上傳會先經過 MarketPantry 營運的上傳中轉服務，再傳送至 Imgur。

所選圖片、上傳必要的檔案中繼資料，以及 IP 位址等標準網路資訊，可能由相關服務處理；上傳後圖片的保存依各圖片託管服務的政策處理。

收藏圖片的文字辨識與分類使用 Apple Vision 在裝置上執行；分析結果不會傳送至 MarketPantry 的通知或情緒伺服器。

## 其他網路資料與第三方

依你使用的功能，MarketPantry 可能連線至：

- PTT：帳號驗證、看板、文章、推文、發文與回覆
- Apple App Attest 與 APNs：App 完整性驗證與遠端通知
- MarketPantry 的情緒、通知及 Imgur 中轉服務
- ImgBB、Imgur 或 Catbox：你選擇上傳圖片時
- 你從 PTT 內容主動開啟的外部網站

上述服務及一般網路基礎設施可能處理 IP 位址、請求時間、裝置或協定資訊及防濫用訊號等標準連線資料；其處理由各服務自身條款與隱私政策規範。

## 使用者產生內容與本機過濾

PTT 包含 PTT 使用者產生的內容，平台由 PTT 營運與審核。MarketPantry 的黑名單與白名單只改變內容在你裝置上的呈現，不會刪除、檢舉、修改或影響 PTT 上的內容。不當或違法內容應依 PTT 自身規則與其提供的處理機制處理。

## MarketPantry 不會進行的行為

MarketPantry 不會：

- 出售個人資料
- 使用廣告或第三方分析 SDK
- 進行跨 App 或網站追蹤
- 將你的 PTT 密碼傳送至 MarketPantry 支援伺服器
- 將通知識別資訊用於廣告或建立使用者輪廓
- 存取聯絡人、麥克風、相機或精確位置

## 安全措施

MarketPantry 使用傳輸加密、Apple App Attest、一次性 challenge、assertion counter、裝置所有權檢查、iOS Keychain 與有限資料保留等措施保護相關資料。任何系統都無法保證絕對安全，但資料存取會限制在營運及保護上述功能所需的範圍。

## 你的選擇與資料請求

你可以不選擇照片、不使用第三方圖片上傳、不保存憑證，並保持遠端通知關閉。你可以在 App 內關閉遠端通知，停用伺服器上的註冊。

若對 MarketPantry 營運的伺服器資料有疑問，或有無法透過 App 完成的刪除請求，請聯絡：

cocoaswifty@gmail.com

## App Store 隱私揭露

MarketPantry 的 privacy manifest 與 App Store 隱私揭露會依適用情況列出用於 App 功能的資料類別，例如 User ID、Other User Content、Photos or Videos、Device ID 及 Other Diagnostic Data。MarketPantry 不會將這些資料用於追蹤或廣告。僅在裝置上處理的資料（例如本機 Vision 分析）不會由 MarketPantry 收集。

## 政策更新

若 MarketPantry 的功能、資料處理方式、服務供應者或法律義務變更，本政策可能更新，並會在本頁標示新的生效日期。
