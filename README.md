# Scientific Knowledge Question Answering

## Prerequisites
numpy==1.26.0
pandas==2.2.3
torch==2.1.0
elasticsearch==8.8.0
sentence-transformers==2.2.2
transformers==4.37.2
openai==1.7.2


## 1. 개요
- LLM이 발전과 함께 사용자 수 급증함에 따라 Hallucination 문제를 차단하고 좋은 서비스를    제공할 필요가 있음
- 이를 위해 각기 다른 목적에 따른 효과적인 RAG Pipeline구축 필요 
- 이 프로젝트를 통해 각 기업이 필요로 하는 맞춤형 서비스를 설계하기 위함

## 2.개발 환경
- NVIDIA GeForce RTX 3090 24GB
- AMD Ryzen Threadripper 3960X 24-Core Processor

## 3. Dataset 
- 문서 데이터: 과학 상식 정보를 담은 4200여 개의 문서
- 데이터 형식: 각 문서는 DOC_ID와 출처(SRC)가 포함된 JSONL 포맷으로 구성, 실제로 참조할 지식 정보는 CONTENT 필드에 저장

## 4. Document Chunking + Reranking RAG Pipeline
![image](https://github.com/user-attachments/assets/8a773437-bb45-49b7-ab45-823ede38e6bc)

## 5. Hybrid retrieve(Sparse Retrieve ⬆) Reranking RAG Pipeline
![image](https://github.com/user-attachments/assets/49d40e60-afab-44b5-b84a-a9cf17841ae9)