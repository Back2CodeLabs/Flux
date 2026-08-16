# Architecture

Version: 0.1

---

# Vision

Project F.L.U.X. is a Mission Operating System.

Everything is a Mission.

---

# High Level Architecture

                    User
                      │
          Telegram / Web / API
                      │
                ClawSS117
                      │
                Mission Queue
                      │
                    TARS
                      │
        ┌─────────────┼─────────────┐
        │             │             │
     JARVIS         DOC          GUARDIAN
        │             │             │
        └──────┬──────┴──────┬──────┘
               │             │
            EDITH         SCOUT
               │             │
         Docker / MCP    Internet
               │
         Infrastructure

---

# Principles

Single Responsibility

Loose Coupling

Strong Cohesion

Event Driven when valuable

REST First

MCP Native

Container First

---

# Communication

User

↓

Mission

↓

Planner

↓

Execution

↓

Validation

↓

Response

---

# Persistence

PostgreSQL

Business data

Mission history

Agent state

Configuration

---

Redis

Cache

Queues

Events

Temporary memory

---

ChromaDB

Embeddings

Knowledge

Semantic search

Documentation

---

# AI Models

Default

Ollama

Fallback

Cloud providers

Optional only.

---

# Deployment

Docker Compose

One command deployment.

---

# Monitoring

Prometheus (future)

Grafana (future)

Dozzle

Uptime Kuma

FRIDAY