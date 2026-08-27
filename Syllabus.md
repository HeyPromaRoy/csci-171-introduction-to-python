<a id="top"></a>

# CSCI 171 — Introduction to Python

**Fall 2026 Syllabus**  
*John Jay College of Criminal Justice, The City University of New York*

---

| Course information | Details |
|---|---|
| Instructor | Proma Roy |
| Class meetings | Tuesday and Thursday, 10:50 AM–12:05 PM |
| Classroom | NB L2.72.05 |
| Modality | In person |
| Instructional format | Integrated lecture and hands-on computer lab |
| Office | NB 6.63.29 |
| Office hours | By appointment; contact the instructor to arrange an in-person or online meeting |
| Email | PRoy@jjay.cuny.edu |

> **Welcome:** This is a first course in Python. No prior programming experience is expected. We will begin with the basics, practice together in class, and build confidence one small program at a time. Questions are welcome, and mistakes are a normal part of learning to program.

<a id="quick-navigation"></a>

## Quick Navigation

| Section | What you will find |
|---|---|
| [1. Course Overview](#course-overview) | Official description, course design, outcomes, and scope |
| [2. Materials and Technology](#materials-technology) | Brightspace, Google Colab, Google Drive, computer access, and textbook information |
| [3. Assessments and Grading](#assessments-grading) | Grade weights, assessment details, scale, INC, and extra credit |
| [4. Weekly Plan](#weekly-plan) | All Fall 2026 teaching dates, topics, assessments, and no-class dates |
| [5. Responsibilities and Policies](#course-policies) | Attendance, late work, collaboration, AI, integrity, and accommodations |
| [6. Student Support Resources](#student-support) | Wellness, accessibility, tutoring, basic-needs, and library resources |
| [7. Syllabus Acknowledgment](#syllabus-acknowledgment) | Student responsibility for reviewing course expectations |

<div style="page-break-after: always;"></div>

<a id="course-overview"></a>

## 1. Course Overview

### Official Course Description

This course introduces students to the process of transforming their ideas into simple but practical software through the study of a scripting language like Python. Students will learn to read and write data from various file formats, use basic data structures for data manipulation, and produce basic statistical information about the data. Programming skills will be developed through hands-on lab exercises, complemented by project-based assignments representative of current tasks in data science.

The current [John Jay Undergraduate Bulletin](https://jjay.smartcatalogiq.com/en/2025-2026/undergraduate-bulletin/course-descriptions/csci-computer-science/100/csci-171) identifies CSCI 171 as a three-hour, three-credit course.

### How This Course Is Designed

The course is practice-first and beginner-friendly. Most new ideas will follow the same pattern:

1. See a small example.
2. Predict what the code will do.
3. Run and discuss the example.
4. Change one part and observe the result.
5. Build a short program with guidance.
6. Practice independently and explain the result.

Class meetings use an integrated lecture/lab format: short explanations and live coding are followed by guided notebook work, debugging, discussion, and individual practice during the same in-person meeting. Although each meeting lasts 75 minutes, course notebooks are planned around approximately 60 usable instructional minutes so there is time for arrival, computer and Colab setup, saving, transitions, and questions. At-home practice is clearly separated from the in-class core.

The goal is not to memorize every Python feature. The goal is to learn how to break a problem into manageable steps, test those steps, and ask useful questions when code does not work yet.

### Learning Outcomes

By the end of the course, students who successfully complete the work should be able to:

1. Explain, at an introductory level, the roles of hardware, software, the CPU, memory, storage, the operating system, data, programs, and algorithms.
2. Run, edit, organize, save, and submit a Python notebook using Google Colab and Google Drive.
3. Use variables, basic data types, arithmetic, input, output, and type conversion.
4. Read, trace, and write programs that use Boolean expressions and `if`/`elif`/`else` decisions.
5. Use `while` and `for` loops to repeat tasks, count values, and accumulate results.
6. Define and call functions using parameters and return values.
7. Work with strings, lists, dictionaries, tuples, and sets at an introductory level, and choose an appropriate basic structure for a small task.
8. Read from and write to simple text and CSV files using built-in Python tools.
9. Produce basic summaries such as counts, totals, averages, minimums, maximums, and simple frequency tables.
10. Test a program with several inputs, interpret common error messages, and debug code systematically.
11. Explain their own code and use collaboration, online sources, and AI tools responsibly and transparently.

### Course Scope

#### Core topics

- Computer basics: hardware, software, CPU, memory, storage, operating systems, files, programs, instructions, and algorithms
- Python notebooks, expressions, variables, and data types
- Keyboard input, printed output, arithmetic, and type conversion
- Boolean logic and conditional statements
- `while` loops, `for` loops, `range`, counters, and accumulators
- Functions, parameters, return values, and basic variable scope
- Strings and common string operations
- Lists, iteration, indexing, slicing, and common list methods
- Dictionaries and key-value data
- Introductory use of tuples and sets
- Text and CSV file input/output
- Basic exceptions for file and input errors
- Simple descriptive summaries of data
- Testing, debugging, and clear code explanations

#### Deliberate limits for an introductory course

Recursion, lambda expressions, arbitrary argument lists, advanced sorting algorithms, classes and object-oriented programming, and third-party data-science libraries are not required course outcomes. Some may be shown briefly as optional enrichment if the class is ready. They will not appear on a graded assessment unless they have been taught and clearly announced in advance.

Students will solve the final data task with core Python. Packages such as pandas, NumPy, and scikit-learn are not required.

[↑ Back to Quick Navigation](#quick-navigation)

---

<a id="materials-technology"></a>

## 2. Materials and Technology

- **Brightspace:** The central hub for announcements, weekly readings, assignments, quizzes, project requirements, rubrics, submission instructions, feedback, grades, and schedule changes. Check it several times each week.
- **Course notebook repository:** The public notebook index is maintained at [HeyPromaRoy/csci-171-introduction-to-python](https://github.com/HeyPromaRoy/csci-171-introduction-to-python). Each instructional notebook is published only after its scheduled class meeting has ended, normally later that same day. During class, students work in their own blank Colab notebook; the released notebook becomes a post-class reference rather than an advance answer or practice sheet.
- **Python 3:** All course code will use Python 3.
- **Google Colab notebooks:** Demonstrations, guided labs, and most coding work will use [Google Colab](https://colab.research.google.com/), a browser-based environment for `.ipynb` notebooks. A dedicated Python installation, virtual environment, or Jupyter installation is not required on a student's personal computer.
- **Google account and Drive access:** Students must have access to a working Google account and Google Drive so they can open Colab, save personal notebook copies, organize course files, and continue work outside class. Students should confirm access before the first notebook meeting and contact the instructor promptly if account access creates a barrier.
- **Computer and internet access:** Students need regular access to a computer with a current web browser and internet connection. A personal laptop may be brought to class and should be charged before arrival. Students who plan to use a campus computer must still be able to sign in to their own Google account and Google Drive.
- **File backup:** Course notebooks should be saved in the student's organized CSCI 171 Google Drive folder. Important submitted work should also be retained after submission; a Colab runtime is temporary and is not a file backup.
- **Textbook and readings:** No paid textbook is required. Any required or recommended reading will be assigned separately for the appropriate week through Brightspace; readings are not bundled into the GitHub repository.

Unless an assignment says otherwise, work will be submitted through Brightspace. Students do not need to install Git, use Git commands, create a GitHub account, or submit work through GitHub in this first Python course. The public repository is a read-only distribution source for released instructional notebooks. It does not contain weekly readings, quiz questions, the midterm, the final evaluation, graded answer keys, or the official submission materials for graded work.

### Google Colab workflow

Google Colab will be the course's standard Python notebook environment. Students will learn the full setup process during the first class meeting and practice it again during the second meeting. The standard workflow is:

1. At the start of class, open a new blank notebook directly in Google Colab.
2. Rename it using the course naming convention, save it in Google Drive, and move it into the correct CSCI 171 subfolder.
3. Enter, predict, run, repair, and annotate code as directed during the live lab. Confirm that the personal notebook is saved before leaving class.
4. After the class meeting has ended, open the released instructor notebook from the [course repository README](https://github.com/HeyPromaRoy/csci-171-introduction-to-python) or its `notebooks/` folder.
5. Use the released notebook's **Open in Google Colab** badge and choose **File → Save a copy in Drive** if a separate post-class reference copy is wanted.
6. Submit any requested personal notebook file or link through Brightspace according to the assignment instructions.

Notebooks opened directly from the course repository are post-class instructor copies, not the student's in-class working notebook. No completed instructor notebook is published before or during its scheduled meeting. The repository README is the single meeting index; future links remain unavailable until the corresponding class has ended. Each released notebook includes its own **Open in Google Colab** badge. Students should keep any post-class reference copy separate from the personal notebook created during the live lab. In Colab, use **File → Open notebook → Google Drive** to reopen existing saved work.

Colab code runs on a temporary remote runtime. Variables, uploaded files, and files created only in the runtime may disappear after disconnection or inactivity. The notebook file saved in Google Drive remains, but runtime-only files do not. File-based lessons will therefore include a clearly labeled setup cell, and project instructions will explain how to upload or connect required data safely.

Google's [Colab FAQ](https://research.google.com/colaboratory/faq.html) provides additional information about notebook storage, GitHub loading, temporary runtimes, and Google Drive permissions.

[↑ Back to Quick Navigation](#quick-navigation)

---

<a id="assessments-grading"></a>

## 3. Assessments and Grading

| Assessment | Weight |
|---|---:|
| Guided notebook labs | 20% |
| Four programming assignments | 20% |
| Quizzes | 10% |
| Midterm: exam and individual coding assessment | 20% |
| Final: group project and individual reflection | 20% |
| Class participation and discussion | 5% |
| Attendance | 5% |
| **Total** | **100%** |

### Guided notebook labs — 20%

Notebook labs provide repeated practice with the exact skills being introduced. Most will begin in class. Students may ask questions and compare approaches, but each student must understand and submit their own work. The two lowest notebook-lab scores will be dropped to provide room for an early mistake, illness, or difficult week.

### Programming assignments — 20%

Four individual assignments, worth 5% each, will build gradually:

1. Input, arithmetic, and decisions
2. Loops and functions
3. Strings and lists
4. Dictionaries and file-based data

Assignments will be small enough to start early and test in parts. Grading will emphasize correct reasoning, working behavior, readable code, useful tests, and the ability to explain the submission.

### Quizzes — 10%

Two announced quizzes, worth 5% each, will check foundational ideas, code reading, prediction, and debugging. Students will not be assessed on syntax or techniques that have not been practiced in class.

### Midterm: exam and code — 20%

The midterm has two individual parts: an exam covering concepts, code reading, and tracing, plus a hands-on coding assessment. It will focus on the first half of the course: computer and programming foundations, values, variables, input/output, arithmetic, decisions, and loops. Review guidance and the point distribution will be provided before the assessment.

### Final: group project and individual reflection — 20%

The final consists of a scaffolded **group project (15%)** and an **individual reflection (5%)**. It is a small data task rather than a large software system. Using an instructor-provided or instructor-approved text/CSV file, each group will:

- read and validate data;
- organize values with appropriate basic data structures;
- compute several simple summaries;
- present the results clearly;
- test the program; and
- demonstrate and explain how the main parts work.

Each student must contribute meaningfully to the project and submit an individual reflection describing their contribution, decisions, learning, testing, and challenges. The final evaluation period will include the group demonstration and individual accountability questions. No third-party data-science library is required.

### Participation — 5%

Participation includes asking or answering questions, attempting in-class exercises, contributing respectfully to pair or group discussions, and explaining a debugging idea. Participation measures engagement, not how quickly a student finishes.

### Attendance — 5%

Attendance points are assigned before any separate departmental letter-grade penalty:

- 0 unexcused absence equivalents: 5 points
- 0.5–1 unexcused absence equivalents: 4 points
- 1.5–2 unexcused absence equivalents: 3 points
- 2.5–3 unexcused absence equivalents: 2 points
- More than 3 unexcused absence equivalents: 0 points

### Course percentage scale

| Grade | Percentage | Grade | Percentage |
|---|---:|---|---:|
| A | 93–100 | A− | 90–92.99 |
| B+ | 87–89.99 | B | 83–86.99 |
| B− | 80–82.99 | C+ | 77–79.99 |
| C | 73–76.99 | C− | 70–72.99 |
| D+ | 67–69.99 | D | 63–66.99 |
| D− | 60–62.99 | F | Below 60 |

See John Jay's [Grades policy](https://www.jjay.cuny.edu/academics/academic-resources-services/registrar/academic-standards-requirements/grades) for official grade symbols, grade-point values, withdrawals, and Pass/No Credit rules.

### Incomplete grades

An INC may be considered only when a student would otherwise be passing the course and, after consultation with the instructor, there is a reasonable expectation that the outstanding work can be completed by the last day of the following semester. An INC is not guaranteed and is assigned at the instructor's discretion. If the work is not successfully completed and no grade change is submitted, the INC becomes a FIN under College policy.

### Extra credit

Extra credit is not guaranteed. If an opportunity is offered, it will be announced to the entire class. All extra-credit work must be submitted by its posted deadline; missed opportunities cannot be extended or completed retroactively.

[↑ Back to Quick Navigation](#quick-navigation)

<div style="page-break-after: always;"></div>

<a id="weekly-plan"></a>

## 4. Weekly Plan

Brightspace is the primary source for weekly readings, exact due dates, graded activities, submission instructions, and announcements. Each public instructional notebook is released through GitHub only after that scheduled class has ended, normally later the same day. Students use their own blank Colab notebook during the live lab. The release schedule may be adjusted to match the class's learning pace; substantive changes will be announced in class and posted on Brightspace with reasonable notice.

> **Calendar check:** There are 30 possible Tuesday/Thursday meeting slots from September 1 through December 10. October 13 follows a Monday schedule, and the College is closed on November 26. The course therefore has **28 regular class meetings**. Both exceptions are shown below.

| Week | Dates | Plan and milestones |
|---:|---|---|
| 1 | Sep&nbsp;1&nbsp;and&nbsp;Sep&nbsp;3 | **Sep 1:** Course welcome; computer-system foundations; where Python and Google Colab fit; Google account check; accessing Colab; creating and organizing the `CSCI 171 - Fall 2026` Google Drive folder; saving and locating a personal notebook copy. **Sep 3:** First Google Colab notebook; code and text cells; runtime state; running cells in order; renaming and saving; `print`; values; and learning from simple errors. |
| 2 | Sep&nbsp;8&nbsp;and&nbsp;Sep&nbsp;10 | Variables and basic types; keyboard input; strings and numbers; type conversion; arithmetic; and readable output. **Lab:** small calculator/converter. |
| 3 | Sep&nbsp;15&nbsp;and&nbsp;Sep&nbsp;17 | Comparisons, Boolean expressions, and `if`/`elif`/`else`. **Assignment 1 begins.** |
| 4 | Sep&nbsp;22&nbsp;and&nbsp;Sep&nbsp;24 | **Sep 22:** More decisions, nested conditions, and boundary testing. **Sep 24:** Private Quiz 1 followed by a shortened debugging clinic and guided lab. Quiz questions and answers are not published in the repository. |
| 5 | Sep&nbsp;29&nbsp;and&nbsp;Oct&nbsp;1 | `while` loops, counters, input validation, and tracing repeated steps. **Guided loop lab.** |
| 6 | Oct&nbsp;6&nbsp;and&nbsp;Oct&nbsp;8 | `for` loops, `range`, accumulators, and simple nested-loop patterns. **Assignment 2.** |
| 7 | Oct&nbsp;13&nbsp;and&nbsp;Oct&nbsp;15 | **Oct 13: No Tuesday class—classes follow a Monday schedule.** **Oct 15:** Dedicated midterm review covering foundations, values and types, input/output, arithmetic, decisions, tracing, debugging, and loops. The review notebook contains practice patterns but no assessment questions. |
| 8 | Oct&nbsp;20&nbsp;and&nbsp;Oct&nbsp;22 | **Oct 20:** Midterm exam and individual coding assessment; no public practice notebook. **Oct 22:** Begin defining and calling functions with parameters and return values. |
| 9 | Oct&nbsp;27&nbsp;and&nbsp;Oct&nbsp;29 | Functions continued; local variables; strings, indexing, and slicing. **Guided string exercises.** |
| 10 | Nov&nbsp;3&nbsp;and&nbsp;Nov&nbsp;5 | String methods; `for` loops over text; lists and list indexing. **Assignment 3 begins.** |
| 11 | Nov&nbsp;10&nbsp;and&nbsp;Nov&nbsp;12 | List iteration and methods; copying; search patterns; and simple list summaries. **Assignment 3.** |
| 12 | Nov&nbsp;17&nbsp;and&nbsp;Nov&nbsp;19 | **Nov 17:** Dictionaries, keys, and values. **Nov 19:** Private Quiz 2 followed by frequency counting and choosing lists vs. dictionaries; Assignment 4 begins. Quiz questions and answers are not published in the repository. |
| 13 | Nov&nbsp;24&nbsp;and&nbsp;Nov&nbsp;26 | **Nov 24:** Brief introduction to tuples and sets, followed by the final group-project launch. Class time includes assignment and rubric discussion, group formation, data/question planning, responsibilities, milestones, contribution records, individual accountability, and submission expectations. **Nov 26: College closed—no class.** |
| 14 | Dec&nbsp;1&nbsp;and&nbsp;Dec&nbsp;3 | Reading and writing text files; CSV basics; `with open`; and simple exception handling. **Dec 3 project data checkpoint:** demonstrate that the approved data loads and document conversion, missing-data, or malformed-data risks. |
| 15 | Dec&nbsp;8&nbsp;and&nbsp;Dec&nbsp;10 | **Dec 8:** Counts, totals, averages, minimum/maximum, frequency tables, and a project draft-summary checkpoint. **Dec 10:** Project completion workshop, fresh-runtime testing, rubric and submission check, demonstration rehearsal, individual-accountability preparation, and independent-reflection guidance. |
| Final | Dec&nbsp;15, 10:30&nbsp;AM–12:30&nbsp;PM | **Final group-project demonstration and individual reflection. No public practice notebook is released for the final evaluation.** |

Important calendar notes are based on the [John Jay Fall 2026 Academic Calendar](https://www.jjay.cuny.edu/sites/default/files/2026-04/Fall-2026-Academic-Calendar.pdf) and [Fall 2026 Undergraduate Final Exam Schedule](https://www.jjay.cuny.edu/sites/default/files/2026-07/Fall-2026-Undergraduate-Final-Exam-Schedule.pdf). College dates are subject to change.

[↑ Back to Quick Navigation](#quick-navigation)

<div style="page-break-after: always;"></div>

<a id="course-policies"></a>

## 5. Responsibilities and Course Policies

### Course expectations and communication

This course meets twice per week in person using an integrated lecture/lab format. Students are expected to keep up with weekly materials, participate in both explanation and hands-on portions, and monitor course updates regularly. Brightspace is the central hub for announcements, weekly readings, assignments, quizzes, project instructions, rubrics, submission requirements, feedback, grades, and schedule changes. The GitHub repository distributes only the released public instructional notebooks.

- Check Brightspace several times each week.
- Complete assigned weekly readings in Brightspace before the meeting when requested.
- Open the released class notebook from the repository only after that class has ended and the post-class release is announced.
- Attend regularly and arrive on time with the materials needed to work.
- Complete quizzes, evaluations, and in-class activities at the scheduled times.
- Back up work and verify that submitted files open and run.
- Be ready to explain submitted code in plain language.
- Email or Brightspace messages will normally receive a response within 24 hours, Monday–Friday. Messages sent on weekends or College holidays may receive a response on the next business day.

### Course flexibility

To support student learning, the instructor may adapt this syllabus and weekly plan in response to class progress, demonstrated understanding, instructional needs, College calendar changes, or unforeseen circumstances. Adjustments may include the pace or sequence of topics, readings, activities, assignments, or due dates. Substantive changes will be announced in class and posted on Brightspace with reasonable notice; grading changes will not be applied retroactively to work already submitted.

### Respectful participation and collaboration

Students are expected to engage respectfully and professionally with classmates. Participation may include asking questions during demonstrations, offering ideas, discussing debugging strategies, and contributing to guided pair or group work.

Students may explain concepts and compare problem-solving strategies when collaboration is allowed. The final group project is collaborative, but each student must make a documented contribution and complete the reflection independently. Sharing a complete solution on other individual work, copying code, or allowing another person to complete individual work is not permitted. Respect the different experience levels, backgrounds, names, and perspectives represented in the classroom.

### Departmental attendance policy

Regular attendance is expected and essential to success in the course. Students are responsible for all material, announcements, and assignments covered in class, whether present or not.

- **Unexcused absences:** More than 3 unexcused absence equivalents in the semester will result in a one-full-letter-grade penalty, such as B to C or B+ to C+. Additional unexcused absences may result in further letter-grade penalties and may result in a failing grade.
- **Excused absences:** Documented illness, religious observance, family emergency, jury duty, or military service requires notification and, where possible, documentation within 2 class meeting days.
- **Late arrival or early departure:** Arriving more than 15 minutes late or leaving more than 15 minutes early counts as one-half absence. Two partial absences equal one full absence.
- **Missed material:** It is the student's responsibility to obtain missed notes, materials, and announcements from a classmate and to review Brightspace.
- **Make-up work:** Work missed because of an excused absence must be arranged with the instructor within 1 week of returning to class.

Approved Office of Accessibility Services accommodations will be applied as authorized. This policy will be reviewed during the first class meeting and posted on Brightspace.

### Late work and make-up policy

- **Notebook labs, quizzes, and participation tasks:** Complete these on time. They generally cannot be made up after answers or feedback have been discussed, except when an excused absence qualifies for make-up work under the attendance policy.
- **Programming assignments and project checkpoints:** Work may be submitted up to 3 days late only when the student contacts the instructor before the due date. Approved late submissions may receive up to a 20% deduction.
- **Midterm and final evaluation:** These must be completed on the scheduled dates unless the student has a documented emergency or an approved accommodation.

If a student is falling behind, contacting the instructor early is strongly encouraged. Asking for help does not reduce a grade.

### Use of AI tools

AI tools may support learning when used thoughtfully, but they may not replace the student's own programming and reasoning.

**Allowed unless an assignment says otherwise:**

- asking for an explanation of an error message after making an attempt;
- asking for a simpler explanation of a concept;
- requesting an additional practice problem that is different from the graded problem; and
- asking for feedback on code the student wrote, without asking the tool to replace the solution.

**Not allowed unless explicitly authorized:**

- asking an AI tool to generate all or part of a graded solution;
- copying AI-generated code into a submission and presenting it as the student's own work;
- using AI during a quiz, midterm, final check, or other closed-resource activity; or
- using an AI tool to hide, rewrite, or misrepresent the source of submitted work.

Any permitted AI help used on graded work must be disclosed in an **AI-use note** at the end of the notebook or submission. The note must identify the tool, date, purpose, and prompt. Students must keep the relevant conversation and be prepared to show it if requested. Students must also be able to explain every line they submit.

Example: *Used ChatGPT on October 29, 2026, to explain why my loop skipped the last value. Prompt: “Explain this error without rewriting my assignment solution: [code].” I then corrected and tested the code myself.*

When unsure whether a use is permitted, ask the instructor before using the tool.

### Academic integrity

Academic dishonesty is prohibited. Penalties may include academic sanctions, such as a failing or reduced grade, and disciplinary sanctions, including suspension or expulsion.

**Cheating** is the unauthorized use or attempted use of materials, information, notes, study aids, devices, collaboration, or communication during an academic exercise. Examples include copying or sharing answers, collaborating when collaboration is not authorized, having another person complete work, completing work for another student, or using unauthorized websites, devices, or AI tools.

**Plagiarism** is presenting another person's ideas, writing, code, media, or computer-generated content as one's own without appropriate attribution. This includes copying or paraphrasing from online sources without acknowledgment, failing to identify collaborators, or submitting AI-generated content as original work.

Students must credit all permitted external help and be prepared to explain submitted code. If unsure whether a resource or form of collaboration is allowed, ask before submitting. Review the [John Jay Academic Integrity Office](https://www.jjay.cuny.edu/about/senior-leadership/academic-affairs/academic-integrity-office) for College policy and process information.

### Accessibility services

Students who believe they may need an accommodation for a temporary or permanent disability are encouraged to contact the [Office of Accessibility Services](https://www.jjay.cuny.edu/student-life/wellness-center/accessibility-services) at [accessibilityservices@jjay.cuny.edu](mailto:accessibilityservices@jjay.cuny.edu). OAS handles disability documentation and coordinates approved academic adjustments.

Students are welcome, but not required, to discuss course-specific needs with the instructor privately. A student does not need to disclose a diagnosis or the specific nature of a disability to the instructor. Please contact OAS and the instructor as early as possible so approved accommodations can be implemented.

### Religious accommodations

Students seeking an accommodation for a sincerely held religious belief should contact the instructor and the appropriate Student Affairs office as early as possible. CUNY policy provides an equivalent opportunity to make up examinations, study, or work requirements missed for religious observance. See the [CUNY Religious Accommodations policy](https://www.cuny.edu/about/administration/offices/legal-affairs/policies-resources/reasonable-accommodations-and-academic-adjustments/religious-accommodations/).

[↑ Back to Quick Navigation](#quick-navigation)

---

<a id="student-support"></a>

## 6. Student Support Resources

Seeking support early is a responsible step. John Jay resources include:

- [Wellness Center](https://www.jjay.cuny.edu/student-life/wellness-center) — health, counseling, crisis, accessibility, and other wellness services.
- [Emergency Funding and Basic-Needs Support](https://www.jjay.cuny.edu/student-life/wellness-center/emergency-funding) — emergency grants, food pantry, book and meal vouchers, transportation assistance, and related resources.
- [Office of Accessibility Services](https://www.jjay.cuny.edu/student-life/wellness-center/accessibility-services) — registration, accommodations, exam requests, and assistive technology.
- [Math and Science Resource Center](https://www.jjay.cuny.edu/academics/academic-resources-services/tutoring-academic-support/math-science-resource-center) — tutoring and academic support; check current services and schedules.
- [Lloyd Sealy Library](https://www.lib.jjay.cuny.edu/) — research help, study space, technology, and course resources.

[↑ Back to Quick Navigation](#quick-navigation)

---

<a id="syllabus-acknowledgment"></a>

## 7. Syllabus Acknowledgment

Students are responsible for reading this syllabus, checking Brightspace, and asking questions about any expectation that is unclear. Continuing in the course means working within these policies, including the attendance, academic integrity, collaboration, and AI-use expectations.

[↑ Back to Top](#top)

---

*Prepared for Fall 2026. Last updated August 26, 2026.*
