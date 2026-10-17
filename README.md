# Telegram Glass for Android

Неофициальная модификация Telegram для Android с эффектом «жидкого стекла» в стиле iOS 26.
*Unofficial Telegram for Android mod with an iOS 26‑style "liquid glass" look.* (English below)

> ⚠️ Это **не** официальное приложение Telegram. Сделано на основе открытого исходного кода
> [Telegram for Android](https://github.com/DrKLO/Telegram) (GPL v2). Используйте на свой риск.

---

## 🇷🇺 Русский

### Что нового в v3.0
- **Основа обновлена до Telegram 13.0.2** — все функции Glass перенесены на новую версию.
- **🪩 Дискотека при музыке** (переключатель в Настройках, включён по умолчанию): пока играет музыка, пузыри сообщений и фон профилей плавно меняют цвет (розовый → фиолетовый → синий → голубой → зелёный → жёлтый → оранжевый), стеклянные панели становятся радужными матовыми, по чату скользят белые блики от зеркального шара. Когда музыка останавливается, всё плавно возвращается.
- **Диско-шары на главном экране**: во время музыки листья плавно исчезают, а вместо них падают зеркальные диско-шары (с теми же настройками размера, скорости и количества).
- **Текст остаётся читаемым** во время дискотеки: шапка, плеер, закреп и поле ввода получают плотное матовое стекло.
- **Чаты с ботами**: кнопка «Меню» больше не наезжает на кнопку записи — в чатах с ботами запись голосовых/видео убрана, кнопка «Меню» стоит внутри стеклянной панели.

### Что нового в v2.2
- **Перевод работает**: сервер Telegram отключает перевод для приложений со своим api_id — теперь в этом случае используется встроенный переводчик. «Перевести» в меню сообщения включено по умолчанию; у Premium есть панель «Перевести весь чат/канал».

### Что нового в v2.1
- **Настоящие листья**: в листопаде теперь падают фотореалистичные листья — вытянутый оранжевый лист с черешком и кленовый лист, вперемешку. Поведение и настройки прежние.

### Что нового в v2
- **Без ⋮ в личных чатах**: в шапке осталась только круглая аватарка собеседника — нажатие открывает профиль, **долгое нажатие** открывает прежнее меню ⋮. В группах и каналах ⋮ на месте.
- **Узоры фона профиля** — 11 вариантов (классический, без узора, точки, кольца, ромбы, звёзды, сердечки, волны, листья, кошачьи лапки, снежинки), свой для каждого профиля.
- **Осенний листопад на главном экране**: листья 🍂 падают позади списка чатов и прячутся только за текстом и аватарками, между строками остаются видны. Все настройки в одной строке «🍂 Осенние листья»: вкл/выкл, размер, скорость, количество.
- **Кнопки «Ответить» и «Прочитано»** в уведомлениях, пришедших через официальный Telegram, пока приложение в фоне.

### Что нового в v1.2
- **Аватарка собеседника в шапке чата** вместо кнопки звонка — нажатие открывает профиль. Звонок перенесён в меню ⋮.
- **Анимированные фоны профиля** на весь экран профиля (свечение + плавно движущийся узор, «стеклянные» полупрозрачные карточки) — 8 вариантов. Выбираются через «🎨 Фон профиля» в Настройках или кнопкой-палитрой в шапке профиля. Можно задать свой фон себе и отдельно каждому собеседнику. Хранится **только локально** — другие люди его не видят.
- **Подсветка краёв стекла**: мягкий градиентный блик по краю стеклянных элементов, чтобы они отделялись от фона.
- Мелкие исправления и обновлённый исходный патч.

### Что нового в v1.1
- Курсор больше не наезжает на подсказку «Сообщение»: подсказка начинается сразу после курсора, как в оригинальном Telegram.
- В настройках уведомлений показывается правильная версия.

### Что было в v1
- Шейдер «жидкого стекла» (AGSL, Android 13+): настоящее преломление фона по краям, без размытия и цветной каймы — в меню, диалогах, нижних панелях, шапке чата и панели ввода.
- Стекло без белых рамок, с мягкой градиентной подсветкой краёв (ярче сверху‑слева и снизу‑справа).
- Профиль в стиле iOS: большое фото, крупные круглые стеклянные кнопки с подписями (звонок, видео, звук, поиск, ещё); в своём профиле — «Выбрать фото», «Изменить», «Настройки».
- Раздельная панель ввода: круглая скрепка слева, капсула «Сообщение» со смайликом внутри, круглая кнопка микрофона/отправки справа. Скрепка видна и при наборе, и при редактировании.
- Ретрансляция уведомлений через официальный Telegram: если официальное приложение установлено, Telegram Glass видит его уведомления, сам подгружает новые сообщения и показывает свои уведомления.
- Ввод своих api_id / api_hash при первом запуске, смена в настройках.
- Переключатель «Жидкое стекло» в Настройки → Энергосбережение.

### Отличия от оригинального Telegram
| | Telegram | Telegram Glass |
|---|---|---|
| Жидкое стекло с преломлением | нет | да (Android 13+) |
| Профиль с круглыми кнопками iOS | нет | да |
| Раздельная панель ввода | нет | да |
| Push через Google (FCM) | да | **нет** — только фоновое соединение / ретрансляция |
| Вход через Google, passkeys, покупки Google Play | да | **нет** |

### Установка и настройка — по шагам
1. **Скачайте APK** со страницы [Releases](../../releases) (`telegram-glass-v3.0.apk`).
2. **Разрешите установку из неизвестных источников**: при открытии APK Android предложит разрешить установку для браузера/файлового менеджера → «Настройки» → включить «Разрешить из этого источника».
3. **Play Protect** может показать предупреждение «Приложение не проверено» — нажмите «Подробнее» → «Всё равно установить». Это нормально для неофициальных сборок.
4. **Получите api_id и api_hash**:
   1. Откройте https://my.telegram.org/apps в браузере.
   2. Введите номер телефона в международном формате, затем код, который придёт **в Telegram** (не SMS).
   3. Нажмите «API development tools».
   4. Заполните форму: App title — любое (например, `My Glass`), Short name — 5–32 латинских букв/цифр, Platform — Android. URL и описание можно оставить пустыми.
   5. Нажмите «Create application» и скопируйте **App api_id** (число) и **App api_hash** (32 символа).
5. **Введите их в приложении**: при первом запуске появится окно «API ID / API Hash» → вставьте значения → «Сохранить». Приложение перезапустится.
6. **Войдите** по номеру телефона как в обычном Telegram.
7. **Включите жидкое стекло**: Настройки → Энергосбережение → Чаты → «Жидкое стекло» (там же показан статус шейдера). Нужен Android 13+.
8. **Уведомления через официальный Telegram** (рекомендуется, т.к. FCM нет):
   1. Установите официальный Telegram и войдите в тот же аккаунт.
   2. В Telegram Glass: Настройки → Уведомления → включите ретрансляцию и нажмите «Доступ к уведомлениям» → разрешите Telegram Glass.
   3. На Android 13+: если переключатель серый — Настройки Android → Приложения → Telegram Glass → ⋮ → «Разрешить ограниченные настройки», затем повторите.
   4. Разрешите Telegram Glass показывать уведомления.
9. **Отключите оптимизацию батареи**: Настройки Android → Приложения → Telegram Glass → Батарея → «Без ограничений». На Xiaomi/Huawei/Samsung также разрешите автозапуск и фоновую работу.
10. Сменить api_id/api_hash позже: Настройки → Энергосбережение → строка «🔑 API ID / API Hash» внизу.
11. **Фон профиля**: Настройки → строка «🎨 Фон профиля» (вверху, после аккаунтов) → выберите вариант или «Стандартный». Фон виден, когда вы открываете свой профиль (нажмите на свою аватарку). Для собеседника: откройте его профиль → кнопка-палитра справа вверху (рядом с ⋮) → выберите фон. Всё сохраняется сразу и видно только вам.
12. **Узор фона**: «🎨 Фон профиля» (или кнопка-палитра в профиле) → «✨ Узор» → выберите узор. Сначала выберите цвет фона («🎨 Цвет фона»), иначе узор не виден.
13. **Листопад**: Настройки → «🍂 Осенние листья» → в одном окне: переключатель вкл/выкл, Размер, Скорость, Количество. Применяется сразу.
14. **Меню чата (⋮)** в личных чатах: долгое нажатие на аватарку справа в шапке чата.

### Ограничения
- Нет push через Firebase (FCM): уведомления — только фоновым соединением или через ретрансляцию официального Telegram.
- Нет входа через Google, passkeys и покупок через Google Play.
- Шейдер стекла работает только на Android 13+; на старых версиях — обычный вид.
- Play Protect может ругаться на неофициальную сборку.
- Возможны визуальные огрехи на отдельных экранах; проект любительский.

---

## 🇬🇧 English

### What's new in v3.0
- **Based on Telegram 13.0.2** — all Glass features ported to the new upstream version.
- **🪩 Disco while music plays** (Settings toggle, on by default): message bubbles and profile backgrounds smoothly cycle through one colour at a time (pink → purple → blue → cyan → green → yellow → orange), glass panels turn into iridescent frosted glass, and white mirror-ball light spots sweep across the chat. Everything fades back when the music stops.
- **Disco balls on the main screen**: during music the leaves fade out and mirror disco balls fall instead (same size/speed/amount settings).
- **Text stays readable** during disco: the header, player bar, pinned bar and input bar get dense frosted glass.
- **Bot chats**: the bot "Menu" button no longer overlaps the record button — voice/video recording is removed in bot chats and the Menu button sits inside the glass bar.

### What's new in v2.2
- **Translation works**: Telegram's server disables translation for apps with their own api_id — the built‑in translator is now used in that case. "Translate" in the message menu is on by default; Premium users get the "Translate entire chat/channel" bar.

### What's new in v2.1
- **Real leaves**: the leaf fall now uses photo‑realistic leaves — an elongated orange leaf with a stem and a maple leaf, mixed randomly. Behaviour and settings unchanged.

### What's new in v2
- **No ⋮ in private chats**: only the round peer avatar remains — tap opens the profile, **long‑press** opens the old ⋮ menu. Groups and channels keep ⋮.
- **Profile background patterns** — 11 options (classic, none, dots, rings, diamonds, stars, hearts, waves, leaves, cat paws, snowflakes), per profile.
- **Autumn leaf fall on the main screen**: 🍂 leaves fall behind the chat list and are hidden only behind text and avatars, staying visible between lines. All settings in one row "🍂 Осенние листья": on/off, size, speed, quantity.
- **"Reply" and "Mark as read" buttons** on notifications relayed from the official Telegram while the app is in the background.

### What's new in v1.2
- **Peer avatar in the chat header** instead of the call button — tap opens the profile. Calls moved to the ⋮ menu.
- **Animated profile backgrounds** covering the whole profile (glow + slowly moving pattern, translucent glass cards) — 8 options. Choose via "🎨 Фон профиля" (Profile background) in Settings or the palette button in a profile's header. You can set one for yourself and a separate one per contact. Stored **locally only** — nobody else sees it.
- **Edge highlight on glass**: soft gradient rim on glass elements so they stand out from the background.
- Minor fixes, updated source patch.

### What's new in v1.1
- The caret no longer overlaps the "Message" hint: the hint starts right after the caret, like stock Telegram.
- Correct version label in notification settings.

### What was in v1
- Liquid‑glass AGSL shader (Android 13+): real edge refraction, no blur, no chromatic fringe — menus, dialogs, sheets, chat header and input bar.
- Rimless glass with a soft gradient edge highlight (brighter top‑left / bottom‑right).
- iOS‑style profile: big photo, large round glass buttons with labels (call, video, mute, search, more); own profile: Set photo, Edit, Settings.
- Split input bar: round paperclip, "Message" pill with emoji button inside, round mic/send button. The paperclip stays visible while typing and editing.
- Notification relay through the official Telegram app: Glass listens to official notifications, fetches updates and shows its own notifications.
- Enter your own api_id / api_hash on first launch; change later in settings.
- "Liquid glass" toggle in Settings → Power saving.

### Install & setup, step by step
1. Download `telegram-glass-v3.0.apk` from [Releases](../../releases).
2. Allow installing from unknown sources for your browser / file manager when prompted.
3. If Play Protect warns, tap "More details" → "Install anyway".
4. Get api_id / api_hash: open https://my.telegram.org/apps, log in with your phone (the code arrives in Telegram), open "API development tools", fill in any app title, a 5–32 char short name, platform Android, press "Create application", copy **App api_id** and **App api_hash**.
5. On first launch paste them into the "API ID / API Hash" dialog → Save (the app restarts).
6. Log in with your phone number.
7. Enable liquid glass: Settings → Power saving → Chats → "Liquid glass" (Android 13+).
8. Notification relay: install the official Telegram (same account) → in Glass: Settings → Notifications → enable relay → grant Notification access. On Android 13+ you may need App info → ⋮ → "Allow restricted settings" first. Allow notifications for Glass.
9. Disable battery optimization for Telegram Glass (Battery → Unrestricted; allow autostart on Xiaomi/Huawei/Samsung).
10. Change api credentials later: Settings → Power saving → "🔑 API ID / API Hash" row.
11. Profile background: Settings → "🎨 Фон профиля" row (near the top, after accounts) → pick one or "Стандартный" (default). It shows when you open your own profile (tap your avatar). For a contact: open their profile → palette button top‑right (next to ⋮) → pick. Saved instantly, visible only to you.
12. Background pattern: "🎨 Фон профиля" (or the palette button in a profile) → "✨ Узор" → pick. Choose a background color first ("🎨 Цвет фона"), otherwise the pattern isn't visible.
13. Leaf fall: Settings → "🍂 Осенние листья" → one dialog with on/off switch, size, speed and quantity. Applies instantly.
14. Chat menu (⋮) in private chats: long‑press the avatar at the top right of the chat header.

### Limitations
- No Firebase (FCM) push; no Google sign‑in, passkeys or Google Play purchases.
- Glass shader requires Android 13+.
- Unofficial build — Play Protect may warn.

---

## License / Source
Based on [Telegram for Android](https://github.com/DrKLO/Telegram) (GNU GPL v2). The complete source changes are in
[`telegram-glass-v3.0.patch`](telegram-glass-v3.0.patch), applied on top of upstream commit `f32ffeec7` ("update to 13.0.2 (7175)"):

```
git clone https://github.com/DrKLO/Telegram && cd Telegram && git checkout f32ffeec7
git apply ../telegram-glass-v3.0.patch
./gradlew :TMessagesProj_App:assembleAfatRelease
```
No api credentials are included; users supply their own. This project is not affiliated with Telegram FZ‑LLC.
