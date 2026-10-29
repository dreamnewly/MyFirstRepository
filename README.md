# Учебный проект по Git и GitHub

Небольшая программа на Python и рабочее пространство с практическими упражнениями курса по Git.

## Основной проект

- `main.py` — выводит приветствие на русском языке.
- `.gitignore` — исключает виртуальное окружение, кэш, временные файлы, настройки IDE и системные файлы.
- `requirements.txt` — сторонние зависимости не нужны.

## Запуск

```powershell
python main.py
```

Для локального окружения:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Каталог `.venv/` остаётся на компьютере и не отправляется в GitHub.

## Практические упражнения

Каждая практика находится в отдельной ветке GitHub; в ветке есть README на русском с описанием выполненных шагов.

- `praktika-2-5-navigatsiya` — `checkout`, `detached HEAD`, `old-version`, `reset`, `restore`, `revert`.
- `praktika-2-5-old-version` и `praktika-2-5-temp` — сохранённые состояния дополнительных веток из упражнения.
- `praktika-3-3-cherry-pick-rebase` — перенос коммита, переименование и объединение коммитов через интерактивный rebase.
- `praktika-3-3-feature-logging` — исходная ветка `feature-logging` до cherry-pick.
- `praktika-4-2-amend` — добавление `author.py` в последний коммит через `git commit --amend`.
- `praktika-4-4-tegi` — аннотированные теги `v1.0` и `v2.0`.
- `praktika-4-6-describe` — вывод `git describe --tags` для лёгкого тега `v1.0`.

Тег для практики 4.6 опубликован как `praktika-4-6-v1.0`, чтобы не пересекаться с тегом `v1.0` из практики 4.4. В README практики объяснено, почему с лёгким тегом нужен флаг `--tags`.