---
layout: default
title: QTap Privacy Policy
permalink: /QTap/privacy-policy/
---

# QTap Privacy Policy

Effective date: September 24, 2026

QTap is an iOS app that receives push notifications sent to channels you create. You can copy a channel's sender URL and use it from your own scripts or tools. This policy explains what QTap stores on your device, what the QTap service processes, and how Apple and Cloudflare support the service.

## Information Stored on Your Device

QTap stores the following information locally:

- A random installation identifier and device credential
- Your channel names, channel identifiers, and sender tokens
- Connection and onboarding state, plus the App Attest key identifier
- Push notifications received by the app, including their title, body, channel, time, and optional link

The installation credential and channel sender tokens are stored together in Apple Keychain. The App Attest key identifier is stored in app preferences. Notification history is stored on your device so you can read it in QTap. Deleting a notification clears its title, body, and link from the inbox; a small identifier remains locally to prevent a repeated push from restoring the deleted item.

## Information Processed by the QTap Service

When you enable notifications and connect QTap, the app sends your random installation identifier, APNs device token, APNs environment, and App Attest verification data to the QTap service at `qtap.761223.xyz`. The service uses this information to verify the app installation and register your device with Apple Push Notification service (APNs).

The service stores the installation identifier, APNs device token and environment, a hash of the device credential, and App Attest information such as the key identifier, public key, receipt, and verification counter. It does not store the device credential in plain text. For each channel, the service stores its identifier and name and a hash of its sender token. It does not store the sender token in plain text.

The service uses these records only to authenticate your app, route messages to the right device, and prevent unauthorized or replayed registration requests. It does not associate an installation with a personal account; QTap has no account or sign-in system.

## Messages and Push Notifications

When a script or tool sends a message using a channel's sender URL, the QTap service processes the message title, body, and optional link in memory and forwards the notification payload to Apple APNs. Apple processes that payload to deliver the notification to your device. QTap does not save message contents in its server database. The app and its notification extension receive the notification and save it on your device as inbox history.

Anyone who has a channel's sender URL can send messages to that channel. Treat the URL as a password: do not post or share it publicly. Deleting a channel in QTap revokes its sender URL and deletes that channel's name and token hash from the QTap service. Push delivery depends on Apple and your network and is not guaranteed.

## Third-Party Services and Network Information

QTap uses:

- **Cloudflare**, to host the QTap API and database and apply request limits. Cloudflare may process IP addresses and standard request metadata to deliver and protect the service. The QTap app database does not store your raw IP address.
- **Apple**, for App Attest verification, APNs registration, and push delivery. Apple processes the device token, app verification data, and notification payload needed for these functions under Apple's own terms and privacy practices.

QTap does not use advertising or analytics SDKs, sell personal information, or track you across apps or websites. QTap does not request access to your contacts, photos, camera, microphone, or location.

## Retention and Your Choices

You can delete a channel in QTap to revoke its sender URL and remove that channel's server record. QTap currently has no in-app control to unregister a device or delete its server-side installation and App Attest records. These registration records do not currently expire automatically. Deleting all channels or removing the app does not itself remove the server-side registration. To request deletion, contact us below and include information that can help us identify the registration, such as your channel name. Do not send a sender URL or credential.

Notification history is stored locally on your device. You can delete individual messages in QTap. Removing the app removes its local message history; iOS may retain Keychain items after an app is removed.

You can decline notification permission or turn notifications off in iOS Settings. Without notification permission, QTap cannot receive push notifications.

## Security

The QTap app connects to its service over HTTPS. Device credentials and channel sender tokens are random, and the service stores their hashes. App Attest helps verify supported app installations. These measures reduce risk but cannot guarantee absolute security.

## Contact and Policy Changes

For support, privacy questions, or a request to delete server-side registration data, contact:

cocoaswifty@gmail.com

This policy may be updated when QTap's features, service providers, or data practices change. Updates will be posted on this page with a revised effective date.

---

# QTap 隱私權政策

生效日期：2026 年 9 月 24 日

QTap 是一款 iOS App，用來接收你建立的頻道所收到的推播通知。你可以複製頻道的發送網址，並從自己的腳本或工具發送訊息。本政策說明 QTap 在裝置上保存哪些資料、QTap 服務如何處理資料，以及 Apple 與 Cloudflare 如何支援服務運作。

## 儲存在裝置上的資料

QTap 會在裝置本機保存：

- 隨機產生的安裝識別碼與裝置憑證
- 頻道名稱、頻道識別碼與發送 token
- 連線及初始設定狀態，以及 App Attest key ID
- App 收到的推播通知，包括標題、內容、頻道、時間及選用連結

安裝憑證與頻道發送 token 會一併存放在 Apple Keychain；App Attest key ID 存在 App 偏好設定中。通知歷史保存在你的裝置上，供你在 QTap 查閱。刪除通知時，App 會清除收件匣中的標題、內容與連結，但會在本機留下少量識別碼，避免重複推播讓已刪除的項目再次出現。

## QTap 服務處理的資料

啟用通知並連線時，App 會將隨機安裝識別碼、APNs 裝置 token、APNs 環境及 App Attest 驗證資料傳送至 `qtap.761223.xyz`。QTap 服務使用這些資料驗證 App 安裝，並向 Apple Push Notification service（APNs）註冊裝置。

服務會保存安裝識別碼、APNs 裝置 token 與環境、裝置憑證的雜湊值，以及 App Attest 資料，例如 key ID、公鑰、receipt 與驗證 counter。服務不會以明文保存裝置憑證。每個頻道會保存識別碼、名稱及發送 token 的雜湊值，不會以明文保存發送 token。

服務僅使用這些資料驗證 App、將訊息送至正確裝置，以及防止未授權或重放的註冊請求。QTap 不會將安裝資料連結至個人帳號；QTap 沒有帳號或登入系統。

## 訊息與推播通知

腳本或工具透過頻道發送網址送出訊息時，QTap 服務會在記憶體中處理訊息標題、內容及選用連結，再將通知 payload 轉送給 Apple APNs。Apple 會處理該 payload 並將通知送至你的裝置。QTap 不會將訊息內容保存至伺服器資料庫。App 與通知擴充功能收到通知後，會將其保存於你的裝置，作為收件匣歷史。

任何取得頻道發送網址的人都能向該頻道發送訊息。請把網址當成密碼，不要公開張貼或分享。你在 QTap 刪除頻道後，該發送網址會失效，QTap 服務也會刪除該頻道的名稱與 token 雜湊值。推播是否送達取決於 Apple 與網路狀況，無法保證。

## 第三方服務與網路資訊

QTap 使用：

- **Cloudflare**：託管 QTap API 與資料庫並套用請求速率限制。Cloudflare 可能為提供與保護服務而處理 IP 位址及一般請求中繼資料；QTap App 資料庫不會保存你的原始 IP 位址。
- **Apple**：提供 App Attest 驗證、APNs 註冊與推播傳送。Apple 會依其自身條款與隱私政策，處理這些功能所需的裝置 token、App 驗證資料與通知 payload。

QTap 不使用廣告或分析 SDK、不出售個人資料，也不會跨 App 或網站追蹤你。QTap 不會要求存取聯絡人、照片、相機、麥克風或位置。

## 資料保留與你的選擇

你可以在 QTap 刪除頻道，撤銷其發送網址並移除伺服器上的頻道紀錄。目前 QTap 沒有可在 App 內解除裝置註冊或刪除伺服器安裝與 App Attest 紀錄的功能；這些註冊資料目前不會自動到期。刪除所有頻道或移除 App 本身，不會刪除伺服器上的裝置註冊資料。若要申請刪除，請透過下方方式聯絡我們，並提供有助辨識註冊資料的資訊，例如頻道名稱。請勿寄送推播網址或憑證。

通知歷史保存在你的裝置上，你可以在 QTap 刪除個別訊息。移除 App 會刪除本機訊息歷史；iOS 移除 App 後仍可能保留 Keychain 項目。

你可以拒絕通知權限，或在 iOS 設定中關閉通知。未授權通知時，QTap 無法接收推播。

## 安全措施

QTap App 透過 HTTPS 連線至服務。裝置憑證與頻道發送 token 均為隨機值，服務只保存其雜湊值。App Attest 可協助驗證受支援的 App 安裝。這些措施能降低風險，但無法保證絕對安全。

## 聯絡方式與政策更新

如需支援、詢問隱私，或申請刪除伺服器上的裝置註冊資料，請聯絡：

cocoaswifty@gmail.com

若 QTap 功能、服務供應商或資料處理方式變更，本政策可能更新；更新後會在本頁標示新的生效日期。
