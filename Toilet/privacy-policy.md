---
layout: default
title: Toilet Privacy Policy
permalink: /Toilet/privacy-policy/
---

# Toilet Privacy Policy

Effective date: August 27, 2026

Toilet is an iOS app for finding nearby public toilets and helping improve toilet location information. It uses your location to show nearby toilets, lets you submit new or corrected toilet information for administrator review, and uses Firebase services for account identification, data storage, and app diagnostics.

This policy explains what information Toilet stores, what services it contacts, and what the app does not do.

## Information Stored on Your Device

Toilet may store the following information locally on your device:

- An anonymous Firebase user identifier
- Your last known position and country code, used to load nearby toilet data faster
- App state such as login count, review status, paid status, and filter preferences

This local information is stored using Apple UserDefaults for app functionality.

## Location

Toilet asks for location permission so it can show toilets near you, sort toilets by distance, move the map to your current area, and associate reports or diagnostics with the relevant country or nearby area.

Your location may be sent to Firebase when the app loads nearby toilets, records loading or route-related app diagnostics, reports errors, or when you submit a new or corrected toilet location. Toilet does not use location data for advertising or tracking across apps and websites.

## Firebase and App Data

Toilet uses Firebase Authentication and Cloud Firestore. The app signs in anonymously and stores an anonymous user identifier so app data can be associated with one app installation.

To provide and improve app functionality, Toilet may send the following data to Firebase:

- Anonymous Firebase user identifier
- Device system name, iOS version, app language, country code, installation time, last active time, color mode, login count, and review status
- Loading time, app interaction records, route or stay records related to toilet search and map usage
- Error diagnostics, including error text, country code, approximate stored position, and timestamp
- Toilet information you submit, such as name, address or location note, coordinates, toilet type, accessibility, payment, baby-changing availability, rating, report reason, and timestamp

Firebase may process standard network information such as your IP address as part of normal internet communication.

## User-Submitted Toilet Information and Review

When you submit a new toilet, edit a toilet, or submit a deletion, the proposed listing data is sent to Firebase and placed in an administrator review queue. An administrator reviews the proposed change, and only an approved submission updates the public toilet directory. While a submission is pending, the submitting device may show a local preview of the proposed change; the pending change is not published to other users until it is approved. You can see the status of your submissions in the app.

If you find inaccurate listing information, the current in-app way to bring it to our attention is to edit the listing and submit the proposed correction. This workflow is for factual toilet-data corrections. Toilet does not currently provide free-form posts, comments, chat, or an in-app user-blocking feature. Ratings are a separate feature and may update an aggregate toilet rating without going through the listing-edit review queue.

Do not enter personal information into toilet names, address notes, or report fields.

## Retention and Deletion

Toilet keeps information only for as long as it is needed for the purposes described in this policy. Our current retention rules are:

- Local information, including the last known location, country code, and filter preferences, remains on your device until you uninstall Toilet or clear its app data.
- The anonymous Firebase user ID and account metadata are kept while the installation uses Toilet. If you ask us to delete your data, we will delete the anonymous Firebase user and associated user records from the production database within 30 days, except for information that must be retained for security, fraud prevention, or legal reasons.
- Pending or rejected submissions may be retained for up to 24 months after the last moderation action for review and abuse prevention. Approved toilet information is public content and may remain published while it is useful to the community; we may remove or anonymize it when requested or when it is no longer needed.
- Error and operational diagnostic records are retained for up to 90 days. Deleted data may remain in encrypted backups for up to 90 additional days before the backup cycle removes it.

To request deletion, email [cocoaswifty@gmail.com](mailto:cocoaswifty@gmail.com?subject=Toilet%20data%20deletion%20request) with the subject “Toilet data deletion request”. Include the anonymous user ID if you have it and enough information for us to identify the installation or submissions. We will confirm the request and tell you if any data must be retained and why. Deleting the anonymous account may prevent access to pending submissions and other installation-linked features.

## Withdrawing Permission and Consent

Location access is optional. You can withdraw location permission at any time in **iOS Settings → Privacy & Security → Location Services → Toilet**. After permission is withdrawn, Toilet will not request or send new location data, but nearby-toilet search and distance sorting may not work. Previously collected location data is not automatically deleted; request deletion using the email process above.

You can also stop Firebase processing by stopping use of the app and requesting deletion of the anonymous account and associated data. Uninstalling the app removes local UserDefaults data from the device, but does not by itself delete data already sent to Firebase.

## What Toilet Does Not Do

Toilet does not:

- Sell personal data
- Use advertising SDKs
- Track you across apps or websites
- Ask for your name, email address, phone number, contacts, microphone, camera, or photos
- Operate a social account system or collect passwords

## App Store Privacy Disclosure

Toilet's privacy manifest and App Store disclosures may identify precise location, user ID, product interaction, other user content, and diagnostic data as data used for app functionality and limited app analytics. These categories cover nearby toilet search, anonymous Firebase operation, usage and loading diagnostics, submitted toilet information, and error reporting.

The app declares UserDefaults usage in its privacy manifest for storing app preferences and local app state.

Toilet does not use collected data for tracking or advertising.

## Contact

For privacy questions about Toilet, contact:

cocoaswifty@gmail.com

## Changes to This Policy

This privacy policy may be updated when Toilet changes its features, data practices, or third-party services. Updates will be posted on this page.

---

# Toilet 隱私權政策摘要

生效日期：2026 年 8 月 27 日

Toilet 是用來尋找附近公廁並協助改善廁所地點資料的 iOS App。App 會使用定位權限來顯示附近廁所、依距離排序、移動地圖到目前位置，並在你提交新增、修改或刪除資料時，將提案交由管理員審核。

App 可能在裝置本機保存匿名 Firebase 使用者 ID、最後位置、國家碼、登入次數、評論狀態、付費狀態與篩選偏好。這些資料使用 Apple UserDefaults 儲存。

Toilet 使用 Firebase Authentication 匿名登入，並使用 Cloud Firestore 儲存與讀取廁所資料。App 可能傳送匿名使用者 ID、裝置系統名稱、iOS 版本、語言、國家碼、安裝時間、最後活躍時間、深色/淺色模式、登入次數、載入時間、路徑或停留紀錄、錯誤診斷，以及你主動提交的廁所名稱、地址或位置描述、座標、類型、無障礙、付費、換尿布檯、評分與回報原因。

Firebase 在正常網路連線中可能處理你的 IP 位址。Toilet 不使用廣告 SDK、不出售個人資料、不跨 App 或網站追蹤你，也不會要求姓名、電子郵件、電話、聯絡人、麥克風、相機、照片或密碼。

請不要在廁所名稱、地址描述或回報內容中輸入個人資料。

## 使用者提交資料與人工審核

當你新增公廁、修改公廁資料或提交刪除要求時，提案會先送到 Firebase 的管理員審核清單。管理員檢查提案後，只有核准的內容才會更新公開公廁資料。審核期間，提交修改的裝置可能會先看到修改內容的本機預覽；其他使用者要等管理員核准後才會看到更新。你可以在 App 內查看自己提交資料的審核狀態。

如果你發現公廁資料有誤，目前 App 內將問題交給我們處理的方式，是直接編輯該筆資料並提交修改。這個流程是針對公廁事實資料的更正；Toilet 目前沒有自由發文、留言、聊天或 App 內封鎖使用者功能。評分是獨立功能，可能會直接更新公廁的彙總評分，不會進入公廁資料修改的審核流程。

## 資料保存期限與刪除

Toilet 只會在完成本政策所述目的所需期間保存資料，目前規則如下：

- 最後位置、國家碼與篩選偏好等本機資料，會保留到你解除安裝 Toilet 或清除 App 資料為止。
- 匿名 Firebase 使用者 ID 與帳戶中繼資料會在此安裝仍使用 Toilet 期間保存。你提出刪除要求後，我們會在 30 天內刪除 Firebase 匿名使用者與正式資料庫中的關聯使用者資料；基於安全、防濫用或法律義務必須保留的資料除外。
- 待審核或遭拒的投稿，可能在最後一次審核動作後保存最多 24 個月，用於審核與防止濫用。已核准的公廁資料屬於公開內容，在對社群有用期間可能持續保留；收到要求或不再需要時，我們會移除或匿名化。
- 錯誤與營運診斷資料最多保存 90 天。刪除後的資料可能因加密備份週期再保留最多 90 天，之後才會從備份移除。

如要刪除資料，請寄信至 [cocoaswifty@gmail.com](mailto:cocoaswifty@gmail.com?subject=Toilet%20data%20deletion%20request)，主旨填寫「Toilet data deletion request」。若知道匿名使用者 ID 請一併提供，並提供足以辨識安裝或投稿的資訊。我們會確認要求，並說明任何因安全、反詐欺或法律原因必須保留的資料及理由。刪除匿名帳戶後，可能無法再存取待審投稿或其他與該安裝相關的功能。

## 撤回權限與同意

定位權限不是強制的。你可以隨時前往 **iOS「設定」→「隱私權與安全性」→「定位服務」→「Toilet」** 撤回定位權限。撤回後，Toilet 不會再要求或傳送新的定位資料，但附近公廁搜尋與距離排序可能無法使用。先前已收集的定位資料不會自動刪除，請依上述電子郵件流程提出刪除要求。

你也可以停止使用 App，並透過電子郵件要求刪除匿名帳戶及相關資料，以停止 Firebase 的後續處理。解除安裝 App 會移除裝置上的 UserDefaults 本機資料，但不會自動刪除已傳送至 Firebase 的資料。

本 App 的隱私問題請聯絡：

cocoaswifty@gmail.com
