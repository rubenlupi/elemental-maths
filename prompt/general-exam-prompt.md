# 🟦 GENERAL EXAM GENERATOR PROMPT

**LANGUAGE:** Generate all content in **CATALAN**.

You will receive:
1. **Theory content** - The educational material/concepts to be tested
2. **Topic requirements** - Specific topics and concepts to cover in the exam

Based on these inputs, generate **TWO separate files in Markdown format** with 10 math exercises.

---

## 📥 INPUT FORMAT

When using this prompt, provide:

### 1. Theory Content
```
[Paste or reference the theory document that contains the concepts to be tested]
```

### 2. Topic Requirements
```
[List the specific topics, concepts, operations, or skills to cover in the exam]
```

---

## 📁 FILE ORGANIZATION

**IMPORTANT:** Create a new folder with the following name format:
```
exam_YYYYMMDD_HHMMSS
```

Where:
- `YYYY` = year (4 digits)
- `MM` = month (2 digits)
- `DD` = day (2 digits)
- `HH` = hour (2 digits, 24h format)
- `MM` = minutes (2 digits)
- `SS` = seconds (2 digits)

**Example:** `exam_20251118_143052` (November 18, 2025, 14:30:52)

Inside this folder, create two files:
1. `exercises.md` - File for the student
2. `solutions.md` - File with complete answers

**Advantage:** Each time you generate a new exam, a unique folder will be created without overwriting previous ones.

---

## 📋 FORMAT REQUIREMENTS

### File 1: exercises.md
- **Exam format:** each exercise with clear point value (e.g.: "(1.5 points)", "(2 points)")
- **Point distribution:** total must add up to 10 points
- **Space for answers:** after each question, include blank lines or clearly marked sections where the student can write
- **No solutions:** this file only contains problem statements
- **Header:** Include space for student name and date

### File 2: solutions.md
- **Same order:** exercises numbered the same as file 1
- **Complete development:** each solution with step-by-step justification
- **Detailed explanations:** include reasoning and intermediate calculations
- **Mathematical rigor:** use proper notation and terminology from the theory
- **Include tips when relevant:** Add brief memory tricks or shortcuts ("Truc:", "Drecera:") - max 1 line
- **Add context:** When appropriate, mention practical applications or interesting facts - keep concise

---

## 🎯 CONTENT REQUIREMENTS

### Exercise Design Principles:

#### 1. **Difficulty Distribution**
- **3 moderate exercises** (0.8-1.0 points each): Direct application of basic concepts
- **5 intermediate exercises** (1.0-1.3 points each): Require multiple steps or concept combination
- **2 challenging exercises** (1.5 points each): Complex problem-solving with reverse reasoning

#### 2. **Cognitive Diversity**
Include exercises that require:
- **Direct recall/application**: Apply formulas or definitions directly
- **Procedural fluency**: Execute algorithms and calculations
- **Conceptual understanding**: Explain why something works
- **Problem-solving**: Analyze, deduce, and discover from incomplete information
- **Reverse reasoning**: Work backwards from results to find initial conditions
- **Pattern recognition**: Identify relationships and structures

#### 3. **Representation Variety**
Use multiple formats:
- Explicit numerical/algebraic expressions
- Verbal descriptions requiring translation to math
- Visual representations (diagrams, tables, graphs, ASCII art)
- Real-world contexts and applied problems (shopping, sports, cooking, travel, etc.)
- Abstract mathematical scenarios
- Include at least 2-3 exercises with practical real-world contexts

#### 4. **Conceptual Traps (Subtle, Not Obvious)**
Include challenges that require careful analysis:
- Edge cases and special situations
- Conditions that appear to contradict but don't
- Numbers/elements that almost meet criteria but fail on one detail
- Common misconceptions that need to be addressed
- Distinctions between similar concepts

#### 5. **Technical Requirements**
- Each exercise must have **unique and elegant solution**
- Use correct mathematical notation from the theory
- Must NOT be trivial or solvable by simple inspection
- Include full justification in solutions
- Ensure exercises test different aspects of the theory
- Align with learning objectives from the theory document
- Include practical/real-world problems to show relevance (at least 2-3)
- Keep solutions focused - add tips/tricks only when they genuinely help (avoid unnecessary fluff)

---

## 📝 OUTPUT STRUCTURE

### FILE 1: exercises.md

````markdown
# EXERCISES — [Topic Name]

**Name:** ________________________________  **Date:** ______________

---

**Exercise 1** (X points)
[Problem statement - clear, concise, unambiguous]

**Answer:**

[Sufficient blank space for student work]

_________________________________________________________________________________

_________________________________________________________________________________

---

**Exercise 2** (X points)
[Problem statement with sub-sections if applicable]

**a)** [First part]

**Answer:** _________________________________________________

**b)** [Second part]

**Answer:** _________________________________________________

---

[...continue with all exercises...]

---

**TOTAL SCORE: _____ / 10 points**
````

### FILE 2: solutions.md

````markdown
# SOLUTIONS — [Topic Name]

---

**Exercise 1** (X points)

**Answer:** [Direct, complete answer]

**Justification:**
[Detailed step-by-step development with explanations]
- Step 1: [Action and reasoning]
- Step 2: [Action and reasoning]
- Step 3: [Action and reasoning]
- Conclusion: [Final interpretation/verification]

[Include relevant formulas, theorems, or definitions from theory]
[Optional: **Truc:** Add brief memory trick or shortcut if helpful - 1 line max]
[Optional: **Curiositat:** Add interesting fact if relevant - max 2 lines]

---

**Exercise 2** (X points)

**a)** [Answer for section a]

**Justification:** [Detailed explanation with references to theory]

**b)** [Answer for section b]

**Justification:** [Detailed explanation with references to theory]

---

[...continue with all solutions...]
````

---

## 🎓 THEORY ALIGNMENT GUIDELINES

When creating exercises from theory:

1. **Map to learning objectives**: Ensure exercises cover all main concepts from the theory
2. **Use theory notation**: Match symbols, terminology, and conventions exactly
3. **Reference definitions**: Base problems on definitions and properties from theory
4. **Progressive complexity**: Start with foundational concepts, build to complex applications
5. **Balance coverage**: Don't over-focus on one topic; distribute across theory sections
6. **Test understanding, not memorization**: Require application and reasoning, not just recall

---

## ⚠️ EXECUTION CHECKLIST

Before generating, verify:
- [ ] Theory content has been reviewed and understood
- [ ] Topic requirements have been identified
- [ ] Folder name follows format: `exam_YYYYMMDD_HHMMSS`
- [ ] Both files will be generated completely
- [ ] Points add up to exactly 10
- [ ] Exercises test different aspects of theory
- [ ] Difficulty is appropriately distributed
- [ ] Solutions include complete justifications
- [ ] Language is CATALAN throughout

---

## 📤 OUTPUT FORMAT

**First:** Announce the folder name:
```
Creating exam folder: exam_YYYYMMDD_HHMMSS
```

**Second:** Generate both files with clear separators:
```
=== FILE 1: exercises.md ===
[Complete content]

=== FILE 2: solutions.md ===
[Complete content]
```

---

## 💡 USAGE EXAMPLE

```
I have the following theory about [topic]:
[paste theory content]

And I want to test these concepts:
- [Concept 1]
- [Concept 2]
- [Concept 3]
...

Please generate an exam following the general exam prompt.
```
