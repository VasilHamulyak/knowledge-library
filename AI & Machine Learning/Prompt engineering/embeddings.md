# Embeddings

Embedding — це числове представлення тексту або даних, яке зберігає їхній зміст.

Приклад:

"React Context"
→ [0.12, -0.55, 0.91, ...]

## Основна ідея
Схожі за змістом тексти мають схожі embeddings.

## Використання
- semantic search,
- RAG системи,
- recommendation systems,
- AI memory,
- кластеризація даних,
- code search.

## Як працює RAG
1. Документи діляться на chunks
2. Для chunk створюються embeddings
3. Вектори зберігаються у vector DB
4. Query користувача теж embedding
5. Система знаходить найближчі chunks
6. Вони додаються в context window LLM

## Vector databases
Популярні рішення:
- Pinecone
- Qdrant
- Weaviate
- PostgreSQL + pgvector