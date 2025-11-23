# Швидкий старт

## Локальний запуск

1. Відкрийте `index.html` у браузері
2. Для повної функціональності потрібен локальний сервер (через CORS)

### Запуск через Python
```bash
python -m http.server 8000
```
Потім відкрийте http://localhost:8000

### Запуск через Node.js
```bash
npx http-server
```

## Деплой на Netlify

1. Завантажте проєкт на GitHub/GitLab
2. Увійдіть на [Netlify](https://app.netlify.com/)
3. Натисніть "New site from Git"
4. Оберіть ваш репозиторій
5. Налаштування:
   - Build command: (залиште порожнім)
   - Publish directory: `.` (крапка)
6. Натисніть "Deploy site"

## Налаштування CMS

1. Після деплою перейдіть на `your-site.netlify.app/admin`
2. У налаштуваннях Netlify:
   - Identity → Enable Identity
   - Identity → Services → Enable Git Gateway
3. Зареєструйтеся через `/admin`
4. Почніть додавати контент!

## Структура контенту

Всі файли контенту зберігаються в папці `content/`:
- `about/index.json` - інформація про дизайнера
- `services/index.json` - опис послуг
- `contacts/index.json` - контактна інформація
- `portfolio/` - папка з роботами (створюється через CMS)
- `tariffs/` - папка з тарифами (створюється через CMS)

## Важливо

- Після деплою на Netlify, всі зміни через CMS будуть автоматично зберігатися в вашому репозиторії
- Тільки авторизовані користувачі можуть редагувати контент
- Паролі зберігаються безпечно через Netlify Identity

