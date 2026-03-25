# 🏗️ AI-Powered JIRA Duplicate Defect Detection Agent - Architecture

## 📋 Table of Contents

1. [Overview](#overview)
2. [High-Level Architecture](#high-level-architecture)
3. [Component Details](#component-details)
4. [Database Schema](#database-schema)
5. [API Endpoints](#api-endpoints)
6. [Data Flow](#data-flow)
7. [Technology Stack](#technology-stack)
8. [Implementation Phases](#implementation-phases)

---

## Overview

**Purpose:** Automatically detect duplicate defects in JIRA using AI-powered semantic search and validation.

**Problem Solved:**
- **20–30% of defects** in large QA teams are duplicates
- Manual detection is time-consuming, error-prone, and inefficient
- Results in wasted engineering effort and increased backlog noise

**Expected Benefits:**
- Reduce duplicate defects by **40–60%**
- Faster triage (seconds vs minutes)
- Improved defect quality and developer productivity

---

## High-Level Architecture
# 🏗️ AI-Powered JIRA Duplicate Defect Detection Agent - Architecture

## 📋 Table of Contents

1. [Overview](#overview)
2. [High-Level Architecture](#high-level-architecture)
3. [Component Details](#component-details)
4. [Database Schema](#database-schema)
5. [API Endpoints](#api-endpoints)
6. [Data Flow](#data-flow)
7. [Technology Stack](#technology-stack)
8. [Implementation Phases](#implementation-phases)

---

## Overview

**Purpose:** Automatically detect duplicate defects in JIRA using AI-powered semantic search and validation.

**Problem Solved:**
- **20–30% of defects** in large QA teams are duplicates
- Manual detection is time-consuming, error-prone, and inefficient
- Results in wasted engineering effort and increased backlog noise

**Expected Benefits:**
- Reduce duplicate defects by **40–60%**
- Faster triage (seconds vs minutes)
- Improved defect quality and developer productivity

---

## High-Level Architecture
# 🏗️ AI-Powered JIRA Duplicate Defect Detection Agent - Architecture

## 📋 Table of Contents

1. [Overview](#overview)
2. [High-Level Architecture](#high-level-architecture)
3. [Component Details](#component-details)
4. [Database Schema](#database-schema)
5. [API Endpoints](#api-endpoints)
6. [Data Flow](#data-flow)
7. [Technology Stack](#technology-stack)
8. [Implementation Phases](#implementation-phases)

---

## Overview

**Purpose:** Automatically detect duplicate defects in JIRA using AI-powered semantic search and validation.

**Problem Solved:**
- **20–30% of defects** in large QA teams are duplicates
- Manual detection is time-consuming, error-prone, and inefficient
- Results in wasted engineering effort and increased backlog noise

**Expected Benefits:**
- Reduce duplicate defects by **40–60%**
- Faster triage (seconds vs minutes)
- Improved defect quality and developer productivity

---

## High-Level Architecture
# 🏗️ AI-Powered JIRA Duplicate Defect Detection Agent - Architecture

## 📋 Table of Contents

1. [Overview](#overview)
2. [High-Level Architecture](#high-level-architecture)
3. [Component Details](#component-details)
4. [Database Schema](#database-schema)
5. [API Endpoints](#api-endpoints)
6. [Data Flow](#data-flow)
7. [Technology Stack](#technology-stack)
8. [Implementation Phases](#implementation-phases)

---

## Overview

**Purpose:** Automatically detect duplicate defects in JIRA using AI-powered semantic search and validation.

**Problem Solved:**
- **20–30% of defects** in large QA teams are duplicates
- Manual detection is time-consuming, error-prone, and inefficient
- Results in wasted engineering effort and increased backlog noise

**Expected Benefits:**
- Reduce duplicate defects by **40–60%**
- Faster triage (seconds vs minutes)
- Improved defect quality and developer productivity

---

## High-Level Architecture
# 🏗️ AI-Powered JIRA Duplicate Defect Detection Agent - Architecture

## 📋 Table of Contents

1. [Overview](#overview)
2. [High-Level Architecture](#high-level-architecture)
3. [Component Details](#component-details)
4. [Database Schema](#database-schema)
5. [API Endpoints](#api-endpoints)
6. [Data Flow](#data-flow)
7. [Technology Stack](#technology-stack)
8. [Implementation Phases](#implementation-phases)

---

## Overview

**Purpose:** Automatically detect duplicate defects in JIRA using AI-powered semantic search and validation.

**Problem Solved:**
- **20–30% of defects** in large QA teams are duplicates
- Manual detection is time-consuming, error-prone, and inefficient
- Results in wasted engineering effort and increased backlog noise

**Expected Benefits:**
- Reduce duplicate defects by **40–60%**
- Faster triage (seconds vs minutes)
- Improved defect quality and developer productivity

---

## High-Level Architecture
# 🏗️ AI-Powered JIRA Duplicate Defect Detection Agent - Architecture

## 📋 Table of Contents

1. [Overview](#overview)
2. [High-Level Architecture](#high-level-architecture)
3. [Component Details](#component-details)
4. [Database Schema](#database-schema)
5. [API Endpoints](#api-endpoints)
6. [Data Flow](#data-flow)
7. [Technology Stack](#technology-stack)
8. [Implementation Phases](#implementation-phases)

---

## Overview

**Purpose:** Automatically detect duplicate defects in JIRA using AI-powered semantic search and validation.

**Problem Solved:**
- **20–30% of defects** in large QA teams are duplicates
- Manual detection is time-consuming, error-prone, and inefficient
- Results in wasted engineering effort and increased backlog noise

**Expected Benefits:**
- Reduce duplicate defects by **40–60%**
- Faster triage (seconds vs minutes)
- Improved defect quality and developer productivity

---

## High-Level Architecture
┌─────────────┐
│ Web UI │
└──────┬──────┘
│
┌──────▼────────────────┐
│ FastAPI Backend │
├──────────────────────┤
│ - Defect Controller │
│ - JIRA Controller │
└──────┬────────────────┘
│
┌──────▼──────────────────┐
│ Processing Layer │
├──────────────────────────┤
│ - Text Cleaning │
│ - OCR Processing │
│ - Text Merging │
└──────┬──────────────────┘
│
┌──────▼──────────────────┐
│ Embedding Layer │
├──────────────────────────┤
│ - Vector Generation │
│ - Store Embeddings │
└──────┬──────────────────┘
│
┌──────▼──────────────────┐
│ Search Layer │
├──────────────────────────┤
│ - Vector Similarity │
│ - Top-K Retrieval │
└──────┬──────────────────┘
│
┌──────▼──────────────────┐
│ LLM Validation Layer │
├──────────────────────────┤
│ - Match Classification │
│ - Explanation Gen │
└──────┬──────────────────┘
│
┌──────▼──────────────────┐
│ PostgreSQL Database │
├──────────────────────────┤
│ - Defects Table │
│ - Embeddings Table │
└──────────────────────────┘


---

## Component Details

### 1. **API Layer**

**Responsibility:** Handle incoming requests and orchestrate service layer calls.

**Controllers:**
- `DefectController` - Manage defect operations
- `JiraController` - Manage JIRA synchronization

**Key Endpoints:**
- `POST /defect/check-duplicate` - Check for duplicates
- `GET /defect/similar/{id}` - Retrieve cached similar defects
- `POST /jira/sync` - Sync defects from JIRA

---

### 2. **Processing Layer**

**Responsibility:** Prepare raw input for embedding generation.

**Tasks:**
- Text cleaning and normalization
- Noise removal
- OCR extraction from screenshots
- Merge OCR output with user-provided text
- Handle special characters and formatting

**Input:** Raw defect text + screenshot (optional)  
**Output:** Cleaned, merged text ready for embedding

---

### 3. **Embedding Layer**

**Responsibility:** Convert processed text into vector embeddings.

**Tasks:**
- Generate embeddings using a language model (e.g., Mistral, OpenAI)
- Store embeddings in the database
- Support batch processing for bulk defects

**Input:** Cleaned text  
**Output:** Vector embedding (e.g., 384D or 1536D)

---

### 4. **Search Layer**

**Responsibility:** Find similar defects using vector similarity.

**Approach:** Cosine similarity search in vector space

**Tasks:**
- Query the embedding database
- Return top-K similar defects (ranked by similarity score)
- Support filtering by date, status, or project

**Input:** Query embedding  
**Output:** List of similar defect IDs with similarity scores

---

### 5. **LLM Validation Layer**

**Responsibility:** Validate and classify search results.

**Tasks:**
- Receive top-K search results
- Perform semantic analysis
- Classify match type:
  - **Exact Match** - Clearly the same defect
  - **Partial Match** - Related but not identical
  - **Not Duplicate** - False positive
- Generate human-readable explanation
- Create recommendation ("Mark as duplicate" or "Create new")

**Input:** Original defect + top-K similar defects  
**Output:** Classification, explanation, recommendation

---

### 6. **Web UI Layer**

**Responsibility:** User-facing interface for defect submission and results.

**Components:**
- Defect submission form (summary, description, screenshot upload)
- Results display page (similar defects list, explanations, recommendations)
- Status indicators (processing, completed, errors)

---

## Database Schema

### Tables

#### **Defects Table**
```sql
CREATE TABLE defects (
    id UUID PRIMARY KEY,
    summary TEXT NOT NULL,
    description TEXT,
    status VARCHAR(50),  -- Open, Closed, Duplicate, etc.
    created_at TIMESTAMP,
    updated_at TIMESTAMP,
    project_key VARCHAR(10),
    created_by VARCHAR(100)
);

CREATE TABLE embeddings (
    id UUID PRIMARY KEY,
    defect_id UUID REFERENCES defects(id),
    embedding_vector VECTOR(384),  -- pgvector extension
    created_at TIMESTAMP,
    model_version VARCHAR(50)
);

CREATE TABLE similarity_results (
    id UUID PRIMARY KEY,
    query_defect_id UUID REFERENCES defects(id),
    matched_defect_id UUID REFERENCES defects(id),
    similarity_score FLOAT,
    match_type VARCHAR(50),  -- Exact, Partial, NotDuplicate
    explanation TEXT,
    created_at TIMESTAMP
);
API Endpoints
POST /defect/check-duplicate
Check if a defect is a duplicate.

Request:
{
  "summary": "Login button not responding",
  "description": "User cannot click login button on signup page.",
  "screenshot": "[base64 image or file upload]"
}
Response:
{
  "query_defect_id": "uuid-1",
  "similar_defects": [
    {
      "id": "uuid-2",
      "summary": "Login button unresponsive",
      "similarity_score": 0.94,
      "match_type": "Exact"
    },
    {
      "id": "uuid-3",
      "summary": "Signup form buttons broken",
      "similarity_score": 0.78,
      "match_type": "Partial"
    }
  ],
  "recommendation": "Mark as duplicate (ID: uuid-2)",
  "explanation": "This defect matches an existing report about login button responsiveness with 94% semantic similarity."
}
GET /defect/similar/{id}
Retrieve previously computed similar defects.

Response:
{
  "defect_id": "uuid-1",
  "similar_defects": [...],
  "cached_at": "2026-03-25T10:30:00Z"
}
POST /jira/sync
Sync defects from JIRA into the local database.

Request:
{
  "project_key": "MYPROJECT",
  "since": "2026-01-01"
}
Response:

{
  "synced_count": 120,
  "failed_count": 0,
  "status": "SUCCESS"
}
Data Flow
End-to-End Duplicate Detection Flow
1. User submits defect
   ├─ Summary
   ├─ Description
   └─ Screenshot (optional)
                    │
                    ▼
2. API receives request → DefectController.checkDuplicate()
                    │
                    ▼
3. ProcessingService cleans text
   ├─ Remove noise
   ├─ Extract OCR from screenshot
   └─ Merge text + OCR output
                    │
                    ▼
4. EmbeddingService generates vector
   ├─ Call embedding model (Mistral, OpenAI, etc.)
   └─ Return 384D or 1536D vector
                    │
                    ▼
5. SearchService queries similar defects
   ├─ Cosine similarity search
   ├─ Return top-K results (e.g., top-5)
   └─ Include similarity scores
                    │
                    ▼
6. LLMService validates results
   ├─ Classify match type (Exact/Partial/NotDuplicate)
   ├─ Generate explanation
   └─ Create recommendation
                    │
                    ▼
7. Response returned to user
   ├─ Similar defects list
   ├─ Recommendations
   └─ Explanations
Technology Stack
Layer	Technology	Purpose
Framework	FastAPI	REST API backend
Language	Python 3.10+	Core implementation
Database	PostgreSQL + pgvector	Vector storage & similarity search
Embeddings	Mistral / OpenAI	Text-to-vector conversion
LLM	Mistral / OpenAI	Validation & classification
Frontend	React	Web UI
ORM	SQLAlchemy	Database abstraction
Web Server	Uvicorn	ASGI server
Implementation Phases
Phase 1: API Layer & Database (Week 1-2)
✅ Design REST endpoints
✅ Create PostgreSQL schema
✅ Implement DefectController
✅ Implement JiraController
✅ Unit tests for API layer
Phase 2: Processing & Database Repositories (Week 2-3)
✅ ProcessingService (text cleaning, OCR)
✅ DefectRepository (CRUD operations)
✅ EmbeddingRepository (vector storage)
✅ Integration tests
Phase 3: Embedding & Search (Week 3-4)
✅ EmbeddingService (vector generation)
✅ SearchService (similarity search)
✅ Caching layer
✅ Performance benchmarking
Phase 4: LLM Validation (Week 4-5)
✅ LLMService (classification & explanation)
✅ Prompt engineering
✅ Error handling and fallbacks
Phase 5: Web UI (Week 5-6)
✅ Defect submission form
✅ Results display page
✅ Integration with backend
Phase 6: Testing & Deployment (Week 6-7)
✅ End-to-end testing
✅ Performance testing
✅ JIRA integration testing
✅ Production deployment
Design Principles
✅ Applied Guidelines
Simple Architecture - No overengineering (no Kafka, LangGraph, microservices)
API-First Design - Clear, RESTful contracts
Modularity - Separated concerns, easy to test
Testability - Each service has unit & integration tests
Scalability - Database indexes, vector caching, batch processing
❌ Avoided
Kafka (unnecessary complexity)
Microservices (premature optimization)
LangGraph (overkill for this use case)
Redis caching (database is sufficient; add later if needed)
Future Enhancements
Hybrid Search - Combine BM25 (keyword) + vector search
JIRA Webhook Integration - Real-time sync instead of batch
Feedback Loop - Improve embeddings based on user feedback
Domain-Specific Model - Fine-tune embeddings for QA defects
Analytics Dashboard - Duplicate reduction metrics, trends
Multi-Modal Search - Better screenshot analysis and comparison
Smart Categorization - Auto-tag defects by component/subsystem
Summary
This architecture provides a clean, scalable solution for AI-powered duplicate defect detection. It balances simplicity with functionality, using modern technologies (embeddings, LLMs) while avoiding unnecessary complexity. The modular design enables iterative development and future enhancements.

Key Success Metrics:

Duplicate detection accuracy > 85%
Response time < 5 seconds
Reduced duplicate defects by 40–60%
User satisfaction score > 8/10


