# Lisa Ulianova — Portfolio Website

Static HTML/CSS website based on Figma design. Ready to deploy on GitHub + Vercel.

---

## Файлы сайта

```
index.html          — главная страница (портфолио)
cv.html             — страница CV
megamarket.html     — кейс Megamarket
avito.html          — кейс Avito
viju-streaming.html — кейс VIJU (стриминг)
viju-cms.html       — кейс VIJU (CMS)
brag-house.html     — кейс Brag House
sbermarket.html     — кейс Sbermarket
styles.css          — все стили
images/             — папка для изображений (добавь сюда PNG/JPG из Figma)
```

---

## Как задеплоить: шаг за шагом

### Шаг 1 — Загрузи файлы на GitHub

1. Зайди на [github.com](https://github.com) → **New repository**
2. Название: `portfolio` (или любое другое)
3. Поставь **Public** (Vercel бесплатно работает с публичными репо)
4. Нажми **Create repository**
5. Загрузи все файлы:
   - Нажми **uploading an existing file**
   - Перетащи все файлы из этой папки (включая `styles.css`)
   - Нажми **Commit changes**

---

### Шаг 2 — Подключи Vercel

1. Зайди на [vercel.com](https://vercel.com) → **Sign up with GitHub**
2. После входа нажми **Add New → Project**
3. Найди свой репозиторий `portfolio` → нажми **Import**
4. Настройки оставь по умолчанию (Framework: Other, root directory: `/`)
5. Нажми **Deploy**

Через 30 секунд сайт будет доступен по адресу вида `https://portfolio-xxx.vercel.app`

---

### Шаг 3 — Подвязать свой домен

1. В Vercel зайди в свой проект → вкладка **Settings → Domains**
2. Введи свой домен, например `lisa.design` → **Add**
3. Vercel покажет DNS-записи (обычно два варианта: A-запись или CNAME)
4. Зайди к своему регистратору домена (где купила домен — Namecheap, GoDaddy, RU-CENTER и т.д.)
5. В DNS-настройках добавь записи, которые показал Vercel:
   - **Вариант A**: добавь `A record` → `76.76.21.21`
   - **Вариант B**: добавь `CNAME record` → `cname.vercel-dns.com`
6. Подожди 5–30 минут (иногда до 24 часов) — DNS обновится
7. Vercel автоматически выпустит SSL-сертификат (https будет работать сразу)

---

### Как обновлять сайт после деплоя

Просто загрузи обновлённые файлы в GitHub-репозиторий — Vercel автоматически задеплоит новую версию через ~30 секунд.

---

## Как добавить изображения из Figma

1. В Figma выдели нужный элемент (mockup, скриншот приложения)
2. В правом панели → **Export → PNG** → нажми Export
3. Назови файл: `megamarket.png`, `avito.png` и т.д.
4. Положи в папку `images/` рядом с остальными файлами
5. Загрузи папку `images/` в GitHub

Файлы подключены в HTML автоматически — если изображений нет, карточки просто покажутся без картинки.
