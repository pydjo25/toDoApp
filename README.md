<div align="center">

# 📝 **Todo App** - Умный планировщик задач

![Todo App Banner](https://via.placeholder.com/800x200/4F46E5/FFFFFF?text=Todo+App+-+Smart+Task+Management)
*Визуальное представление интерфейса приложения*

[![Go Version](https://img.shields.io/badge/Go-1.21+-00ADD8?style=for-the-badge&logo=go&logoColor=white)](https://golang.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Docker](https://img.shields.io/badge/Docker-✓-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docker.com)
[![JWT Auth](https://img.shields.io/badge/JWT-Auth-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)](https://jwt.io)

</div>

## 🚀 **О проекте**

<div align="center">

![Workflow](https://via.placeholder.com/700x300/1F2937/FFFFFF?text=Create+→+Schedule+→+Repeat+→+Complete)

</div>

**Todo App** — это современное веб-приложение для управления задачами с интеллектуальной поддержкой повторяющихся событий. Приложение сочетает в себе простоту использования и мощные функции автоматизации.

### 🎯 **Ключевые возможности**

<table>
<tr>
<td width="33%">

#### 📅 **Повторяющиеся задачи**
- Ежедневные
- Еженедельные  
- Ежемесячные
- Ежегодные
- Противоположные дни

</td>
<td width="33%">

#### 🔒 **Безопасность**
- JWT аутентификация
- Защищенные маршруты
- Переменные окружения
- Docker-контейнеризация

</td>
<td width="33%">

#### 🔍 **Умный поиск**
- Поиск по тексту
- Фильтрация по дате
- Расширенная фильтрация
- Быстрый доступ

</td>
</tr>
</table>

## 🛠 **Архитектура проекта**

```mermaid
graph TB
    A[Пользователь] --> B[Веб-интерфейс]
    B --> C[JWT Middleware]
    C --> D[Task Service]
    D --> E[Database SQLite]
    D --> F[Recurrence Engine]
    
    G[Docker] --> H[Application]
    I[Environment Variables] --> H
    
    style A fill:#4F46E5,color:#fff
    style H fill:#10B981,color:#fff
