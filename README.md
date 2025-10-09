# Financial Policy RAG: Retrieval-Augmented Generation for SME Loan & FCA Regulation
This project builds an advanced RAG pipeline for financial policy documents, focusing on SME loan eligibility and UK FCA regulations. It uses semantic chunking, FAISS search, query rewriting, and reranking (cosine similarity &amp; step-back prompting) to improve reasoning and relevance in high-stakes regulatory contexts.

## Project Overview 
This project develops a domain-specialized Retrieval-Augmented Generation (RAG) pipeline tailored for financial policy documents, addressing the limitations of large language models (LLMs) like GPT-4 and Cohere, which often lack access to up-to-date, domain-specific information.

### Key Features
Focusing on UK Financial Conduct Authority (FCA) regulations and SME loan eligibility policies, the system integrates dense retrieval with LLMs to generate grounded, contextually accurate responses. It extends standard RAG approaches by incorporating advanced techniques to boost retrieval quality and reasoning precision:
1. **Semantic Chunking:** Segments documents into meaningful units to preserve context.
2. **FAISS Vector Search:** Enables efficient similarity-based retrieval over dense embeddings.
3. **Query Rewriting:** Refines user input to improve retrieval relevance.
4. **Reranking via Cosine Similarity:** Prioritizes retrieved chunks based on semantic closeness to the query.
5. **Step-Back Prompting:** Enhances reasoning by guiding the LLM through intermediate steps.

## Implementation
<img width="249" alt="Screenshot 2025-07-01 at 1 12 56 AM" src="https://github.com/user-attachments/assets/f48f9fc6-da50-4180-9865-85a09cc3793f" /> 

The pipeline is benchmarked against a non-retrieval LLM baseline, with evaluation metrics based on faithfulness and relevance—supplemented by multi-rater confidence intervals—to validate its effectiveness in high-stakes, regulation-heavy environments.

### Evaluation
The RAG system is evaluated against a non-retrieval LLM baseline. Performance metrics include:
1. Faithfulness: Accuracy and factual consistency of generated responses.
2. Relevance: Appropriateness and specificity of the retrieved content.
3. Multi-Rater Error Bars: Inter-annotator agreement provides robust evaluation confidence.

<img width="350" alt="Screenshot 2025-07-01 at 1 42 23 AM" src="https://github.com/user-attachments/assets/8602d890-6af7-47e5-9352-8616671da66f" /> 
<img width="350" alt="Screenshot 2025-07-01 at 1 44 58 AM" src="https://github.com/user-attachments/assets/d77aaa6d-e081-4a7c-926c-69cae071078f" />

### Use Cases

- Interpreting complex financial policy documents
- Supporting SME loan eligibility assessments
- Assisting compliance teams with FCA regulatory guidelines
