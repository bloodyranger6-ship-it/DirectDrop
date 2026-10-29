# DirectDrop

Прямая зашифрованная передача файлов между друзьями: папки, drag and drop, докачка, проверка BLAKE3 и автоматическое сжатие. Файлы и их метаданные идут только напрямую.

## Скачать 0.7.0

| Платформа | Скачать |
| --- | --- |
| **Windows 10/11 x64** | [Установщик EXE](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.7.0/DirectDrop-Setup-0.7.0.exe) · [Portable ZIP](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.7.0/DirectDrop-0.7.0-win-x64.zip) |
| **Android ARM64** | [APK — экспериментальная версия](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.7.0/DirectDrop-Android-0.7.0-arm64.apk) |
| **iPhone / iPad** | Пока исходники: нужны Mac и подпись Apple. Готового IPA нет. |
| **Linux / macOS** | Готовые пакеты пока не выпущены. |
| **Исходный код** | [Полный DirectDrop-Source-0.7.0.zip](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.7.0/DirectDrop-Source-0.7.0.zip) |

[Все релизы и описание изменений](https://github.com/bloodyranger6-ship-it/DirectDrop/releases) · [Контрольные суммы](https://github.com/bloodyranger6-ship-it/DirectDrop/releases/download/v0.7.0/SHA256SUMS.txt)

Обновите обе стороны до 0.7 для сжатия. В Windows перетащите файлы или папку, создайте передачу и передайте код другу через доверенный канал. На телефоне можно сканировать QR; пока держите мобильное приложение открытым. Физические телефоны и фоновые передачи ещё не проверены.

По умолчанию — X25519 + ML-KEM-768 / AES-256-GCM, без тихого понижения защиты. Сжатие отключается отдельно. Передача не требует предварительного ZIP: уже сжатые данные могут не уменьшиться.

Прямое подключение зависит от NAT, UDP и сети провайдеров; при невозможности прямого маршрута файлы через сервер не пересылаются. Скорость WAN не гарантируется.

Для разработчиков: полный код Windows, Flutter Android/iOS, Rust-движок, тесты, лицензии и ограничения проверок находятся в **полном source ZIP** выше. Автоматические GitHub-архивы «Source code» этой страницы содержат только материалы страницы, а не полный движок.
