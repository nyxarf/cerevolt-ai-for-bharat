# Cerevolt – System Design Document

---

##  System Architecture Overview

Cerevolt follows a secure, scalable microservices architecture.

Client Applications
↓
Authentication & Security Layer
↓
API Gateway
↓
Microservices Layer
    ├── Session Engine
    ├── Recommendation Engine
    ├── Analytics Engine
    ├── AI Classification Engine
    ├── Neurofeedback Processor
↓
Encrypted Cloud Database
↓
Model Server (Optional GPU Support)

---

##  Core Components

### 1. Client Layer
- Child App (Home Mode)
- School Dashboard
- Parent Dashboard
- Clinician Dashboard
- Admin Panel

Supports:
- Responsive Web
- Mobile App
- Offline Mode

---

### 2. Security Layer
- JWT Authentication
- Role-Based Access Control
- Encrypted Data Transmission
- Session Timeout Enforcement
- Audit Logging

---

### 3. API Gateway
- Central request routing
- Rate limiting
- Load balancing
- Request validation
- Logging & monitoring

---

### 4. Microservices Layer

#### Session Engine
- Controls screen time
- Manages session pacing
- Logs engagement

#### Recommendation Engine
- AI-driven personalization
- Content matching
- Adaptive difficulty

#### Analytics Engine
- Engagement tracking
- Emotional pattern analysis
- Report generation

#### AI Classification Engine
- Calm vs overstimulated detection
- Behavioral trend modeling

#### Neurofeedback Processor
- EEG/HRV data processing
- Real-time adaptive therapy

---

### 5. Database Design

Encrypted Cloud Storage

Stores:
- User profiles
- Session logs
- Emotional state history
- Cognitive scores
- Institutional data

Encryption:
- AES-256 at rest
- Encrypted local storage for offline mode

---

##  Process Flow

Login
↓
Authentication
↓
Select Mode (Home / School / Clinical)
↓
Session Start
↓
AI Analysis
↓
Content Recommendation
↓
Child Interaction
↓
Data Capture
↓
Analytics Processing
↓
Report Generation
↓
Encrypted Storage
↓
Continuous Learning Loop

---

##  Admin Panel Design

Modules:
- User Management
- Study Material Management
- Video & Audio Library
- Institutional Management
- AI Monitoring
- Compliance Dashboard
- Contact Management

---

##  Data Flow Design

Data Flow:
User → API Gateway → Services → Database → Analytics → Dashboard

Control Flow:
Admin/Teacher/Parent → Session Config → Recommendation Engine → Content Delivery

---

##  Deployment Design

- Docker Containerized Services
- Kubernetes Orchestration
- Cloud Hosting (AWS/GCP/Azure)
- CDN for static content
- Redis caching layer
- Auto-scaling infrastructure

---

##  Design Principles

- Child-first design philosophy
- Autism-inclusive UX
- Ethical AI implementation
- Data privacy by design
- Scalable & modular architecture
- Cross-environment continuity (Home–School–Clinic)

---

##  Future Design Expansion

- Wearable sensor API integration
- Advanced AI conversational model
- Cross-language localization
- Research analytics dashboard
- Companion physical kit integration

---

##  Authors

- Arfa Ahmed Ansari  
- Abhiroop Mukherjee  
- Ankur Banerjee  
- Kaushani Chandra  

---
