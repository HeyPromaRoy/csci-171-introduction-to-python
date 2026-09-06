# Python Naming Do's and Don'ts

**Course:** CSCI 171 — Introduction to Python
**Instructor:** Proma Roy
**Term:** Fall 2026
**Companion to:** [Meeting 3 — Variables and Basic Data Types](notebooks/03_2026-09-08_variables_and_basic_types.ipynb)

This guide collects, in one place, the naming rules that Meetings 1–5 introduce piece by piece. It separates three different kinds of rules, because beginners often blur them together:

1. **Illegal** — Python refuses to run the code at all (`SyntaxError`).
2. **Legal but discouraged** — Python runs the code, but the name causes confusion, hides a bug, or breaks a tool students rely on (`print`, `type`, autograders).
3. **House style for this course** — not a Python requirement, but the convention every reference notebook follows so examples stay consistent and readable.

The goal at this stage is not to memorize a professional style guide. It is to build habits that make code easy to read, easy to predict, and easy to debug — the same habits that later, larger style rules (PEP 8, docstrings, constants) will simply formalize. Full-scale style discipline is postponed until functions and larger programs (Meetings 15–16 and beyond), on purpose.

---

## 1. Rules Python enforces (must not be violated)

Breaking any of these stops the program before it runs. Meeting 3 deliberately triggers one of these (`2students = 25`) so students see the error before learning the rule.

| Rule | Why | Illegal example | Legal fix |
|---|---|---|---|
| A name must start with a letter or an underscore, never a digit. | Python reads a leading digit as the start of a number, not a name. | `2students = 25` | `student_count = 25` |
| A name may contain only letters, digits, and underscores — no spaces, hyphens, or punctuation. | A space or hyphen splits the line into pieces Python cannot parse as one identifier. | `student count = 25`, `student-count = 25` | `student_count = 25` |
| A name cannot be a Python **keyword**. | Keywords already have a fixed grammatical meaning; Python cannot also treat them as a variable. | `class = "CSCI 171"`, `for = 3` | `course_name = "CSCI 171"`, `count = 3` |
| Assignment (`=`) is not equality (`==`). | `=` stores a value; `==` asks a yes/no question. Using `=` inside a condition is a syntax error. | `if age = 18:` | `if age == 18:` |

**The 35 reserved keywords** (never usable as a variable, function, or parameter name):

```
False   None    True    and    
 as      assert  async   await
break   class   continue def   
 del     elif    else    except
finally for     from    
global  if      import  in    
  is lambda  nonlocal not   
or      pass    raise   return  try
while   with    yield
```

Python will raise `SyntaxError: invalid syntax` immediately if a keyword is used as a name — there is no partial credit or silent fallback.

---

## 2. Legal, but must be avoided (shadowing and misleading names)

These do not crash the program, which is exactly what makes them dangerous — the mistake surfaces later, often confusingly, in a different cell.

### 2.1 Don't reuse the name of something Python already provides

Python lets a variable overwrite a built-in function's name. Once that happens, the built-in is unreachable for the rest of the runtime — a bug that only appears several cells later.

| Don't do this | Why it breaks things | Do this instead |
|---|---|---|
| `type = "essay"` | `type()` — the exact tool Meeting 3 uses to inspect a value — now refers to the string `"essay"` and can no longer be called. | `assignment_type = "essay"` |
| `print = "done"` | `print(...)` stops working; every later `print(...)` call raises `TypeError: 'str' object is not callable`. | `status = "done"` |
| `input = "yes"` | `input(...)` (Meeting 4) breaks the same way. | `user_response = "yes"` |
| `str = "42"`, `int = 5`, `float = 2.5`, `bool = True`, `list = [1, 2]`, `len = 3` | Each hides a built-in type or function used constantly in this course. | `str_value`, `student_count`, `average_score`, `is_enrolled`, `grades`, `name_length` |

**Why this matters especially in this course:** `type()` is the evidence-gathering tool taught in Meeting 3 ("use `type(value)` when you need evidence" instead of guessing). A student who names a variable `type` loses that tool for the rest of the session and gets a confusing `TypeError` far from the actual mistake.

### 2.2 Don't use single, ambiguous, or ultra-short letters

| Don't do this | Why | Do this instead |
|---|---|---|
| `l = 50`, `I = 10`, `O = 0` | In many fonts, lowercase `l`, uppercase `I`, and the digit `1` look nearly identical; uppercase `O` and `0` are also easy to confuse. A misread name causes a `NameError` that is hard to spot by eye. | `length = 50`, `id_number = 10`, `option = 0` |
| `x = 88.5`, `y = True`, `z = "Jordan"` | Tells the reader nothing about what the value represents; every value in Meeting 3's guided practice has a specific role (name, credits, GPA, enrollment). | `average_score`, `is_enrolled`, `student_name` |

**Course exception, introduced later:** short loop counters such as `i`, `j`, or short accumulator names are conventional once `for` loops and `range` are introduced (Meeting 11) — but that convention applies specifically to loop counters, not to ordinary data.

### 2.3 Don't invent your own leading/trailing underscore or ALL-CAPS conventions yet

| Don't do this | Why | What it actually means in Python |
|---|---|---|
| `_score`, `__score`, `__score__` | Leading and double-leading/trailing underscores are not decorative — they signal specific things (privacy convention, name-mangling, or reserved "dunder" names like `__init__`) that this course has not covered. | Use a plain name: `score`. |
| `AVERAGE_SCORE = 88.5` for a value that changes | ALL-CAPS is the conventional signal for a **constant** — a value that is not meant to be reassigned. Using it for an ordinary variable misleads a reader into thinking the value never changes. | `average_score = 88.5` (lowercase, because Meeting 3's `reassignment` idea — `score = score + 5` — depends on it being an ordinary variable). |

### 2.4 Don't mix naming styles within the same notebook or program

| Don't do this | Why | Do this instead |
|---|---|---|
| `studentCount`, `Student_Name`, `studentgpa` in the same cell | Mixing `camelCase`, capitalized words, and no separators at all forces the reader to re-parse each name individually and makes searching/renaming error-prone. | `student_count`, `student_name`, `student_gpa` — one style, applied consistently. |

`camelCase` and `PascalCase` are not illegal in Python, and students will encounter both later (`PascalCase` is the convention for class names, taught in a later course). For this course's variables and functions, **`snake_case` is the only style used**, so that every reference notebook looks consistent and a mixed style doesn't get mistaken for a meaningful difference.

---

## 3. House style this course follows (Do's)

These are the conventions every notebook from Meeting 1 onward already demonstrates. They are not enforced by Python — they are enforced by *readability*, and by matching the reference notebooks so students can compare their own code against them.

| Do this | Why | Example from the notebooks |
|---|---|---|
| Use `snake_case`: lowercase words separated by underscores. | Matches Python's own standard library and every built-in name; one style removes a whole category of guesswork. | `student_count`, `average_score`, `class_is_in_person` |
| Choose a name that describes *what the value represents*, not its type or its position. | The name should make `print(student_count)` self-explanatory without a comment. | `student_count` (not `x` or `num1`) |
| Phrase Boolean names as a yes/no question or condition. | Reading `if class_is_in_person:` aloud should sound like a real question. | `is_enrolled`, `has_student_id`, `room_has_computers`, `lab_is_open` |
| Keep a name specific enough to distinguish it from similar values in the same cell. | Meeting 3's guided practice uses four different variables (name, credits, GPA, enrollment) that must never be confused with each other. | `completed_credits` vs. `current_gpa` |
| Introduce (assign) a name in an earlier cell before any cell uses it. | Meeting 2 shows that using a name before it is defined raises `NameError`; notebook cells must be runnable top-to-bottom in one pass. | `course_name = "CSCI 171"` before `print(course_name)` |
| Verify an uncertain type with `type(value)` instead of guessing from appearance. | `42` and `"42"` look almost identical on the page but behave completely differently in arithmetic (Meeting 4's `TypeError` example). | `print(numeric_text, type(numeric_text))` |

---

## 4. Quick reference

| Situation | Verdict |
|---|---|
| Name starts with a digit (`2students`) | **Illegal** — `SyntaxError` |
| Name contains a space or hyphen (`student count`) | **Illegal** — `SyntaxError` |
| Name is a keyword (`class`, `for`, `True`) | **Illegal** — `SyntaxError` |
| `=` used where `==` is meant | **Illegal** — `SyntaxError` |
| Name shadows a built-in (`type`, `print`, `input`, `str`, `list`, `len`) | **Legal, but breaks that tool for the rest of the runtime** — avoid |
| Single ambiguous letter (`l`, `I`, `O`, or non-descriptive `x`, `y`, `z`) | **Legal, but hard to read or misread** — avoid |
| Leading/trailing underscores (`_score`, `__score__`) | **Legal, but means something else in Python** — avoid until taught |
| ALL_CAPS for a value that will be reassigned | **Legal, but misleading** — reserve ALL_CAPS for true constants |
| Mixed styles in one notebook (`studentCount` next to `student_name`) | **Legal, but inconsistent** — pick `snake_case` and keep it |
| Descriptive `snake_case`, question-style Booleans, defined-before-use | **Do this** |

---

© 2026 Proma Roy. Except where otherwise noted, this original instructional material is licensed under the [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](LICENSE).

This independently maintained instructor resource is not an official publication of John Jay College or The City University of New York.
