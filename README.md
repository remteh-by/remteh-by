# RemTeh · приложения и инструменты

Развиваем приложения для Remote Play и наблюдаемой диагностики устройств. Репозиторий, пакет и проверка на конкретном устройстве — разные этапы: ниже указаны фактические платформы и публичные каналы.

## Быстрые тесты онлайн

[**Мышь: кнопки и удержание →**](https://remteh-by.github.io/Mouse-Tester/#buttons) · [**Колесо →**](https://remteh-by.github.io/Mouse-Tester/#wheel) · [**Движение →**](https://remteh-by.github.io/Mouse-Tester/#movement) · [**Рисование →**](https://remteh-by.github.io/Mouse-Tester/#sensor) · [**Отчёт →**](https://remteh-by.github.io/Mouse-Tester/#report)

[**Геймпад: открыть вебдиагностику RemTeh →**](https://remteh.by/remont-gamepadov/diagnostika-gejmpada)

[**Device Lab: открыть историю и сравнение отчётов →**](https://remteh-by.github.io/Device-Lab/) · [**Тест мыши на RemTeh.by →**](https://remteh.by/remont-myshek/test-myshek)

| Проект | Назначение и платформа | Загрузка / исходники | Статус |
|---|---|---|---|
| **Deckivo** | PS5 Remote Play; Android ARM64, macOS Apple Silicon, подготовленная Switchroot Ubuntu ARM64 | [Сайт](https://remteh-by.github.io/remteh-remote-play/) · [Releases](https://github.com/remteh-by/remteh-remote-play/releases) · [Исходники](https://github.com/remteh-by/remteh-remote-play) | Опубликована 0.8.9 preview (Android 34, desktop 25), без физической приёмки. Для Ubuntu архив обновления не заменяет первую установку runtime |
| **X Play** | Xbox Remote Play launcher для macOS Apple Silicon и Ubuntu ARM64 | [Сайт](https://remteh-by.github.io/x-portal/) · [Releases](https://github.com/remteh-by/x-portal/releases/tag/v1.3.1) · [Исходники](https://github.com/remteh-by/x-portal) | 1.3.1 preview: именованные профили, импорт/экспорт, профиль отдельной игровой сессии. Проверки окна на Switch относятся к 1.3.0; новый пакет и Xbox-сеанс требуют физической приёмки. Mac ad-hoc, без нотарификации |
| **DualSense Tester** | Наблюдения Android InputDevice API, профиль DualSense | [Исходники и инструкции](https://github.com/remteh-by/dualsense-tester) · [Releases](https://github.com/remteh-by/dualsense-tester/releases/tag/v1.2.2) | Debug preview 1.2.2 / 5; обновление debug 1.2.1 с сохранением данных проверено в Android 15 SDK. Для прежней release-установки нужен оригинальный сертификат |
| **Xbox Tester** | Аналогичная диагностика Android, профиль Xbox | [Исходники и инструкции](https://github.com/remteh-by/xbox-tester) · [Releases](https://github.com/remteh-by/xbox-tester/releases/tag/v1.2.2) | Debug preview 1.2.2 / 5; проверено обновление debug 1.2.1 в Android 15 SDK. Прежняя release-установка требует оригинального сертификата |
| **Joy-Con Tester** | Android, доступные оси/кнопки Joy-Con | [Исходники и инструкции](https://github.com/remteh-by/joycon-tester) · [Releases](https://github.com/remteh-by/joycon-tester/releases/tag/v1.2.2) | Debug preview 1.2.2 / 5; debug-обновление проверено в SDK. Одиночный/парный режим и вибрация физически не приняты |
| **Mouse Tester** | Веб-инструмент: кнопки, колесо, события браузера, локальная история и отчёт | [Открыть онлайн](https://remteh-by.github.io/Mouse-Tester/) · [Releases](https://github.com/remteh-by/Mouse-Tester/releases/tag/v1.3.1) · [Исходники](https://github.com/remteh-by/Mouse-Tester) | 1.3.1 preview: естественные левые клавиши, вдавливание, стрелки, гравировка логотипа и автономная PWA. Частота браузерных событий не равна USB polling rate |
| **Device Lab** | Локальная история, импорт и сравнение отчётов мыши, геймпада и телефона | [Открыть онлайн](https://remteh-by.github.io/Device-Lab/) · [Releases](https://github.com/remteh-by/Device-Lab/releases/tag/v0.2.2) · [Исходники](https://github.com/remteh-by/Device-Lab) | 0.2.2 preview: сохранение из двух вкладок без перезаписи, объединение прежней истории, автономная PWA. Результаты не отправляются на сервер |
| **PhoneCheck** | Android: локальные приёмочные проверки телефона, история и отчёт | [APK и исходники](https://github.com/remteh-by/Device-Lab/releases/tag/v0.2.2) · [Инструкция](https://github.com/remteh-by/Device-Lab/tree/main/phonecheck) | 0.2.1 / 3 debug preview; обновление, импорт, сравнение и отказы проверены в Android 15 SDK. Физические камера, звук, мотор и питание требуют отдельной проверки |

[Установка и автоматическое обновление в Ubuntu](https://github.com/remteh-by/Device-Lab/tree/main/ubuntu): Mouse Tester, Device Lab, X Play ARM64 и веб-проверка геймпадов. Пользовательский таймер сверяет SHA-256 и сохраняет предыдущую и запущенную версии; Deckivo использует свой механизм. Учебный desktop-tutorial не является продуктом.

## Проверки и ограничения

Предварительные версии опубликованы по поручению владельца. Выполнены сборки и автоматические проверки; окно X Play ARM64 и сохранение профиля версии 1.3.0 ранее проверены на физическом Switch Ubuntu. Для нового выпуска эта проверка остаётся открытой. PS5/Xbox-сеансы и аппаратные измерения Android-тестеров в этом выпуске не приняты. Успешный тест кода или красивый экран не заменяет реальную проверку видео, звука, ввода, сна/пробуждения и обновления с сохранением данных.

Не обещаем нулевую задержку, 4K, любую Ubuntu, все Mac или универсальную аппаратную калибровку. Версии, архитектуры, контрольные суммы, сертификаты и инструкции относятся к конкретному файлу из Releases. Поддержка ведётся через репозитории проектов; не прикладывайте токены, пароли, регистрации консолей и данные клиентов к публичным обращениям.

## Лицензии

Deckivo — AGPL-3.0 с условиями upstream/OpenSSL; X Play — MIT; три Android-тестера имеют собственную proprietary-лицензию. У Mouse Tester новая лицензия от имени владельца не назначалась. Смотрите LICENSE/COPYING соответствующего проекта. Наличие исходников и пожертвование не меняют лицензию автоматически.

RemTeh — независимые проекты, не официальные приложения Sony, Microsoft или Nintendo. Кнопок покупки на несуществующие магазины здесь нет.

## Поддержка разработки

[Выбрать способ поддержки RemTeh](https://remteh-by.github.io/remteh-remote-play/#support): Ko-fi, Afdian, Boosty, DonationAlerts, DonatePay и OKX Pay. Рядом с каждым вариантом указан фактический статус: наличие профиля не подтверждает приём денег. Для Boosty требуется верификация, Afdian ещё не подтверждён; OKX Pay — ручной перевод через приложение. Patreon не используется. Донат добровольный, все проверки доступны без оплаты.
