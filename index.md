---
layout: page
title: LAB
---

# 👋 Welcome!

Это сайт на **GitHub Pages**. Здесь вы найдёте информацию о проекте, полезные ссылки и подстраницы.

---

## 📂 Разделы

<div class="card">
  <h3>📘 О проекте</h3>
  <p>Узнайте больше о цели, функциях и развитии проекта.</p>
  <a href="index_1.html" class="button">Перейти</a>
</div>

<div class="card">
  <h3>📬 Контакты</h3>
  <p>Как со мной связаться, обратная связь и соцсети.</p>
  <a href="index_2.html" class="button">Перейти</a>
</div>

---

## 🖼 Галерея

![Пример изображения](img/example.jpg)

---

## 📌 Навигация

- [Главная](index.html)
- [О проекте](index_1.html)
- [Контакты](index_2.html)

---

## 📅 Обновления

- ✅ Добавлена разметка (24.06.2025)
- 🚧 В разработке новая подстраница: *index_3.md*

---

/* Общие стили для страницы */
body {
  font-family: 'Noto Sans', sans-serif; /* Google Font (не забудь подключить в <head>) */
  background-color: #f9f9f9;            /* Светло-серый фон */
  color: #333;                          /* Тёмно-серый текст */
  line-height: 1.6;                     /* Интерлиньяж для читаемости */
  margin: 0;
  padding: 0;
}

/* Основной контейнер статьи */
.post {
  max-width: 900px;                     /* Ширина контента */
  margin: 40px auto;                    /* Центрирование */
  padding: 0 20px;                      /* Отступы по бокам */
  background: #ffffff;                  /* Белый фон */
  box-shadow: 0 2px 4px rgba(0,0,0,0.05); /* Лёгкая тень */
  border-radius: 8px;                   /* Скругление углов */
}

/* Заголовок блока */
.post-header {
  border-bottom: 2px solid #e0e0e0;
  padding-bottom: 10px;
  margin-bottom: 20px;
}

/* Заголовок страницы */
.post-title {
  font-size: 2rem;
  font-weight: bold;
  color: #2c3e50;
}

/* Основной контент */
.post-content {
  font-size: 1rem;
  padding-bottom: 30px;
}

/* Ссылки */
a {
  color: #007acc;
  text-decoration: none;
  font-weight: 500;
}
a:hover {
  text-decoration: underline;
}

/* Кнопка */
.button {
  display: inline-block;
  margin: 12px 0;
  padding: 10px 18px;
  background-color: #007acc;
  color: white;
  border-radius: 6px;
  text-decoration: none;
  font-weight: bold;
}

/* Секции-карточки (если используешь) */
.card {
  background: #ffffff;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 20px;
  margin: 20px 0;
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
}

/* Списки */
ul {
  padding-left: 20px;
}

