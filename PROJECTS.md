# 🛠️ Projects Tracker & Registry

This document catalogues project ideas, specifications, status, and learning milestones. I build these projects to put syntax and language design theories into practice.

---

## 🐍 Python Projects

### Beginner
* **Name**: CLI Scraping Engine
* **Status**: 🔴 Not Started
* **Skills Practiced**: HTTP Requests (`requests`, `httpx`), BeautifulSoup parser, CSV file writing, Argument Parsing (`argparse`).
* **Description**: A CLI tool that pulls price data from static retail pages and outputs a formatted spreadsheet.

### Intermediate
* **Name**: FastAPI Task Hub API
* **Status**: 🔴 Not Started
* **Skills Practiced**: FastAPI frameworks, Pydantic data schemas, SQLAlchemy ORM, SQLite databases, JWT authentication.
* **Description**: A production-grade REST API backend that supports user registration, task lists, and categorization.

### Advanced
* **Name**: Retreival-Augmented Generation (RAG) Document Agent
* **Status**: 🔴 Not Started
* **Skills Practiced**: Vector search, LangChain, NumPy data ingestion, ChromaDB vector databases, OpenAI API client structures.
* **Description**: An AI system that ingests PDF research files, builds vector indexes, and allows users to query documents using LLMs.

---

## 🦀 Rust Projects

### Beginner
* **Name**: CLI Task Manager (Todo tool)
* **Status**: 🔴 Not Started
* **Skills Practiced**: File serialization, Struct structures, JSON parsing (`serde`), Argument Parsing (`clap`).
* **Description**: A CLI-based task list tracker that saves logs to a hidden directory on disk.

### Intermediate
* **Name**: Multi-threaded Port Scanner
* **Status**: 🔴 Not Started
* **Skills Practiced**: Concurrency, Threading pools, TCP networking streams, Error Handling.
* **Description**: A command-line port scanner that tests target servers concurrently using thread pools.

### Advanced
* **Name**: Python CSV Parser Extension (PyO3)
* **Status**: 🔴 Not Started
* **Skills Practiced**: PyO3 bindings, Rust memory safety/mutability in extensions, Maturin compiler scripts.
* **Description**: A Rust module exposed to Python that parses complex CSV fields up to 10x faster than pure Python.

---

## 📘 TypeScript Projects

### Beginner
* **Name**: Interactive Calculator
* **Status**: 🔴 Not Started
* **Skills Practiced**: DOM manipulation, strict type checking, click events, state variables.
* **Description**: A beautifully styled vanilla-web browser calculator utilizing strict TypeScript rules.

### Intermediate
* **Name**: Weather Dashboard Component
* **Status**: 🔴 Not Started
* **Skills Practiced**: API integration (fetch), asynchronous hooks, interface modeling, React / Next.js basics.
* **Description**: A visual web component displaying current weather conditions based on location input.

### Advanced
* **Name**: Collaborative Real-Time Whiteboard
* **Status**: 🔴 Not Started
* **Skills Practiced**: WebSockets, canvas drawing APIs, custom event handlers, structural state management.
* **Description**: A real-time vector canvas allowing multiple clients to connect and draw together.

---

## 🤝 Integrated Projects

### Advanced (Integrated System)
* **Name**: Full-Stack AI Log Processor & Dashboard
* **Status**: 🔴 Not Started
* **Skills Practiced**: Polyglot architecture, Docker networks, API contracts, FastAPI schemas.
* **Description**:
  1. **Rust**: High-performance parser that reads, formats, and sanitizes logs from a stream.
  2. **Python**: Scans logs, uses models to extract error classifications and anomalies, and updates databases.
  3. **TypeScript**: Displays real-time charts on a dashboard frontend using React & WebSocket alerts.
