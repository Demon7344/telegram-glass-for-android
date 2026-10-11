# Telegram Glass for Android

Неофициальная модификация Telegram для Android с эффектом «жидкого стекла» в стиле iOS 26.
*Unofficial Telegram for Android mod with an iOS 26‑style "liquid glass" look.* (English below)

> ⚠️ Это **не** официальное приложение Telegram. Сделано на основе открытого исходного кода
> [Telegram for Android](https://github.com/DrKLO/Telegram) (GPL v2). Используйте на свой риск.

---

## 🇷🇺 Русский

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
1. **Скачайте APK** со страницы [Releases](../../releases) (`telegram-glass-v1.1.apk`).
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

### Ограничения
- Нет push через Firebase (FCM): уведомления — только фоновым соединением или через ретрансляцию официального Telegram.
- Нет входа через Google, passkeys и покупок через Google Play.
- Шейдер стекла работает только на Android 13+; на старых версиях — обычный вид.
- Play Protect может ругаться на неофициальную сборку.
- Возможны визуальные огрехи на отдельных экранах; проект любительский.

---

## 🇬🇧 English

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
1. Download `telegram-glass-v1.1.apk` from [Releases](../../releases).
2. Allow installing from unknown sources for your browser / file manager when prompted.
3. If Play Protect warns, tap "More details" → "Install anyway".
4. Get api_id / api_hash: open https://my.telegram.org/apps, log in with your phone (the code arrives in Telegram), open "API development tools", fill in any app title, a 5–32 char short name, platform Android, press "Create application", copy **App api_id** and **App api_hash**.
5. On first launch paste them into the "API ID / API Hash" dialog → Save (the app restarts).
6. Log in with your phone number.
7. Enable liquid glass: Settings → Power saving → Chats → "Liquid glass" (Android 13+).
8. Notification relay: install the official Telegram (same account) → in Glass: Settings → Notifications → enable relay → grant Notification access. On Android 13+ you may need App info → ⋮ → "Allow restricted settings" first. Allow notifications for Glass.
9. Disable battery optimization for Telegram Glass (Battery → Unrestricted; allow autostart on Xiaomi/Huawei/Samsung).
10. Change api credentials later: Settings → Power saving → "🔑 API ID / API Hash" row.

### Limitations
- No Firebase (FCM) push; no Google sign‑in, passkeys or Google Play purchases.
- Glass shader requires Android 13+.
- Unofficial build — Play Protect may warn.

---

## License / Source
Based on [Telegram for Android](https://github.com/DrKLO/Telegram) (GNU GPL v2). The complete source changes are in
[`telegram-glass-v1.1.patch`](telegram-glass-v1.1.patch), applied on top of upstream commit `f2908b1` ("update to 12.10.6 (7112)"):

```
git clone https://github.com/DrKLO/Telegram && cd Telegram && git checkout f2908b1
git apply ../telegram-glass-v1.1.patch
./gradlew :TMessagesProj_App:assembleAfatRelease
```
No api credentials are included; users supply their own. This project is not affiliated with Telegram FZ‑LLC.
