# DirectDrop

Прямая зашифрованная передача файлов между устройствами: файлы и папки, drag and drop, докачка, проверка BLAKE3 и автоматическое сжатие. Файлы и их метаданные идут только напрямую.

## Скачать 0.8.0

| Платформа | Скачать |
| --- | --- |
| **Windows 10/11 x64** | [Установщик EXE](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.8.0/DirectDrop-Setup-0.8.0.exe) · [Portable ZIP](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.8.0/DirectDrop-0.8.0-win-x64.zip) |
| **Android ARM64** | [APK — экспериментальная версия](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.8.0/DirectDrop-Android-0.8.0-arm64.apk) |
| **iPhone / iPad** | Пока исходники: нужны Mac и подпись Apple. Готового IPA нет. |
| **Linux / macOS** | Готовые пакеты пока не выпущены. |
| **Исходный код** | [Полный DirectDrop-Source-0.8.0.zip](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.8.0/DirectDrop-Source-0.8.0.zip) |

[Релиз 0.8.0 и изменения](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/tag/v0.8.0) · [Контрольные суммы](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.8.0/SHA256SUMS.txt)

Перетащите файлы или папку в Windows, создайте передачу и передайте код получателю через доверенный канал. На Android можно сканировать QR; пока держите приложение открытым. Физические телефоны, камеры и фоновые передачи этой версии не проверены.

В 0.8.0 обновлён интерфейс Windows. Экспериментальный обмен проверенными блоками между получателями включается в настройках у участников 0.8.0; он пока работает без сжатия. Стандартный режим со сжатием остаётся режимом по умолчанию. Helpers без кода ещё не реализованы.

По умолчанию — X25519 + ML-KEM-768 / AES-256-GCM, без тихого понижения защиты. Прямое подключение зависит от NAT, UDP и сети провайдеров; при невозможности прямого маршрута файлы через публичный relay не пересылаются. Скорость WAN не гарантируется.

Локальные диагностики Windows включены по умолчанию, отключаются в настройках и автоматически никуда не отправляются. Имена/пути файлов, содержимое, коды и IP в них не записываются.

Для разработчиков: полный код Windows, Flutter Android/iOS, Rust-движок, тесты, лицензии и границы проверок находятся в **полном source ZIP** выше. Автоматические GitHub-архивы «Source code» этой страницы содержат только материалы страницы, а не полный движок.
