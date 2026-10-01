# ОГЭ по математике — GitHub Pages

Готовый статический сайт из двух страниц:

- `site/index.html` — главная и тренировка;
- `site/tasks.html` — банк задач;
- `.github/workflows/deploy-pages.yml` — автоматическая публикация в GitHub Pages.

## Как опубликовать

1. Создайте новый репозиторий на GitHub.
2. Загрузите **всё содержимое этой папки**, включая скрытую папку `.github`.
3. Убедитесь, что основная ветка называется `main`.
4. В GitHub откройте **Settings → Pages**.
5. В разделе **Build and deployment → Source** выберите **GitHub Actions**.
6. Сделайте push/commit в `main` (или запустите workflow вручную во вкладке **Actions**).
7. После успешного workflow ссылка на сайт появится в deployment `github-pages` и в **Settings → Pages**.

## Структура

```text
.
├── .github/
│   └── workflows/
│       └── deploy-pages.yml
├── site/
│   ├── index.html
│   └── tasks.html
└── README.md
```

Сайт не требует Node.js, npm или сборки: GitHub Actions публикует содержимое `site/` как статический сайт.
