# RMRP Rules Site

Статический сайт с правилами сервера. Чистый HTML/CSS/JS, без сборки.

## Публикация на GitHub Pages

1. Создайте репозиторий на GitHub.
2. Загрузите `index.html` и `README.md` в корень.
3. Settings → Pages → Source: **Deploy from a branch** → Branch: `main` / `root`.
4. Через минуту сайт будет доступен по адресу `https://<username>.github.io/<repo>/`.

## Как пользоваться

- Верхний поиск: `1.20 ПГО`, `рейд`, `PG`, `допрос`, `1.8`.
- Кнопки-главы — быстрый переход.
- `Ctrl+K` — фокус на поиске.

## Как добавить/изменить правило

Откройте `index.html`, найдите `const DATA = [...]` и добавьте объект:

```js
{
  id: "my-chapter",            // уникальный id
  title: "Моя глава",
  rules: [
    { num: "1.1", text: "Текст правила.", punish: "Warn", note: "Примечание (необязательно)" }
  ]
}
