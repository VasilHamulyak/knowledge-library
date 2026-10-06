# Modern Zero-Shot Prompting Techniques

## Що це таке?

Сучасні Zero-Shot Prompting Techniques — це техніки покращення якості відповідей LLM без використання прикладів (few-shot examples).

Вони допомагають підвищити точність, логічність та якість міркувань моделі за рахунок спеціального формулювання інструкцій.

---

## 1. Emotion Prompting

### Ідея

Використання емоційних стимулів у prompt.

### Приклад

"This is very important for my career. Please analyze this code carefully."

### Переваги

- Покращує уважність моделі.
- Часто підвищує якість відповідей.
- Корисно для складних задач.

### Використання

- Code Review
- Medical Analysis
- Legal Analysis
- Critical Decision Making

---

## 2. Re-Reading (RE2)

### Ідея

Попросити модель перечитати завдання перед відповіддю.

### Приклад

"Read the question carefully. Then read it again before answering."

### Переваги

- Менше пропущених деталей.
- Краща робота зі складними вимогами.

### Використання

- Довгі інструкції
- Технічні специфікації
- Бізнес-вимоги

---

## 3. Rephrase and Respond (RaR)

### Ідея

Модель спочатку перефразовує задачу, а потім відповідає.

### Приклад

"First rephrase the question. Then answer it."

### Переваги

- Зменшує неоднозначність.
- Покращує розуміння задачі.

### Використання

- Аналіз вимог
- Архітектурні рішення
- User Stories

---

## 4. Role Prompting

### Ідея

Призначення моделі конкретної ролі.

### Приклад

"You are a Senior Software Architect."

### Переваги

- Більш релевантні відповіді.
- Експертний контекст.

### Використання

- Software Architecture
- Content Writing
- Business Consulting

---

## 5. System 2 Attention (S2A)

### Ідея

Виділити релевантну інформацію перед відповіддю.

### Приклад

"Identify relevant information. Ignore distractions. Then answer."

### Переваги

- Зменшує вплив шуму.
- Покращує точність.

### Використання

- RAG Systems
- Юридичні документи
- Великі специфікації

---

## 6. SimToM (Simulation Theory of Mind)

### Ідея

Попросити модель подивитися на проблему з точки зору іншої людини.

### Приклад

"Answer from the perspective of a customer."

### Переваги

- Покращує stakeholder analysis.
- Допомагає в user research.

### Використання

- Product Discovery
- UX Research
- Бізнес-аналіз

---

## Порівняння технік

| Technique | Основна ціль |
|------------|------------|
| Emotion Prompting | Покращення уваги |
| Re-Reading | Зменшення пропуску деталей |
| Rephrase and Respond | Усунення неоднозначності |
| Role Prompting | Експертний контекст |
| System 2 Attention | Фільтрація шуму |
| SimToM | Аналіз перспективи іншої людини |

---

## Найбільш корисні техніки для AI Agents

⭐⭐⭐⭐⭐ Role Prompting

⭐⭐⭐⭐⭐ Rephrase and Respond

⭐⭐⭐⭐⭐ System 2 Attention

⭐⭐⭐⭐⭐ Task Decomposition

⭐⭐⭐⭐ Re-Reading

⭐⭐⭐ Emotion Prompting

⭐⭐⭐ SimToM

---

## Рекомендована комбінація

Для сучасних AI Agent систем:

Role Prompting
+
Rephrase and Respond
+
System 2 Attention
+
Task Decomposition

---

## Головна думка

Сучасні Zero-Shot Prompting Techniques дозволяють значно покращити результати LLM без використання прикладів, використовуючи ролі, перефразування, повторне читання, фільтрацію шуму та аналіз перспективи користувача.
