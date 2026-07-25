<div align="center">

# 🎓 Campus OS
### *A Python Programming Portfolio — Told Through One Running Story*

**Anshul Ghildiyal**  |  **SAP ID: 590031643**  |  MCA (AI & ML), UPES Dehradun
Course: Python Programming — Creative Lab Portfolio Assignment

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-orange?logo=jupyter)
![NumPy](https://img.shields.io/badge/NumPy-Data-013243?logo=numpy)
![Pandas](https://img.shields.io/badge/Pandas-Analysis-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visuals-11557C)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

</div>

---

## 🧠 The Idea

Every lab experiment in a typical Python course lives alone — Question 1, Question 2, unrelated to
Question 3. **Campus OS** rejects that. Every one of the ten experiments in this repo is written
around **one continuous cast of characters and one running theme**: campus life at UPES, the gym,
and **Project Vegapunk** — a real, ongoing algorithmic-trading system I'm building as my long-term
MCA capstone.

Each experiment opens with a real-life analogy (a vending machine, a hackathon leaderboard, a
gym ladder routine) *before* a single line of code appears — the concept has to make sense as a
story first. Then comes clean, commented code, an **"Under the Hood"** section explaining
complexity and gotchas, and a **"Level Up"** section where I push the original lab question
further than what was asked, on my own.

The **mini-project** (`/mini_project`) is where this stops being a metaphor and becomes real: a
small simulation that persists state to disk, mutates a live object across a 14-day loop, and
visualizes the result — using six of the ten required Python concepts working together.

---


## 🎯 The Mini-Project: Campus OS Simulator

> **Where:** [`/mini_project/Mini_Project_CampusOS.ipynb`](UPES_PG_Template\Subjects\Bridge-Course\Practice\Mini_Project_CampusOS.ipynb)

A 14-day semester simulation for a single character, **Ray**, where every day:

1. Study hours and gym hours are generated (with realistic variance)
2. A miniature stand-in for Project Vegapunk's trading engine runs a simulated paper-trade
3. All three feed into a `Student` object whose cash balance, discipline streak, and history evolve
4. Every day's record is **written live to a CSV file on disk** and later **read back independently**
   to prove the persistence actually works
5. Bad input (impossible hours, trading with zero capital) is caught by **custom exceptions**,
   not allowed to crash the simulation
6. The full semester is visualized as a **4-panel Matplotlib dashboard** — study/gym trend, the
   trading balance curve, grade distribution, and discipline streak

**Concepts combined:** Classes & Objects · File Handling · Exception Handling · Functions ·
Loops & Conditionals · Data Visualization (6 of the 10 listed concepts — well above the 4 required).

---

## 🧩 Notebook Highlights

| Experiment | Theme | A "Level Up" worth noticing |
|---|---|---|
| 1 | The University ID Card | Identity vs. equality (`is` vs `==`), memory internals via `sys.getsizeof` |
| 2 | Server room bitwise ops | Truth tables, bit shifting as fast multiplication |
| 3 | Vending machine / physics sim | Complex roots via `cmath`, config-driven grading (no hardcoded `if`) |
| 4 | Progressive-overload factorial | Sieve of Eratosthenes, generator-based Fibonacci |
| 5 | Frat-party vowel bouncer | Hash-set lookups, regex lookahead for overlapping substrings |
| 6 | Ride-share board | `collections.Counter`, `defaultdict`, one-pass runner-up algorithm |
| 7 | Hackathon registration API | `*args`/`**kwargs`, `lru_cache` memoized Fibonacci, mutable-default-argument trap |
| 8 | Dorm party guest list | Custom exceptions with `from e`, safe CSV/structured parsing |
| 9 | University ID template | `@dataclass`, `@property`, MRO / diamond-problem inheritance, operator overloading |
| 10 | Pitch-deck dashboard | NumPy vectorized ops, Pandas index alignment, Seaborn theming |

---

## 🛠️ Use of AI Tools

AI tools (Claude, ChatGPT-style assistants) were used during this assignment for:

- **Debugging** logic errors surfaced during testing (e.g. the factorial initialization gotcha in
  Experiment 4, the negative-modulo edge case in Experiment 2)
- **Improving notebook explanations** — turning a bare code comment into a full analogy-first
  walkthrough
- **Generating the SVG diagrams** embedded throughout the notebooks
- **Structuring the mini-project's architecture** (deciding to separate simulation functions from
  the `Student` class, similar to how Project Vegapunk's satellites stay independently testable)
- **Drafting this README**

All code was independently reviewed, tested, and understood before submission. Every notebook runs
top-to-bottom without errors, and I can walk through the logic of any cell in this repository.

---

## ⚙️ Setup

```bash
pip install -r requirements.txt
jupyter notebook
```

---

<div align="center">

*Built as part of the MCA (AI & ML) Python Programming Lab — UPES Dehradun, 2026*


*Mentor: Vibhu Gautum*

</div>
