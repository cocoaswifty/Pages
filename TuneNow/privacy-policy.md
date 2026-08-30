---
layout: default
title: TuneNow Privacy Policy
permalink: /TuneNow/privacy-policy/
---

# TuneNow Privacy Policy

Effective date: August 30, 2026  
Applies to: TuneNow 1.0 (build 1)

TuneNow (Chinese name: 聽一下電台) is an iOS and iPadOS internet radio directory and player provided by CocoaSwifty ("we," "us," or "the developer"). This policy explains what the app stores, which third-party services it contacts, and the choices available to you.

## Summary

- TuneNow does not require an account and does not operate a user-data backend.
- The developer does not receive or store your favorites, recent stations, searches, or listening history on a TuneNow server.
- TuneNow does not include advertising or analytics SDKs and does not use your data for cross-app or cross-website tracking. Radio Browser mirror operators may process search and station requests for service operation and aggregate directory statistics.
- The station directory is dynamic: TuneNow requests current results and stream URLs at runtime rather than shipping a complete catalogue or a fixed station allowlist.
- TuneNow provides live playback only. It does not record, download, convert, export, or provide user-accessible persistent audio files; Apple's player may transiently buffer audio as required for playback.
- To provide station discovery and playback, the app sends requests directly to Radio Browser, station icon hosts, and radio stream providers. Those services receive ordinary network information such as your IP address.

## Information Stored on Your Device

TuneNow stores the following app-functionality data locally on your device:

- Your selected country and recently selected countries
- Your favorite stations
- Your recently played stations, limited to the most recent entries
- Temporary station-icon files in the app's cache directory

Favorites and recent-station records may include public station information such as the station name, identifier, country, stream URL, and icon URL. The initial country is inferred from your device's region setting; TuneNow does not request GPS or precise-location access.

TuneNow does not sync this information to a TuneNow account or developer-operated server. Apple-controlled device backups may handle local app data according to your device and iCloud backup settings.

TuneNow does not access or transmit an advertising identifier, IDFV, or another device-level identifier. The network providers described below may still receive an IP address and standard connection information as part of delivering their services.

## Network Requests and Third-Party Processing

### Radio Browser

TuneNow uses the community-operated [Radio Browser](https://www.radio-browser.info/) API to retrieve countries, station lists, categories, search results, station metadata, and resolved stream URLs.

The directory is dynamic and community-maintained. TuneNow does not bundle the directory, guarantee that a listing proves ownership or permission for a broadcaster's programming, or use this policy as a rights grant. The app requests current directory results and resolves a selected station at playback time; it may try another documented Radio Browser API mirror if a mirror is unavailable.

Depending on the feature you use, TuneNow may transmit the following to a Radio Browser API mirror:

- The selected country code or category tag
- A search term you enter
- The public identifier of a station you choose to play
- The app name/version and platform in a standard User-Agent header
- Network information automatically associated with the request, including your IP address, date/time, and connection details

The stream-resolution endpoint also acts as Radio Browser's station-click endpoint. Radio Browser mirror operators may temporarily record click and IP information for statistics, duplicate filtering, security, or service operation. Retention and server-log practices are controlled by the relevant mirror operator, not by TuneNow. Radio Browser publishes its [API documentation](https://docs.radio-browser.info/) and [server implementation](https://gitlab.com/radiobrowser/radiobrowser-api-rust).

TuneNow uses this information only to return the directory content or station stream you requested. TuneNow does not receive Radio Browser's server logs.

### Radio station streams

When you play a station, your device connects directly to the broadcaster or its streaming provider. The stream provider can receive your IP address, request time, standard connection headers, and playback-related requests. It may also provide audio metadata, such as a current program or track title, which TuneNow processes for playback display.

TuneNow passes the broadcaster-provided stream URL to Apple's AVPlayer for live playback. TuneNow does not operate an audio relay or proxy, copy the stream to a developer server, record it, or offer a save, export, or download control. The player and operating system may create transient playback buffers that are not exposed as user files by TuneNow.

Some independently operated stations still use unencrypted HTTP audio streams. On such a connection, the requested stream and network traffic are not protected by HTTPS and may be observable or altered in transit. TuneNow does not send your favorites, search history, account credentials, contacts, or precise location to the broadcaster.

Each broadcaster or stream provider operates independently and determines its own logging, retention, and privacy practices.

### Station icons

TuneNow may download the HTTPS station-icon URL supplied by Radio Browser. The icon host receives ordinary network information such as your IP address and request headers. Downloaded icons are downsampled and temporarily cached on your device to improve scrolling performance. TuneNow does not scrape broadcaster websites or use the Apple iTunes Search API for album artwork.

### App Store purchases and downloads

If you purchase or download TuneNow through the App Store, Apple processes your Apple Account, transaction, payment, fraud-prevention, and download information under [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/app-store/). TuneNow does not receive your payment-card details. Apple may provide developers with transaction receipts and aggregated sales or usage reports according to Apple's policies.

## What TuneNow Does Not Do

TuneNow does not:

- Require a TuneNow account or login
- Operate an analytics, advertising, or listening-history server
- Sell personal information
- Share personal information for cross-context behavioral advertising
- Track you across apps or websites
- Access or transmit an advertising identifier, IDFV, or other device-level identifier
- Access your contacts, photos, microphone, camera, health data, or precise location
- Upload your favorites or recent-station list to the developer
- Ship a complete station catalogue or a fixed allowlist of broadcasters
- Record, download, convert, export, or persistently save the audio stream

## Purpose and Retention

Local data is used only to provide app features such as remembering your country, favorites, and recent stations. It remains until you change it, the operating system clears cached files, or you uninstall the app, subject to Apple-controlled backups.

The developer has no TuneNow user profile or server-side listening history to retain or delete. Third-party API mirrors, icon hosts, broadcasters, Apple, and GitHub determine their own retention periods for information they process.

## Your Choices and Deletion

You can remove favorite stations in the app. Uninstalling TuneNow removes its local app container from the device, including its preferences and icon cache, subject to Apple's backup and restoration behavior.

Because the developer does not operate a TuneNow user account or data backend, there is no server-side TuneNow profile to access, export, or delete. For information held by a third-party provider, you must contact that provider directly. You may contact us if you need help identifying the relevant provider.

## International Processing

Radio Browser mirrors, icon hosts, broadcasters, Apple, and GitHub may operate in countries other than your own. Your network requests may therefore be processed internationally under the applicable provider's terms and laws.

## Children

TuneNow is not directed to children and the developer does not knowingly collect personal information from children. Radio programming is supplied by independent broadcasters and is not controlled by TuneNow.

## This Policy Website

This page is hosted using GitHub Pages. When you visit it in a browser, GitHub may process network and usage information under the [GitHub General Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).

## Contact, Privacy Requests, and Content Removal

For privacy questions, requests concerning this policy, or requests to remove a station or station icon, contact:

[cocoaswifty@gmail.com](mailto:cocoaswifty@gmail.com)

Please identify the station or URL involved. Do not email sensitive personal information unless it is necessary for us to answer your request.

## Changes to This Policy

We may update this policy when TuneNow changes its features, data practices, or third-party services. The updated effective date will appear at the top of this page. Material changes will be reflected here before or when the related app update is released.

---

# 聽一下電台隱私權政策

生效日期：2026 年 8 月 30 日  
適用版本：TuneNow 1.0（build 1）

TuneNow（中文名稱：聽一下電台）是由 CocoaSwifty（以下稱「我們」或「開發者」）提供的 iOS 與 iPadOS 網路電台目錄及播放器。本政策說明 App 儲存哪些資料、會連線至哪些第三方服務，以及你可採取的選擇。

## 摘要

- 聽一下電台不需要帳號，也沒有儲存使用者資料的自有後端。
- 開發者不會在 TuneNow 伺服器上收到或保存你的收藏、近期電台、搜尋內容或收聽紀錄。
- TuneNow 不包含廣告或分析 SDK，也不會使用你的資料進行跨 App 或跨網站追蹤。Radio Browser mirror 營運者可能為服務運作及彙總目錄統計而處理搜尋與電台請求。
- 電台目錄是動態的：TuneNow 會在執行時請求最新結果及串流網址，不會隨 App 內建完整目錄或固定電台 allowlist。
- TuneNow 僅提供即時播放，不會錄音、下載、轉檔、匯出或提供使用者可存取的持久音訊檔案；Apple 播放器可能依播放需要暫時 buffer 音訊。
- 為提供電台搜尋及播放功能，App 會直接連線至 Radio Browser、電台圖示主機及電台串流供應者；這些服務會收到 IP 位址等一般網路資訊。

## 儲存在裝置上的資料

聽一下電台會在你的裝置上保存下列 App 功能資料：

- 選取的國家及最近選取的國家
- 收藏電台
- 最近播放的電台（僅保留最近數筆）
- App 快取目錄中的暫存電台圖示

收藏及近期電台紀錄可能包含電台名稱、識別碼、國家、串流網址及圖示網址等公開電台資訊。初始國家是依裝置的地區設定推導；App 不會要求 GPS 或精確位置權限。

這些資料不會同步至 TuneNow 帳號或開發者營運的伺服器。裝置本機資料是否進入 Apple 管理的備份，取決於你的裝置與 iCloud 備份設定。

TuneNow 不會存取或傳送廣告識別碼、IDFV 或其他裝置層級識別碼。不過，下述網路服務商為提供服務，仍可能收到 IP 位址及標準連線資訊。

## 網路請求與第三方處理

### Radio Browser

聽一下電台使用社群營運的 [Radio Browser](https://www.radio-browser.info/) API 取得國家、電台清單、分類、搜尋結果、電台 metadata 及解析後的串流網址。

此目錄由社群維護且會動態變更。TuneNow 不會將目錄完整打包進 App，不會保證目錄列出即代表廣播業者對節目擁有權利或取得許可，也不會把本政策當作權利授與。App 會在播放時請求最新目錄結果並解析所選電台；若某個 API mirror 無法使用，可能改用其他 Radio Browser 官方列出的 mirror。

依你使用的功能，App 可能將下列資料傳送至 Radio Browser API mirror：

- 選取的國家代碼或分類標籤
- 你輸入的搜尋詞
- 你選擇播放之電台的公開識別碼
- 標準 User-Agent header 中的 App 名稱／版本及平台
- 請求自動附帶的 IP 位址、日期時間及連線資訊

串流解析 endpoint 同時是 Radio Browser 的電台點擊 endpoint。Radio Browser mirror 營運者可能為統計、排除重複點擊、安全或服務營運而暫時記錄點擊及 IP 資訊。保存期限與伺服器 log 作法由相關 mirror 營運者控制，並非由 TuneNow 控制。Radio Browser 公開其 [API 文件](https://docs.radio-browser.info/)及[伺服器實作](https://gitlab.com/radiobrowser/radiobrowser-api-rust)。

TuneNow 僅使用上述請求取得你要求的目錄內容或電台串流；開發者不會收到 Radio Browser 的伺服器 log。

### 電台串流

播放電台時，你的裝置會直接連線至廣播業者或其串流供應者。串流供應者可能收到你的 IP 位址、請求時間、標準連線 header 及播放相關請求，也可能提供節目或歌曲標題等音訊 metadata，供 App 顯示播放資訊。

TuneNow 會將廣播業者提供的串流網址交給 Apple AVPlayer 進行即時播放。TuneNow 不會營運音訊 relay 或 proxy，不會將串流複製至開發者伺服器，也不會提供錄音、儲存、匯出或下載控制項。播放器及作業系統可能建立播放所需的暫時 buffer，但 TuneNow 不會把它暴露為使用者檔案。

部分獨立電台仍使用未加密的 HTTP 音訊串流。使用這類連線時，所請求的串流與網路流量不受 HTTPS 保護，可能在傳輸途中被觀察或修改。TuneNow 不會將你的收藏、搜尋紀錄、帳號憑證、聯絡人或精確位置傳送給廣播業者。

各廣播業者或串流供應者均獨立營運，並自行決定其 log、保存期限及隱私作法。

### 電台圖示

TuneNow 可能下載 Radio Browser 提供的 HTTPS 電台圖示網址。圖示主機會收到 IP 位址及 request header 等一般網路資訊。下載的圖示會縮圖處理並暫存在裝置上，以提升捲動效能。TuneNow 不會爬取廣播業者網站，也不再使用 Apple iTunes Search API 查詢專輯封面。

### App Store 購買與下載

若你透過 App Store 購買或下載 TuneNow，Apple 會依其 [App Store 與隱私權說明](https://www.apple.com/legal/privacy/data/zh-tw/app-store/)處理 Apple 帳號、交易、付款、防詐與下載資訊。TuneNow 不會收到你的付款卡資料。Apple 可能依其政策向開發者提供交易收據及彙總銷售或使用報告。

## TuneNow 不會進行的行為

TuneNow 不會：

- 要求 TuneNow 帳號或登入
- 營運分析、廣告或收聽紀錄伺服器
- 出售個人資料
- 為跨情境行為廣告分享個人資料
- 跨 App 或網站追蹤你
- 存取或傳送廣告識別碼、IDFV 或其他裝置層級識別碼
- 存取聯絡人、照片、麥克風、相機、健康資料或精確位置
- 將收藏或近期電台清單上傳給開發者
- 隨 App 內建完整電台目錄或固定廣播業者 allowlist
- 錄音、下載、轉檔、匯出或持久保存音訊串流

## 使用目的與保存期限

本機資料僅用於記住國家、收藏及近期電台等 App 功能，保存至你變更資料、作業系統清除快取或解除安裝 App 為止，但仍受 Apple 管理之備份影響。

開發者沒有可保存或刪除的 TuneNow 使用者 profile 或伺服器端收聽紀錄。第三方 API mirror、圖示主機、廣播業者、Apple 與 GitHub 會自行決定其處理資料的保存期限。

## 你的選擇與刪除方式

你可以在 App 內移除收藏。解除安裝 TuneNow 會從裝置移除其本機 App container，包括偏好設定與圖示快取，但仍受 Apple 備份及回復機制影響。

由於開發者沒有營運 TuneNow 使用者帳號或資料後端，因此沒有可供存取、匯出或刪除的伺服器端 TuneNow profile。若資料由第三方供應者持有，你需要直接聯絡該供應者；如需協助辨識相關供應者，可聯絡我們。

## 跨境處理

Radio Browser mirror、圖示主機、廣播業者、Apple 及 GitHub 可能在你所在國家以外營運，因此網路請求可能依相關供應者的條款與適用法律於境外處理。

## 兒童隱私

TuneNow 並非以兒童為主要對象，開發者也不會故意蒐集兒童的個人資料。電台節目由獨立廣播業者提供，內容不受 TuneNow 控制。

## 本政策網站

本頁面使用 GitHub Pages 託管。當你以瀏覽器造訪時，GitHub 可能依其 [GitHub 一般隱私權聲明](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement)處理網路及使用資訊。

## 聯絡、隱私請求與內容移除

若有隱私問題、本政策相關請求，或希望移除電台／電台圖示，請聯絡：

[cocoaswifty@gmail.com](mailto:cocoaswifty@gmail.com)

請註明相關電台或網址。除非回覆請求所必需，請勿在 Email 中寄送敏感個人資料。

## 政策變更

若 TuneNow 的功能、資料作法或第三方服務發生變更，我們可能更新本政策。更新後的生效日期會顯示於頁面頂端；重大變更會在相關 App 更新發布前或同時反映於本頁。
