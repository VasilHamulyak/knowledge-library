# LangChain

## Що таке LangChain
LangChain — це framework для створення AI-додатків на базі LLM.

Він допомагає:
- працювати з LLM,
- будувати AI workflow,
- підключати пам’ять,
- використовувати RAG,
- викликати tools та API,
- створювати AI агентів.

---

# Основні компоненти

## LLM
Модель генерації тексту:
- OpenAI
- Anthropic
- Gemini
- локальні моделі

---

## Prompt Templates
Шаблони для побудови prompt.

Приклад:

```python
template = "Explain {topic}"
```

---

## Chains
Ланцюжок кроків.

Наприклад:
1. Отримати питання
2. Знайти контекст
3. Передати в LLM
4. Повернути відповідь

---

## Memory
Збереження контексту розмови.

Типи:
- ConversationBufferMemory
- SummaryMemory
- Vector Memory

---

## Document Loaders
Завантаження:
- PDF
- DOCX
- HTML
- GitHub repo
- Notion
- Database

---

## Text Splitters
Розбиття великих документів на chunks.

---

## Embeddings
Перетворення тексту у vectors для semantic search.

---

## Vector Databases
Зберігання embeddings:
- Pinecone
- Qdrant
- Weaviate
- pgvector

---

## Retrievers
Пошук релевантних chunks.

---

## RAG
Retrieval-Augmented Generation:
1. Пошук документів
2. Додавання контексту
3. Генерація відповіді

---

## Agents
AI, який:
- думає,
- вибирає tools,
- виконує дії.

---

# Приклад RAG flow

```text
User Question
    ↓
Retriever
    ↓
Vector DB
    ↓
Relevant Chunks
    ↓
LLM
    ↓
Answer
```

---

# Коли використовувати LangChain

Підходить для:
- AI chatbot,
- knowledge base,
- AI support,
- AI code assistant,
- AI workflow,
- document search,
- internal company AI.

---

# Мінуси
- інколи overengineering,
- abstraction може ускладнювати debug,
- прості задачі можна реалізувати без LangChain.

---

# Альтернативи
- LangGraph
- LlamaIndex
- Haystack
- Semantic Kernel