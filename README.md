# Опционы — учебный тренажёр

Обучающее веб-приложение (уроки, лаборатория, тесты).  
Не магазин сигналов и не брокерский сервис. Аккаунты хранятся в браузере устройства.

## Открыть в браузере

После включения GitHub Pages ссылка будет такой:

`https://ВАШ_ЛОГИН.github.io/ИМЯ_РЕПОЗИТОРИЯ/`

Файл сайта: `index.html`.

## Скачать APK (Android)

Файл: `Options-s-nulya-MVP.apk`  
На телефоне: скачать → разрешить установку из этого источника → установить.

iPhone этот APK не ставит — только сайт в Safari.

---

## Как залить на GitHub (без своего сервера и домена)

### 1. Репозиторий

1. Войдите на [github.com](https://github.com).
2. **New repository**.
3. Имя, например: `options-trainer`.
4. Public.
5. **не** ставьте галочку «Add a README» — файлы уже готовы.
6. Create repository.

### 2. Загрузить эти файлы

На странице пустого репозитория: **uploading an existing file**  
перетащите из папки `options-github`:

- `index.html`
- `README.md`
- `Options-s-nulya-MVP.apk`

Commit changes.

Либо в терминале (подставьте логин и имя репо):

```bash
cd options-github
git init
git add index.html README.md Options-s-nulya-MVP.apk
git commit -m "Учебный тренажёр опционов"
git branch -M main
git remote add origin https://github.com/ВАШ_ЛОГИН/options-trainer.git
git push -u origin main
```

GitHub спросит не пароль аккаунта, а **Personal Access Token**  
(Settings → Developer settings → Personal access tokens → Fine-grained или classic, право `repo`).

### 3. Включить сайт (GitHub Pages) — бесплатно

1. Репозиторий → **Settings** → **Pages**.
2. Source: **Deploy from a branch**.
3. Branch: `main`, папка: `/ (root)`.
4. Save.

Через 1–2 минуты:  
`https://ВАШ_ЛОГИН.github.io/options-trainer/`

### 4. APK для скачивания

Тот же файл в репозитории:

`https://github.com/ВАШ_ЛОГИН/options-trainer/blob/main/Options-s-nulya-MVP.apk`

Кнопка **Download**.  
Или **Releases** → Draft a new release → приложить APK.

Домен и VPS не нужны. Свой домен — по желанию позже в Settings → Pages → Custom domain.
