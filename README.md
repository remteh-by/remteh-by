# RemTeh · приложения и инструменты

Развиваем приложения для Remote Play и наблюдаемой диагностики устройств. Репозиторий, пакет и проверка на конкретном устройстве — разные этапы: ниже указаны фактические платформы и публичные каналы.

| Проект | Назначение и платформа | Загрузка / исходники | Статус |
|---|---|---|---|
| **Deckivo** | PS5 Remote Play; Android ARM64, macOS Apple Silicon, подготовленная Switchroot Ubuntu ARM64 | [Сайт](https://remteh-by.github.io/remteh-remote-play/) · [Releases](https://github.com/remteh-by/remteh-remote-play/releases) · [Исходники](https://github.com/remteh-by/remteh-remote-play) | Опубликована 0.8.7 preview (Android 32, desktop 23), без физической приёмки. Для Ubuntu архив обновления не заменяет первую установку runtime |
| **X Play** | Xbox Remote Play launcher для macOS Apple Silicon | [Сайт](https://remteh-by.github.io/x-portal/) · [Releases](https://github.com/remteh-by/x-portal/releases) · [Исходники](https://github.com/remteh-by/x-portal) | Опубликована 1.2.0 preview с новым адаптивным интерфейсом и прозрачным фото геймпада; Mac ARM64, ad-hoc подпись. Игровая приёмка отдельно |
| **DualSense Tester** | Наблюдения Android InputDevice API, профиль DualSense | [Исходники и инструкции](https://github.com/remteh-by/dualsense-tester) · [Releases](https://github.com/remteh-by/dualsense-tester/releases) | Опубликован debug preview 1.2.0 / 3; это не обновление прежней release-установки |
| **Xbox Tester** | Аналогичная диагностика Android, профиль Xbox | [Исходники и инструкции](https://github.com/remteh-by/xbox-tester) · [Releases](https://github.com/remteh-by/xbox-tester/releases) | Опубликован debug preview 1.2.0 / 3; прежняя release-установка требует оригинального сертификата |
| **Joy-Con Tester** | Android, доступные оси/кнопки Joy-Con | [Исходники и инструкции](https://github.com/remteh-by/joycon-tester) · [Releases](https://github.com/remteh-by/joycon-tester/releases) | Опубликован debug preview 1.2.0 / 3; одиночный/парный режим и вибрация физически не приняты |
| **Mouse Tester** | Веб-инструмент: кнопки, колесо, события браузера, локальная история и отчёт | [Открыть онлайн](https://remteh-by.github.io/Mouse-Tester/) · [Исходники и запуск](https://github.com/remteh-by/Mouse-Tester) | Опубликованы production ZIP и исходники 1.2.0 preview; онлайн-версия доступна без установки, ИИ не подключён. Частота браузерных событий не равна USB polling rate |

Новые локальные прототипы: **RemTeh Device Lab** (общая модель наблюдений и просмотр отчётов) и **PhoneCheck Android** (приёмочная проверка телефона). Отдельный публичный релиз этих прототипов пока не заявлен. Учебный desktop-tutorial не является продуктом.

## Проверки и ограничения

Новые предварительные версии опубликованы по поручению владельца без физической приёмки. Выполнены сборки и автоматические проверки; Switch, PS5, Xbox и реальные контроллеры в этом выпуске не проверялись. Успешный тест кода или красивый экран не заменяет реальную проверку видео, звука, ввода, сна/пробуждения и обновления с сохранением данных.

Не обещаем нулевую задержку, 4K, любую Ubuntu, все Mac или универсальную аппаратную калибровку. Версии, архитектуры, контрольные суммы, сертификаты и инструкции относятся к конкретному файлу из Releases. Поддержка ведётся через репозитории проектов; не прикладывайте токены, пароли, регистрации консолей и данные клиентов к публичным обращениям.

## Лицензии

Deckivo — AGPL-3.0 с условиями upstream/OpenSSL; X Play — MIT; три Android-тестера имеют собственную proprietary-лицензию. У Mouse Tester новая лицензия от имени владельца не назначалась. Смотрите LICENSE/COPYING соответствующего проекта. Наличие исходников и пожертвование не меняют лицензию автоматически.

RemTeh — независимые проекты, не официальные приложения Sony, Microsoft или Nintendo. Кнопок покупки на несуществующие магазины здесь нет.

## Поддержка разработки

[Поддержать бесплатные инструменты RemTeh на Ko-fi](https://ko-fi.com/pavelzayats). Донат добровольный: все проверки доступны без оплаты. В новых приложениях ссылка есть в интерфейсе, а в тестерах — также после сохранения полезного отчёта.
