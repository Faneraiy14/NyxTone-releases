# NyxTone — збірки / builds

> **Бета-версія.** NyxTone ще в повному розпалі розробки: можливі помилки, можливості й формат проєктів змінюватимуться.
> Робіть копії важливих проєктів. / **Beta.** NyxTone is still under heavy development: expect bugs; features and the
> project format will change. Keep backups of important projects.

**NyxTone** — програма для створення музики: запис, інструменти, ефекти, мікшер, експорт.
Тут лише готові збірки (код програми закритий). Завантаження — у розділі **Releases** праворуч.

*NyxTone is a music-making app (recording, instruments, effects, mixer, export). This repository contains
builds only; the source code is closed. Downloads are under **Releases**.*

## Що завантажити / What to download

| Файл | Що це |
|---|---|
| `NyxTone-<версія>-windows-setup.exe` | Інсталятор для Windows 10/11 (64 біти): угода, ярлики, видалення через «Програми». |
| `NyxTone-<версія>-windows-portable.zip` | Та сама програма без встановлення: розпакуйте й запустіть `NyxTone.exe`. |
| `nyxtone_<версія>_amd64.deb` | Linux (Ubuntu 24.04+, Debian 13): `sudo apt install ./nyxtone_<версія>_amd64.deb`. Звук — PipeWire/JACK або ALSA. |
| `NyxTone-<версія>-nyxos.nyxapp` | NyxOS: відкрити у «Файлах» -> «Бібліотека» -> встановити. |
| `EULA.uk.txt`, `EULA.en.txt` | Угода користувача (її показує й сама програма під час першого запуску). |

## Вимоги / Requirements

- Windows 10 або 11, 64 біти; звукова карта з драйвером WASAPI (звичайна вбудована підходить).
- Linux: Ubuntu 24.04 / Debian 13 або новіші, 64 біти (пакет .deb тягне Qt 6, libsndfile, JACK, ALSA з системи).
- NyxOS: ядро NyxCore з підтримкою звуку для програм (nyx_audio).

## Угода / License

Програма розповсюджується за угодою користувача (EULA) — `EULA.uk.txt` / `EULA.en.txt` у кожному релізі.
Усі права застережені. Бібліотеки сторонніх авторів і їхні ліцензії — тека `licenses` і `THIRD_PARTY.txt` поруч із програмою.

*Distributed under the end-user license agreement (EULA) included with every release. All rights reserved.
Third-party libraries and their licenses are listed in the `licenses` folder next to the program.*

## Відомі межі / Known limits

Справжній звук, мікрофон і MIDI на Windows перевіряються на реальному ноутбуці; збірка й тести рушія
проходять автоматично (GitHub Actions) перед кожним релізом.

## Звідки ці збірки / Where builds come from

Кожен реліз збирає GitHub Actions з приватного репо програми, коли проходять тести (рушій, ефекти, інтерфейс,
встановлення .deb, збірка під NyxOS); сюди потрапляють лише готові файли й угода.
*Every release is built by GitHub Actions from the private source repo after the tests pass; only the finished files
and the agreement are published here.*
