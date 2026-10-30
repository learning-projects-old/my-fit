# Путеводитель: my-fit

Автономная инструкция: достаточно этой папки, исходников и перечисленных защищённых копий. История чатов и центральный каталог не требуются.

[Восстановление](RECOVERY.md) · [Карта файлов и зависимостей](PROJECT_MAP.json)

## Назначение

По [package.json](package.json): Fitness tracker app

Обнаруженные языки: JavaScript, TypeScript, Vue SFC.

## Порядок чтения

1. Локальные AGENTS.md / CLAUDE.md и документы ниже.
2. Манифесты: версии среды, зависимости, команды.
3. Кандидаты точек входа; фактический запуск проверить по манифесту.
4. PROJECT_MAP.json: imports_local от источника к импортируемому файлу; входящие рёбра — потребители модуля.
5. RECOVERY.md: независимые данные, восстановление среды, запуск и критерии приёмки.

- [README.md](README.md)

## Манифесты

- [package.json](package.json)
- [apps/app/package.json](apps/app/package.json)
- [apps/backend/package.json](apps/backend/package.json)

## Кандидаты точек входа


## Основные файлы по локальным импортам

| Файл | Входящих импортов |
|---|---:|
| [apps/backend/src/interface/index.ts](apps/backend/src/interface/index.ts) | 8 |
| [apps/backend/src/models/exercise.ts](apps/backend/src/models/exercise.ts) | 2 |
| [apps/backend/src/helpers/index.ts](apps/backend/src/helpers/index.ts) | 2 |
| [apps/backend/src/models/user.ts](apps/backend/src/models/user.ts) | 2 |
| [apps/app/src/App.vue](apps/app/src/App.vue) | 1 |
| [apps/backend/src/app.ts](apps/backend/src/app.ts) | 1 |
| [apps/backend/src/helpers/decodeToken.ts](apps/backend/src/helpers/decodeToken.ts) | 1 |
| [apps/backend/src/helpers/paginate.ts](apps/backend/src/helpers/paginate.ts) | 1 |
| [apps/backend/src/helpers/date.ts](apps/backend/src/helpers/date.ts) | 1 |
| [apps/backend/src/services/activity.ts](apps/backend/src/services/activity.ts) | 1 |
| [apps/backend/src/services/auth.ts](apps/backend/src/services/auth.ts) | 1 |
| [apps/backend/src/services/exercise.ts](apps/backend/src/services/exercise.ts) | 1 |

## Проверки


## Чтение карты без специальных плагинов

PROJECT_MAP.json — UTF-8 JSON: nodes и edges. Пути файлов относительные. contains обозначает наличие файла; imports_local — статически распознанный импорт; declares_dependency — объявление пакета в манифесте. evidence содержит источник и, где доступно, строку. Карта не исполняет код.

Статус исходного анализа: static-scan-complete; ограничений чтения: 0. Исходный снимок: 2026-10-30T14:47:11.360Z.

После изменения кода перечитайте затронутые файлы: карта является снимком. Отсутствие ребра не доказывает отсутствие зависимости.
