# MKDK Docs IT

<p align="center">
  <img src="assets/mkdk-logo.png" alt="Логотип Московского колледжа деловой карьеры" width="180">
</p>

<h2 align="center">Документация IT-департамента МКДК</h2>

<p align="center">
  Единый каталог для описания инфраструктуры, серверов, домена, оборудования и рабочих инструкций IT-департамента.
</p>

<p align="center">
  <strong>Московский колледж деловой карьеры</strong><br>
  Нижегородская 32СБ, Москва<br>
  <a href="https://mkdk-studsovet.ru">mkdk-studsovet.ru</a>
</p>

---

## Быстрый старт

Этот репозиторий нужен, чтобы участники IT-департамента могли быстро понять:

- какие серверы используются;
- где смотреть инвентаризацию оборудования;
- как устроен домен `MKDK`;
- какие работы уже выполнены;
- какие задачи ещё в плане;
- как выполнять типовые действия;
- где находится актуальный журнал работ.

Основной источник табличных данных:

```text
it-templates_2026_04_06.xlsx
```

Markdown-файлы используются для описания, навигации и инструкций. Таблицы остаются в Excel-файле.

---

## Команда

Документацию и инфраструктурные работы ведут:

<div align="center">

**Бадретдинов Даниил** · **Набоков Родион** · **Литвинов Илья** · **Митин Тигран**

</div>

---

## Основные разделы

- [`overview.md`](overview.md) — общий обзор инфраструктуры колледжа.
- [`inventory.md`](inventory.md) — инвентаризация оборудования и правила учёта.
- [`network.md`](network.md) — сеть, VLAN, Wi-Fi и IP-план.
- [`servers.md`](servers.md) — физический сервер, Proxmox и виртуальная машина.
- [`active-directory.md`](active-directory.md) — домен `MKDK`, OU, группы и пользователи.
- [`backup.md`](backup.md) — план настройки резервного копирования.
- [`security.md`](security.md) — безопасность, доступы и текущие риски.
- [`student-council-site.md`](student-council-site.md) — сайт [`mkdk-studsovet.ru`](https://mkdk-studsovet.ru).
- [`work-log.md`](work-log.md) — журнал работ IT-департамента.

---

## Инструкции

- [`runbooks/equipment-inventory.md`](runbooks/equipment-inventory.md) — проведение инвентаризации.
- [`runbooks/join-pc-to-domain.md`](runbooks/join-pc-to-domain.md) — подключение ПК к домену.
- [`runbooks/add-new-user.md`](runbooks/add-new-user.md) — создание пользователя.
- [`runbooks/backup-setup-plan.md`](runbooks/backup-setup-plan.md) — настройка резервного копирования.
- [`runbooks/clonezilla-deploy-images.md`](runbooks/clonezilla-deploy-images.md) — развёртывание образов через Clonezilla.
- [`runbooks/restore-backup.md`](runbooks/restore-backup.md) — восстановление из резервной копии.
- [`runbooks/work-log-rules.md`](runbooks/work-log-rules.md) — правила заполнения журнала работ.

---

## Структура репозитория

```text
mkdk-docs-it/
├── README.md
├── overview.md
├── repository-map.md
├── inventory.md
├── network.md
├── servers.md
├── active-directory.md
├── backup.md
├── security.md
├── student-council-site.md
├── work-log.md
├── assets/
│   └── README.md
└── runbooks/
    ├── equipment-inventory.md
    ├── join-pc-to-domain.md
    ├── add-new-user.md
    ├── backup-setup-plan.md
    ├── clonezilla-deploy-images.md
    ├── restore-backup.md
    └── work-log-rules.md
```

---

## Текущий статус

На основе актуального Excel-файла зафиксировано:

- оборудования в учёте: 17 записей;
- ПК: 13;
- проекторов: 1;
- устройств на ремонте: 2;
- серверы и виртуальные машины: 2;
- записей в журнале работ: 16;
- домен Active Directory: `MKDK`;
- сайт колледжа: [`mkdk-studsovet.ru`](https://mkdk-studsovet.ru).

---

## Ближайшие задачи

Планируется:

- привести инвентаризацию по кабинетам к единому виду;
- дополнить и проверить данные по кабинетам 313, 315, 509, 514 и 515;
- уточнить IP-план и VLAN;
- завершить настройку Active Directory;
- создать и описать файловый сервер;
- настроить групповые политики;
- подготовить эталонные образы и развёртывание через Clonezilla;
- настроить резервное копирование;
- проверить восстановление из резервной копии;
- обновлять журнал работ после каждого изменения.

---

## Правила работы с документацией

После каждого изменения инфраструктуры нужно обновлять:

1. соответствующий Markdown-файл;
2. Excel-файл с табличными данными;
3. журнал работ.

Markdown нужен для объяснений и инструкций. Excel нужен для списков, учёта и журналов.

---

## Что нельзя хранить в репозитории

В репозитории нельзя хранить:

- пароли;
- временные пароли;
- токены;
- приватные ключи;
- доступы к хостингу;
- доступы к серверу;
- доступы к Proxmox;
- дампы баз данных;
- резервные копии;
- лишние персональные данные.

Секретные данные должны храниться отдельно в защищённом хранилище.

---

<p align="center">
  <strong>MKDK Docs IT</strong><br>
  Рабочая документация IT-департамента · <a href="https://mkdk-studsovet.ru">mkdk-studsovet.ru</a>
</p>
