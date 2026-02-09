# SDD-Hackathon-02

A collection of Todo application projects demonstrating progressive development from CLI to full-stack web applications using Spec-Driven Development (SDD) methodology.

## 📋 Overview

This repository contains four phases of Todo application development, each building upon the previous phase with increasing complexity and features. All projects follow the Spec-Driven Development approach with comprehensive documentation, planning, and task breakdown.

## 🗂️ Project Structure

### Phase-01: CLI Todo Application
A command-line interface todo application built with Python.

**Tech Stack:**
- Python 3.x
- Typer (CLI framework)
- SQLModel (ORM)
- Rich (terminal formatting)
- SQLite database

**Features:**
- Add tasks via command line
- SQLite database storage
- Rich terminal UI with colors and formatting
- Simple and lightweight

**Quick Start:**
```bash
cd Phase-01
pip install -r requirements.txt
python main.py add "Your task here"
```

### Phase-02: Full-Stack Todo with Neon Postgres
A web-based todo application with FastAPI backend and Next.js frontend, using Neon Postgres cloud database.

**Tech Stack:**
- Backend: FastAPI, SQLModel, Neon Postgres
- Frontend: Next.js 14, TypeScript, Tailwind CSS
- Database: Neon Postgres with SSL
- Docker support

**Features:**
- RESTful API with FastAPI
- React-based frontend with Next.js
- Cloud database with Neon Postgres
- CORS configuration
- Logging system
- Docker containerization

**Quick Start:**
```bash
cd Phase-02
# Backend
cd backend
pip install -r requirements.txt
uvicorn main:app --reload --port 8000

# Frontend (new terminal)
cd frontend
npm install
npm run dev
```

### Phase-03: Enhanced Full-Stack Todo
An improved version of Phase-02 with better architecture and additional features.

**Tech Stack:**
- Backend: FastAPI, SQLModel, Neon Postgres
- Frontend: Next.js 14, TypeScript, Tailwind CSS
- Database: Neon Postgres
- Docker Compose for orchestration

**Features:**
- All Phase-02 features
- Improved project structure
- Enhanced error handling
- Better separation of concerns
- Docker Compose setup
- Comprehensive documentation

**Quick Start:**
```bash
cd Phase-03
docker-compose up
# Or run manually like Phase-02
```

### Phase-04: (Empty - Future Development)
Reserved for future enhancements.

## 🎯 Development Methodology

All phases follow **Spec-Driven Development (SDD)** principles:

1. **Constitution** - Project principles and guidelines
2. **Specification** - Detailed feature requirements
3. **Planning** - Architecture and design decisions
4. **Tasks** - Testable implementation tasks
5. **Implementation** - Code with proper documentation
6. **Testing** - Verification and validation

Each phase includes:
- `.specify/` - Templates and scripts for SDD workflow
- `specs/` - Feature specifications and plans
- `history/` - Prompt history records and decisions
- `.qwen/` - AI agent command configurations

## 🚀 Getting Started

### Prerequisites
- Python 3.8+ (for backend projects)
- Node.js 18+ (for frontend projects)
- Docker & Docker Compose (optional, for containerized deployment)
- Git

### Installation

1. Clone the repository:
```bash
git clone https://github.com/shayan509/SDD-Hackathon-02.git
cd SDD-Hackathon-02
```

2. Choose a phase and follow its Quick Start guide above

### Environment Variables

Each phase requiring database connection needs a `.env` file:

**Phase-01:**
```env
DATABASE_URL=sqlite:///./todos.db
```

**Phase-02 & Phase-03:**
```env
DATABASE_URL=postgresql://username:password@host/dbname?sslmode=require
```

## 📚 Documentation

Each phase contains detailed documentation:
- `README.md` - Project overview and setup
- `QWEN.md` - AI agent guidelines and SDD rules
- `specs/` - Feature specifications and plans
- `DOCKER_SETUP.md` - Docker configuration (Phase-02, Phase-03)

## 🛠️ Tech Stack Summary

| Component | Phase-01 | Phase-02 | Phase-03 |
|-----------|----------|----------|----------|
| Language | Python | Python + TypeScript | Python + TypeScript |
| Backend | Typer CLI | FastAPI | FastAPI |
| Frontend | - | Next.js 14 | Next.js 14 |
| Database | SQLite | Neon Postgres | Neon Postgres |
| ORM | SQLModel | SQLModel | SQLModel |
| Styling | Rich | Tailwind CSS | Tailwind CSS |
| Container | - | Docker | Docker Compose |

## 🤝 Contributing

This is a hackathon project demonstrating SDD methodology. Feel free to explore the code and learn from the structured development approach.

## 📝 License

This project is part of a hackathon and is available for educational purposes.

## 👤 Author

**Shayan**
- GitHub: [@shayan509](https://github.com/shayan509)

## 🙏 Acknowledgments

- Built using Spec-Driven Development methodology
- Powered by Qwen AI agent for structured development
- FastAPI and Next.js communities for excellent frameworks