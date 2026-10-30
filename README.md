# RemTeh · приложения и инструменты

Развиваем приложения для Remote Play и наблюдаемой диагностики устройств. Репозиторий, пакет и проверка на конкретном устройстве — разные этапы: ниже указаны фактические платформы и публичные каналы.

| Проект | Назначение и платформа | Загрузка / исходники | Статус |
|---|---|---|---|
| **Deckivo** | PS5 Remote Play; Android ARM64, macOS Apple Silicon, подготовленная Switchroot Ubuntu ARM64 | [Сайт](https://remteh-by.github.io/remteh-remote-play/) · [Releases](https://github.com/remteh-by/remteh-remote-play/releases) · [Исходники](https://github.com/remteh-by/remteh-remote-play) | Публичная 0.8.6 preview; 0.8.7 — отдельный кандидат. Для Ubuntu архив обновления не заменяет первую установку runtime |
| **X Play** | Xbox Remote Play launcher для macOS Apple Silicon | [Сайт](https://remteh-by.github.io/x-portal/) · [Releases](https://github.com/remteh-by/x-portal/releases) · [Исходники](https://github.com/remteh-by/x-portal) | Публичная 1.0.0 устарела; 1.1.0 — кандидат с исправлениями ввода и профилями. Игровая приёмка отдельно |
| **DualSense Tester** | Наблюдения Android InputDevice API, профиль DualSense | [Исходники и инструкции](https://github.com/remteh-by/dualsense-tester) · [Releases](https://github.com/remteh-by/dualsense-tester/releases) | Кандидат 1.1.0; опубликованный APK и сертификат обновления проверяются по конкретному выпуску |
| **Xbox Tester** | Аналогичная диагностика Android, профиль Xbox | [Исходники и инструкции](https://github.com/remteh-by/xbox-tester) · [Releases](https://github.com/remteh-by/xbox-tester/releases) | Публичная 1.0.0; 1.1.0 — кандидат. Android API не гарантирует все аппаратные функции |
| **Joy-Con Tester** | Android, доступные оси/кнопки Joy-Con | [Исходники и инструкции](https://github.com/remteh-by/joycon-tester) · [Releases](https://github.com/remteh-by/joycon-tester/releases) | Кандидат 1.1.0; одиночный/парный режим и вибрация требуют проверки устройства и транспорта |
| **Mouse Tester** | Веб-инструмент: кнопки, колесо, события браузера, локальная история и отчёт | [Исходники и запуск](https://github.com/remteh-by/Mouse-Tester) | 1.1.0 — кандидат; публичный production-деплой не заявлен. Частота браузерных событий не равна USB polling rate |

Новые локальные прототипы: **RemTeh Device Lab** (общая модель наблюдений и просмотр отчётов) и **PhoneCheck Android** (приёмочная проверка телефона). Отдельный публичный релиз этих прототипов пока не заявлен. Учебный desktop-tutorial не является продуктом.

## Проверки и ограничения

Для новых кандидатов выполнены доступные сборки и автоматические проверки. Проверку на Switch, PS5, Xbox и физических контроллерах владелец перенёс на следующий этап. Успешный тест кода или красивый экран не заменяет реальную проверку видео, звука, ввода, сна/пробуждения и обновления с сохранением данных.

Не обещаем нулевую задержку, 4K, любую Ubuntu, все Mac или универсальную аппаратную калибровку. Версии, архитектуры, контрольные суммы, сертификаты и инструкции относятся к конкретному файлу из Releases. Поддержка ведётся через репозитории проектов; не прикладывайте токены, пароли, регистрации консолей и данные клиентов к публичным обращениям.

## Лицензии

Deckivo — AGPL-3.0 с условиями upstream/OpenSSL; X Play — MIT; три Android-тестера имеют собственную proprietary-лицензию. У Mouse Tester новая лицензия от имени владельца не назначалась. Смотрите LICENSE/COPYING соответствующего проекта. Наличие исходников и пожертвование не меняют лицензию автоматически.

RemTeh — независимые проекты, не официальные приложения Sony, Microsoft или Nintendo. Кнопок покупки на несуществующие магазины здесь нет.
