# Implementation Report

## Choices
1. **Dataset**: Hotel Booking Demand dataset from Kaggle (119,390 records)
2. **Vector DB**: ChromaDB with persistent storage for local deployment
3. **Embeddings**: all-MiniLM-L6-v2 for balance of performance/size
4. **LLM**: Phi-3-mini-4k-instruct (4.2B params, better CPU/GPU flexibility)
5. **API**: FastAPI for modern Python API development

## Challenges
1. **Data Scale**: Full dataset too large for RAG → sampled 5,000 records
2. **LLM Size**: Mistral-7B requires significant resources → used 4-bit quantization
3. **Numerical QA**: LLMs struggle with precise calculations → precomputed key metrics

## Future Improvements
1. Implement more sophisticated RAG with metadata filtering
2. Add caching for frequent queries
3. Deploy with proper scaling (e.g., Redis cache, load balancing)