## Hi there 👋

# 👨🏻‍💻 Wonshik Nam | Backend / AI / Cloud Engineer

## Career

### <img width="24" height="24" src="https://github.com/user-attachments/assets/64a38f54-f7ed-4e08-bc5f-25f5b6db5dc7" /> ㈜ SuitdiO (CTO/이사) | 2025.05 – 2025.12 (폐업)

AI Agent(LLM) & Backend & Infra 총괄. [ChangeLog](https://feedback.suitdio.com/ko/changelog)

- **핵심 성과:**
1. AI Agent 원천 기술의 우수성을 바탕으로 기업 대상 전문 기술도입계약(Licensing) 체결
2. 신용보증기금 기술 평가를 통한 Easy-Start 2억(우대금리 2.9%) 규모 자금 유치
3. 매출 2200만원 달성, 56개국 접속 트래픽 처리
4. LLM·Embedding 기반 약물 부작용 연구로 국제 SCI 저널 논문 등재
5. 2024 성남시 청년창업지원사업 선정
- **실시간 협업 환경 구축:** WebSocket, SSE 통신 및 Redis Pub/Sub(Message Queue의 메시징 패턴) 기반 무한 캔버스 환경에서의 **실시간 편집 및 트랜잭션 관리 시스템** 구축.
- **운영 및 인프라 총괄:** AWS ECS 기반의 Auto Scaling, GitActions CI/CD 파이프라인, PostgreSQL 및 Redis **AWS 프로덕션 환경 운영**

## Core Projects

### 💻 Backend 시스템 아키텍처 설계 및 구축

- **트랜잭션 원자성 및 동시성 제어:**
  - PostgreSQL ACID 특성 활용한 트랜잭션 원자성 보장 및 All-or-Nothing 처리 구현.
  - Python asyncio.Lock과 SELECT FOR UPDATE 조합하여 Race Condition 발생률 0% 달성.
  - READ COMMITTED 격리 수준으로 Dirty Read 방지 및 동시성 균형 유지.
- **Bulk Processing 및 성능 최적화:**
  - PostgreSQL VALUES 절 활용한 벌크 연산으로 DB 처리 시간 82% 개선.
  - Incremental Update 시스템으로 중복 연산 40% 감소.
- **실시간 협업 시스템:**
  - WebSocket, SSE 통신 및 Redis Pub/Sub(Message Queue의 메시징 패턴) 기반 실시간 편집 시스템 구축.
  - 실시간 메시지 전파 지연시간 50ms 이내 유지 및 데이터 동기화 100% 보장.
- **계층적 자료구조 알고리즘:**
  - DFS 기반 순환 감지 알고리즘 구현으로 O(V+E) 시간복잡도 달성 및 10000개 노드 1초 이내 처리.
  - BFS 기반 계층 구조 최적화로 메모리 효율성 극대화 및 불필요한 연산 제거.

### ☁️ AWS Cloud Infrastructure 설계 및 DevOps

- **서버리스 컨테이너 인프라:**
  - ECS Fargate 및 Application Load Balancer 기반 Auto Scaling 구축으로 CPU 70% 이상 시 자동 확장 적용.
- **글로벌 CDN 및 스토리지:**
  - CloudFront로 56개국 글로벌 트래픽 처리 및 Edge Location 기반 정적 자산 캐싱.
- **CI/CD 파이프라인:**
  - GitHub Actions 기반 완전 자동화 배포 파이프라인 구축 및 배포 시간 83% 단축.
  - Multi-stage Docker Build로 이미지 크기 60% 감소 및 Rolling Update 전략으로 무중단 배포 구현.
- **모니터링 및 운영:**
  - CloudWatch 통합 모니터링 대시보드 구축 및 시스템 가용성 99.95% 달성.

### 🚀 LLM Framework 기반 AI Agent 개발

- **Context Engineering:**
  - `LangChain`, `LangGraph`를 활용하여 복잡도 높은 상태 전이 로직 설계.
  - **사용자 정의 규칙을 ChatState에 추가**하여 장기 기억 및 지침 목록을 관리하는 Context Engineering 기능을 구현하여 AI의 일관성과 추론 품질을 극대화
- **멀티모달 RAG 및 전처리:**
  - **Excel, PDF, YouTube, WebLink, Image, Markdown 등 다양한 형태의 멀티모달 데이터 Import 기능 구현**
  - `PGVector` 기반의 RAG 시스템 구축
- **Tool Calling 및 Code Interpreter 구현:**
  - AI Agent가 **Excel, Block Markdown 편집, Code Interpreter 기반 Chart 및 Diagram 시각화, Web Search** 등 복잡한 도구 호출을 수행할 수 있는 로직 통합
- **Multi-turn Chat Streaming:**
  - **SSE 기반의 Multi-turn Chat 기능**을 구현하여 ChatGPT, Gemini, Claude, Grok, Perplexity 등 **다중 모델을 지원**하고 실시간 응답 환경 제공

## Tech Stack

### 💻 BackEnd/AI

[![LangChain](https://img.shields.io/badge/LangChain-111111?style=for-the-badge&logo=langchain&logoColor=white)](https://www.langchain.com/)[![LangGraph](https://img.shields.io/badge/LangGraph-FF5733?style=for-the-badge&logoColor=white)](https://docs.langchain.com/langgraph/)[![LangSmith](https://img.shields.io/badge/LangSmith-00ABFF?style=for-the-badge&logoColor=white)](https://www.langchain.com/langsmith)

[![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)[![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)](https://www.djangoproject.com/)

[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org/)[![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)

### 📊 Data

[![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.w3schools.com/sql/)[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)[![scikit--learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)

[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)](https://matplotlib.org/)[![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://seaborn.pydata.org/)

[![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white)](https://www.selenium.dev/)[![Google Analytics](https://img.shields.io/badge/Google_Analytics-E37400?style=for-the-badge&logo=googleanalytics&logoColor=white)](https://analytics.google.com/)

### ☁️ Infra&Cloud

[![NGINX](https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=nginx&logoColor=white)](https://www.nginx.com/)[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)

[![ECS](https://img.shields.io/badge/ECS-FF9900?style=for-the-badge&logo=amazon-ecs&logoColor=white)](https://aws.amazon.com/ecs/)[![EC2](https://img.shields.io/badge/EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white)](https://aws.amazon.com/ec2/)[![VPC](https://img.shields.io/badge/VPC-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)](https://aws.amazon.com/vpc/)[![CloudFront](https://img.shields.io/badge/CloudFront-FF4500?style=for-the-badge&logo=amazon-cloudfront&logoColor=white)](https://aws.amazon.com/cloudfront/)[![S3](https://img.shields.io/badge/S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white)](https://aws.amazon.com/s3/)[![Load Balancer](https://img.shields.io/badge/Load_Balancer-8C4FFF?style=for-the-badge&logo=awselasticloadbalancing&logoColor=white)](https://aws.amazon.com/elasticloadbalancing/)

[![RDS](https://img.shields.io/badge/RDS-527FFF?style=for-the-badge&logo=amazon-rds&logoColor=white)](https://aws.amazon.com/rds/)[![ElastiCache](https://img.shields.io/badge/ElastiCache-C925D1?style=for-the-badge&logo=amazonelasticache&logoColor=white)](https://aws.amazon.com/elasticache/)[![CloudWatch](https://img.shields.io/badge/CloudWatch-FF4F8B?style=for-the-badge&logo=amazoncloudwatch&logoColor=white)](https://aws.amazon.com/cloudwatch/)

### 💾 Database&VectorStore

[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)[![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)](https://redis.io/)

[![PGVector](https://img.shields.io/badge/PGVector-4169E1?style=for-the-badge&logoColor=white)](https://github.com/pgvector/pgvector)

### 🔄 CI/CD

[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)](https://github.com/features/actions)[![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)](https://www.jenkins.io/)

### 🛠️ Collabo

[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)](https://git-scm.com/)[![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)](https://slack.com/)[![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)](https://www.notion.so/)[![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/)
