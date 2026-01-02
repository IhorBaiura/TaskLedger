# TaskLedger

**TaskLedger** is a lightweight task manager built with Python — designed to keep a clean “ledger” of what needs doing, what’s in progress, and what’s done.

> Simple by default. Powerful when you need it.

## ✨ Features

- Create, edit, complete, and delete tasks
- Priorities and due dates
- Tags and smart filtering
- Search and sorting
- Persistent storage (local database or file-based)
- Import/Export (JSON/CSV) *(planned)*

## 🧱 Project Status

TaskLedger is in active development. Expect breaking changes until `v1.0.0`.

## 🗺️ Roadmap (High Level)

- [ ] Core task model (title, notes, status, priority, due date, tags)
- [ ] Storage layer (SQLite / JSON)
- [ ] Basic CLI interface
- [ ] Filtering & search
- [ ] Export/import (JSON, CSV)
- [ ] Optional TUI/GUI or REST API

## 🚀 Getting Started

### Requirements
- Python 3.10+ *(recommended 3.11+)*

### Install

```bash
git clone https://github.com/<your-username>/taskledger.git
cd taskledger
python -m venv .venv
# Linux/macOS
source .venv/bin/activate
# Windows
# .venv\Scripts\activate

pip install -r requirements.txt

## Run (example)

```bash
python -m taskledger
```

> If you haven't implemented an entrypoint yet, replace the command above with whatever script you use (e.g., `python main.py`).

## 🧪 Tests

```bash
pytest
```

## 📁 Project Structure (suggested)

```txt
taskledger/
  taskledger/
    __init__.py
    app.py
    models/
      task.py
    storage/
      base.py
      sqlite.py
      json_store.py
    services/
      tasks.py
    cli/
      main.py
  tests/
  README.md
  requirements.txt
  pyproject.toml
```

## 🧠 Core Concepts

A **Task** can include:

- `title` (required)
- `notes`
- `status` (todo / doing / done / archived)
- `priority` (low / medium / high)
- `due_date`
- `tags`
- timestamps (`created_at`, `updated_at`, `completed_at`)

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a branch: `git checkout -b feat/my-feature`
3. Commit changes: `git commit -m "Add my feature"`
4. Push: `git push origin feature/my-feature`
5. Open a Pull Request

## 📜 License

Choose a license and add it here (e.g., MIT):

```txt
MIT License
Copyright (c) 2026
```

## ⭐ Acknowledgements

- Inspired by simple productivity systems (GTD, Kanban, and plain old checklists).
