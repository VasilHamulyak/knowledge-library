# Chain-of-Thought Prompting

## Що таке Chain-of-Thought Prompting?

Chain-of-Thought Prompting (CoT) — це техніка Prompt Engineering, у якій модель стимулюється розв’язувати задачу через послідовні логічні кроки.

Замість того щоб одразу давати фінальну відповідь, модель спочатку структурує міркування, аналізує проміжні етапи та поступово приходить до висновку.

---

## Основна ідея

Замість:

Question
→ Answer

використовується:

Question
→ Reasoning Steps
→ Answer

---

## Простий приклад

### Звичайний prompt

"Який варіант архітектури краще для маркетплейсу?"

### Chain-of-Thought prompt

"Проаналізуй задачу крок за кроком:
1. Визнач вимоги.
2. Оціни складність домену.
3. Порівняй архітектурні варіанти.
4. Дай фінальну рекомендацію."

---

## Для чого використовується

### Reasoning Tasks

- Логічні задачі
- Математичні задачі
- Аналіз причин і наслідків
- Прийняття рішень

### Software Engineering

- System Design
- Code Review
- Debugging
- Refactoring
- Architecture Decisions

### Business Analysis

- Аналіз ризиків
- Пріоритизація
- Вибір стратегії
- Порівняння варіантів

---

## Основні види Chain-of-Thought

### 1. Zero-Shot Chain-of-Thought

Модель просять мислити покроково без прикладів.

Приклад:

"Think step by step before answering."

---

### 2. Few-Shot Chain-of-Thought

Моделі дають приклади, де показані кроки міркування.

Формат:

Question
→ Reasoning
→ Answer

Question
→ Reasoning
→ Answer

New Question
→ Reasoning
→ Answer

---

### 3. Structured Chain-of-Thought

Кроки міркування задаються явно.

Приклад:

1. Analyze requirements.
2. Identify constraints.
3. Compare options.
4. Recommend solution.

---

### 4. Domain-Specific Chain-of-Thought

Кроки адаптовані під конкретний домен.

Приклад для архітектури:

1. Domain complexity
2. Data consistency
3. Scalability
4. Deployment complexity
5. Maintainability

---

## Переваги

- Покращує якість reasoning.
- Зменшує ризик поспішної відповіді.
- Допомагає розв’язувати складні задачі.
- Робить відповідь більш структурованою.
- Корисно для аналізу trade-offs.

---

## Недоліки

- Відповіді стають довшими.
- Може збільшувати вартість через більшу кількість токенів.
- Не завжди потрібен для простих задач.
- Модель може створювати переконливі, але помилкові проміжні кроки.

---

## Best Practices

### Використовуйте для складних задач

CoT найбільш корисний, коли потрібно:
- аналізувати;
- порівнювати;
- планувати;
- приймати рішення.

### Задавайте структуру

Краще не просто писати:

"Think step by step."

Краще:

"Проаналізуй:
1. Вимоги
2. Обмеження
3. Ризики
4. Варіанти
5. Рекомендацію"

### Просіть фінальний висновок

Після аналізу варто явно попросити:

"Наприкінці дай коротку фінальну рекомендацію."

### Не використовуйте для простих фактів

Для простого питання краще короткий direct prompt.

---

## Chain-of-Thought vs Step-Back Prompting

### Chain-of-Thought

Фокус на послідовному розв’язанні задачі.

Question
→ Steps
→ Answer

### Step-Back Prompting

Фокус на загальному принципі перед відповіддю.

Question
→ General Principle
→ Apply Principle
→ Answer

---

## Chain-of-Thought в AI Agents

CoT корисний для агентів, які виконують складні багатоетапні задачі:

- Planning Agent
- Research Agent
- Architecture Agent
- Reviewer Agent
- Debugging Agent
- Business Analyst Agent

Агент може використовувати CoT для:
- планування;
- оцінки варіантів;
- перевірки рішень;
- аналізу помилок.

---

## Приклад prompt-а для Software Architecture

Ти Senior Software Architect.

Задача:
Ми будуємо marketplace platform.

Проаналізуй рішення крок за кроком:

1. Визнач ключові бізнес-вимоги.
2. Визнач технічні обмеження.
3. Порівняй Monolith, Modular Monolith і Microservices.
4. Опиши trade-offs.
5. Дай фінальну рекомендацію.

Формат відповіді:
- Аналіз
- Варіанти
- Trade-offs
- Рекомендація
- Ризики

---

## Головна думка

Chain-of-Thought Prompting допомагає AI розв’язувати складні задачі через послідовний аналіз. Це робить відповіді більш логічними, структурованими та корисними для технічних, бізнесових і стратегічних рішень.
