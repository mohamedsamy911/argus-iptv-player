<p align="center">
  <img src="docs/logo.png" alt="Argus IPTV Player" width="180">
</p>

<h1 align="center">Argus IPTV Player</h1>

<p align="center">
  A fast, good-looking IPTV player for <b>Android TV and Google TV</b>, built for the remote.<br>
  Live TV, movies and series from your own <b>Xtream Codes</b> subscription, in <b>English and Arabic</b>.
</p>

<p align="center">
  <a href="https://github.com/mohamedsamy911/argus-iptv-player/releases/latest/download/argus.apk"><b>⬇ Download the latest APK</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/mohamedsamy911/argus-iptv-player/releases">All releases</a>
  &nbsp;·&nbsp;
  <a href="#العربية">العربية</a>
</p>

<p align="center"><img src="docs/banner.png" alt="" width="480"></p>

> Argus is a player only. It doesn't come with any channels or content. You need a subscription from an IPTV
> provider that gives you an **Xtream Codes** login (server address, username and password).

---

## Contents

- [Features](#features)
- [Install on your TV](#install-on-your-tv)
- [First setup](#first-setup)
- [Settings guide](#settings-guide)
- [Updates](#updates)
- [Privacy](#privacy)
- [Requirements](#requirements)

---

## Features

### Home
- **Netflix-style home** with a warm "Good evening" greeting, the date and the time.
- A big **spotlight card** for the focused title: artwork, year, genre, rating and plot, or
  **"Pick up where you left off"** with the episode and the minutes left.
- Separate **Continue watching** rows for **Series**, **Movies** and **Channels**, plus favorite channels,
  new movies, new series, favorite movies and favorite series.
- Channel cards show the logo, the name and **what's on now**.
- **Hold OK on a card** for a quick menu: add to favorites, remove from Continue watching, mark a movie as watched.

### Live TV
- All your categories, with **favorites**, **recently watched** and **new** lists built in.
- **Grid or list** view, sorting by number or name, and a **live preview** of the focused channel.
- Full-screen player with channel up/down zapping, number entry and the last-channel key.
- **Mini guide** in the player: OK (or the remote's GUIDE key) opens the channel list with what's on now on every channel and what's next on the focused one.
- **Catch-up** (replay) for channels that support it, straight from the TV guide.
- Option to open the **last channel on start**.

### TV guide (EPG)
- A full **TV guide grid**: 24 hours back and 24 hours ahead, by category.
- Guide data from your provider, the provider's full guide file, or **your own XMLTV links**
  (`.xml` or `.xml.gz`). Add **several links**: when two cover the same channel, the first one wins.
- Channels are matched by the provider's guide id or by name ("MBC Masr HD" matches "MBC Masr").
- **Program reminders**: press OK on a show that hasn't started, and a "Starting now" popup offers to switch
  to the channel when it begins.
- **Search the guide**: Search also finds shows by name across all channels, "On now" to watch or later to set a reminder.
- A time shift setting if your guide runs early or late.

### Movies and series
- Every category, grid or list view, sorting, favorites and search.
- Detail pages with the poster, backdrop, plot, director, cast, rating, running time and trailer.
- **TMDB details** (optional, free key): Arabic or English plot, genres, **cast photos**, better artwork and
  trailers from The Movie Database, filling in what your provider leaves out.
- **Resume where you stopped**, even after a power cut. Progress shows on the Resume button and on every
  episode card ("12 min left"), and finished episodes get a check mark.
- **Auto-play next episode** with a 10-second "Next episode in…" card, and a **Skip intro** button.
  Both can be turned off.
- Previous and next episode from the player.
- **Mark as watched / unwatched**: a button on movies, and hold OK on an episode.

### Player
- Built on **Media3 / ExoPlayer** with an **FFmpeg** audio decoder for AC3, E-AC3, DTS and other formats TVs
  often can't play.
- Audio track and subtitle choice, preferred audio and subtitle language, and subtitle size.
- Aspect ratio (fit, fill, zoom), playback speed and a sleep timer.
- **Stream info** overlay: resolution, frame rate, codecs, bitrate, connection speed, buffer and dropped frames.
- Buffer size, hardware or software audio decoding, **match frame rate (AFR)**, tunneled playback and a custom
  user agent for difficult streams.
- Automatic fallback between stream formats (`.ts`, `.m3u8`) when a provider only serves one.
- Option to use an **external player** instead (for example VLC or MX Player).

### Made for the TV
- **Type on your phone instead of the remote**: scan a QR code to add a playlist or to fill in a settings
  section (guide links, TMDB key, user agent) from your phone. The phone needs to be on the same Wi-Fi.
- **Android TV home screen**: your continue-watching titles in the system "Play next" row and an Argus row of
  favorites.
- **Voice search** from the remote's microphone button.
- Smooth remote navigation: rows only scroll when needed and focus comes back to where you were.
- Mouse and touch work too (handy on phones, tablets and Windows Subsystem for Android).
- An "Exit Argus?" check so one stray Back press doesn't close the app.

### Look and language
- **English and Arabic** throughout, with a full right-to-left layout in Arabic and an in-app language switch.
- Four themes: **Dark** (default), **Argus** (warm amber), **Cinema** (black and red) and **Light**.
- Interface size, text size and grid size settings for any TV and viewing distance.

### Account and content
- Several playlists, each with its account status, expiry date and number of connections.
- **Automatic content updates** (on every start, every 6 or 12 hours, daily or weekly) or update now.
- **Parental PIN**, plus hiding and locking categories.
- Clear watch history at any time.

---

## Install on your TV

Argus isn't on the Play Store, so you install the APK file yourself. You only do this once: after that the
app updates itself.

**With the Downloader app (easiest):**
1. On the TV, install **Downloader** (by AFTVnews) from the Play Store.
2. Allow it to install apps: *Settings → Apps → Special app access → Install unknown apps → Downloader*.
3. Open Downloader and enter this link:
   ```
   https://github.com/mohamedsamy911/argus-iptv-player/releases/latest/download/argus.apk
   ```
4. Press **Install** when Android asks.

**From a computer or a USB stick:** download `argus.apk` from the
[latest release](https://github.com/mohamedsamy911/argus-iptv-player/releases/latest), copy it to the TV and open
it with a file manager. Or install it with `adb install argus.apk`.

---

## First setup

1. Open Argus. The **Add playlist** screen asks for your provider's **server address**, **username** and
   **password** (and an optional name).
2. Typing with the remote is slow, so the screen also shows a **QR code**. Scan it with your phone camera,
   fill in the login on your phone and tap **Send to TV**. The TV fills the form and logs in.
3. Argus downloads your channels, movies and series. Large lists take a minute the first time.
4. You land on **Home**. Use the left menu for Search, Live TV, TV guide, Movies, Series and Settings.

---

## Settings guide

| Section | What you'll find |
|---|---|
| **General** | Language (System, English, العربية), theme, interface size, text size, grid size |
| **Playlist** | Switch or add playlists, account status, **Update now**, automatic updates |
| **Player** | Built-in or external player, live preview, open last channel on start, auto-play next episode, Skip intro, channel key direction, aspect ratio, audio and subtitle language, subtitle size |
| **Playback & decoding** | Live stream format, buffer, audio decoder, match frame rate, tunneled playback, user agent |
| **Lists & TV guide** | Channel order, guide time shift, **TV guide source** and **guide links**, guide status |
| **Movie and series details** | **TMDB key** for richer details (see below) |
| **Parental control** | PIN, hide and lock categories |
| **Data** | Clear watch history, automatic update check, version and **Check for updates** |

Sections with long text fields have a **Set up from your phone** row: scan the QR code, edit everything on your
phone and tap Send.

### Free TV guide

If your provider has no guide, add a free XMLTV link under *Lists & TV guide → TV guide source → Custom link*.
For example, the Middle East file from [epgshare01](https://epgshare01.online/epgshare01/):

```
https://epgshare01.online/epgshare01/epg_ripper_AE1.xml.gz
```

### TMDB key (optional)

1. Create a free account at [themoviedb.org](https://www.themoviedb.org/), then go to *Settings → API* and request
   a key.
2. In Argus, open *Movie and series details → Set up from your phone* and paste the **API key** or the
   **API Read Access Token**.
3. Open any movie or series: you'll see cast photos, a better backdrop and the plot in your language.

---

## Updates

- Argus checks this page for a new version when it starts (up to twice a day). When there is one, a box shows
  what's new with **Update** and **Later**.
- **Update** downloads the new version and opens the Android installer. Press **Install**. Your playlists,
  favorites, history and settings stay.
- The first time, Android asks you to allow Argus to **install apps**. Turn it on, go back and press Update again.
- You can check by hand from *Settings → Data → Version*, and turn the automatic check off there.

---

## Privacy

- Your login, history, favorites and settings stay **on your TV**. There are no accounts, ads or tracking.
- Argus only talks to your IPTV provider, the guide links you add, TMDB (only if you add a key) and GitHub
  (to look for updates).
- The QR code pages run on your TV, only on your home network, and only while that screen is open.

---

## Requirements

- Android TV, Google TV or any Android device with **Android 7.0** or newer.
- An IPTV subscription with an **Xtream Codes** login.
- For the phone QR pages: a phone on the same Wi-Fi as the TV.

---

<a id="العربية"></a>

<div dir="rtl">

## العربية

**أرجوس** مشغّل IPTV سريع وأنيق لأجهزة **Android TV وGoogle TV**، مصمَّم للتحكم بالريموت. يعرض البث المباشر والأفلام
والمسلسلات من اشتراك **Xtream Codes** الخاص بك، والتطبيق بالكامل **بالعربية والإنجليزية** مع واجهة من اليمين إلى اليسار.

> أرجوس مشغّل فقط ولا يحتوي على أي قنوات أو محتوى. تحتاج إلى اشتراك من مزوّد IPTV يعطيك بيانات دخول Xtream Codes
> (عنوان السيرفر واسم المستخدم وكلمة المرور).

### أهم المزايا
- **واجهة رئيسية بأسلوب نتفليكس** مع تحية وبطاقة كبيرة "أكمل من حيث توقفت"، وصفوف متابعة المشاهدة للمسلسلات والأفلام والقنوات.
- **البحث في دليل البرامج**، و**دليل مصغّر** داخل المشغّل يعرض ما يُعرض الآن والتالي، و**تحديد العناوين كمُشاهَدة**.
- **البث المباشر** بكل الفئات، مع المفضلة والمشاهدة مؤخرًا، وعرض شبكي أو قائمة، ومعاينة القناة، والتنقل بين القنوات، والإعادة (Catch-up).
- **دليل برامج كامل** من المزوّد أو من **روابط XMLTV متعددة** تضيفها بنفسك، مع **تذكير بالبرامج** قبل بدايتها.
- **الأفلام والمسلسلات** مع **متابعة المشاهدة من حيث توقفت**، و**التشغيل التلقائي للحلقة التالية**، و**زر تخطي المقدمة**.
- **تفاصيل من TMDB** (اختياري): القصة بالعربية، وصور طاقم التمثيل، وصور خلفية أفضل، والإعلانات.
- **مشغّل قوي** مع فك ترميز الصوت FFmpeg، واختيار الصوت والترجمة، وأبعاد الصورة، والسرعة، ومؤقت النوم، و**معلومات البث**.
- **الكتابة من هاتفك بدلًا من الريموت**: امسح رمز QR لإضافة قائمة تشغيل أو لتعبئة إعدادات (روابط الدليل، مفتاح TMDB) من هاتفك.
- صف على **شاشة Android TV الرئيسية**، و**البحث الصوتي**، و**أربعة مظاهر**، والتحكم في حجم الواجهة والخط والشبكة.
- **رمز PIN للرقابة الأبوية**، وإخفاء الفئات وقفلها، وتحديث المحتوى تلقائيًا.
- **تحديث التطبيق ذاتيًا** من هذه الصفحة، مع إمكانية البحث عن تحديث يدويًا أو إيقاف البحث التلقائي.

### التثبيت
1. ثبّت تطبيق **Downloader** على التلفاز من متجر Play، واسمح له بتثبيت التطبيقات.
2. افتحه وأدخل الرابط:
   ```
   https://github.com/mohamedsamy911/argus-iptv-player/releases/latest/download/argus.apk
   ```
3. اضغط **تثبيت**. بعد ذلك يحدّث التطبيق نفسه تلقائيًا.

### الإعداد الأول
افتح أرجوس، ثم امسح رمز QR الظاهر في شاشة **إضافة قائمة تشغيل** بكاميرا هاتفك، واكتب بيانات الدخول على الهاتف
واضغط **إرسال إلى التلفاز**. سيُحمِّل التطبيق القنوات والأفلام والمسلسلات ثم يفتح الواجهة الرئيسية.

### الخصوصية
بيانات الدخول والسجل والمفضلة والإعدادات تبقى **على جهازك فقط**، بدون حسابات أو إعلانات أو تتبّع.

</div>
