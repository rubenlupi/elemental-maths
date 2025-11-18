# 🎯 MASTER TOPIC GENERATOR PROMPT

This prompt orchestrates the complete creation of a mathematics topic module using the existing theory and exam generation prompts.

---

## 📥 INPUT REQUIREMENTS

Provide the following information:

### 1. Topic Information
```
**Topic Name:** [Name of the mathematical topic]
Example: "Fractions and Operations"

**Module Number:** [Optional - if part of a sequence]
Example: "Module 9"
```

### 2. Language Selection
```
**Language:** [Choose one]
Options: Catalan, English, Spanish
Default: Catalan
```

### 3. Concepts to Cover
```
**Concepts List:**
- [Concept 1]
- [Concept 2]
- [Concept 3]
...

Example:
- What is a fraction (numerator, denominator)
- Equivalent fractions
- Comparing fractions
- Adding fractions with same denominator
```

### 4. Target Level (Optional)
```
**Educational Level:** [Target audience]
Examples: 
- Primary school (10-12 years)
- Secondary school (12-16 years)
- Gifted students (8-10 years with advanced curriculum)
```

---

## 🔧 EXECUTION PROCESS

This prompt will execute the following steps automatically:

### Step 1: Create Folder Structure
Create a folder with the topic name (normalized, lowercase, hyphens):
```
docs/[topic-name]/
```

Example: `docs/fractions-operations/`

### Step 2: Generate Theory Document
Using the **general-theory-prompt.md**, create:
```
docs/[topic-name]/teoria.md
```

The theory will include:
- All concepts with clear definitions
- Multiple examples per concept
- Visual representations (diagrams, number lines, tables)
- Properties and rules
- Common misconceptions addressed
- All content in the selected language

### Step 3: Generate Exam
Using the **general-exam-prompt.md**, create:
```
docs/[topic-name]/exam_YYYYMMDD_HHMMSS/
  ├── exercises.md
  └── solutions.md
```

The exam will include:
- 10 exercises covering all theory concepts
- Total of 10 points distributed appropriately
- Mix of difficulties (3 moderate, 5 intermediate, 2 challenging)
- Minimum 5 exercises with reverse reasoning
- Complete solutions with step-by-step justifications
- All content in the selected language

### Step 4: Create Reference Prompt (Optional)
Copy the exam prompt to the topic folder for future exam generation:
```
docs/[topic-name]/exam-prompt.md
```

---

## 📋 FOLDER STRUCTURE OUTPUT

After execution, you will have:

```
docs/[topic-name]/
├── teoria.md                           # Theory document
├── exam-prompt.md                      # Prompt for generating future exams
└── exam_YYYYMMDD_HHMMSS/              # First exam
    ├── exercises.md                    # Student version
    └── solutions.md                    # Teacher version with solutions
```

---

## 🎯 EXECUTION INSTRUCTIONS

### For the AI Assistant:

When this prompt is invoked:

1. **Parse the input** to extract:
   - Topic name
   - Language
   - Concepts list
   - Target level

2. **Create the folder structure:**
   - Normalize topic name (lowercase, replace spaces with hyphens)
   - Create `docs/[topic-name]/` directory

3. **Generate theory document:**
   - Apply the **general-theory-prompt.md** guidelines
   - Use the provided concepts list
   - Adapt to the target level
   - Write entirely in the selected language
   - Save as `docs/[topic-name]/teoria.md`

4. **Generate exam:**
   - Apply the **general-exam-prompt.md** guidelines
   - Use the theory document as reference
   - Cover all concepts from the theory
   - Create timestamped folder: `exam_YYYYMMDD_HHMMSS`
   - Generate both `exercises.md` and `solutions.md`
   - Write entirely in the selected language

5. **Create exam prompt reference:**
   - Copy or create a specific exam prompt for this topic
   - Include topic-specific requirements
   - Save as `docs/[topic-name]/exam-prompt.md`

6. **Confirm completion:**
   - List all files created
   - Provide file paths
   - Summarize what was generated

---

## 💡 USAGE EXAMPLE

### Input:
```
**Topic Name:** Integers and Operations
**Language:** Catalan
**Module Number:** Module 2
**Educational Level:** Gifted students (9-11 years)

**Concepts to Cover:**
- Positive and negative numbers
- Number line representation
- Absolute value
- Comparing integers
- Adding integers (same sign, different signs)
- Subtracting integers
- Integer word problems
- Real-world applications (temperature, elevation, debt)
```

### Expected Output:
```
✅ Created topic module: Integers and Operations

📁 Folder structure:
docs/integers-operations/
├── teoria.md (Complete theory in Catalan)
├── exam-prompt.md (Future exam generation prompt)
└── exam_20251118_143052/
    ├── exercises.md (10 exercises, 10 points)
    └── solutions.md (Complete solutions)

📊 Content summary:
- Theory: 8 concepts covered with examples
- Exam: 10 exercises (3 moderate, 5 intermediate, 2 challenging)
- Language: Catalan throughout
- Target level: Gifted students (9-11 years)
```

---

## ⚙️ CONFIGURATION OPTIONS

### Language Templates

**Catalan:**
- Headers: "EXERCICIS", "SOLUCIONS", "Nom:", "Data:"
- Point format: "1.5 punts"
- Total: "PUNTUACIÓ TOTAL: ___ / 10 punts"

**English:**
- Headers: "EXERCISES", "SOLUTIONS", "Name:", "Date:"
- Point format: "1.5 points"
- Total: "TOTAL SCORE: ___ / 10 points"

**Spanish:**
- Headers: "EJERCICIOS", "SOLUCIONES", "Nombre:", "Fecha:"
- Point format: "1.5 puntos"
- Total: "PUNTUACIÓN TOTAL: ___ / 10 puntos"

### Difficulty Distribution
- **Moderate (3 exercises):** 0.8-1.0 points each
- **Intermediate (5 exercises):** 1.0-1.3 points each
- **Challenging (2 exercises):** 1.5 points each
- **Total:** Exactly 10 points

---

## ✅ QUALITY CHECKLIST

Before completing, verify:

**Folder Structure:**
- [ ] Topic folder created with normalized name
- [ ] Theory file exists and is complete
- [ ] Exam folder exists with timestamp
- [ ] Both exercise and solution files exist
- [ ] Exam prompt reference file created

**Theory Document:**
- [ ] All concepts from input are covered
- [ ] Each concept has definition + examples
- [ ] Visual representations included where appropriate
- [ ] Language is consistent throughout
- [ ] Appropriate for target level
- [ ] Mathematical notation is correct

**Exam Document:**
- [ ] Exactly 10 exercises
- [ ] Points total to 10
- [ ] Difficulty distribution: 3-5-2
- [ ] Exercises cover all theory concepts
- [ ] At least 5 exercises use reverse reasoning
- [ ] Solutions are complete with justifications
- [ ] Language matches theory document
- [ ] File structure and formatting are correct

---

## 🔄 GENERATING ADDITIONAL EXAMS

After initial setup, to generate more exams for the same topic:

1. Navigate to `docs/[topic-name]/`
2. Read `teoria.md` for reference
3. Use `exam-prompt.md` (or general-exam-prompt.md)
4. Specify the same language
5. New exam will be created in new timestamped folder

This preserves all previous exams without overwriting.

---

## 🚀 QUICK START COMMAND

```
Create a complete topic module:

Topic: [Your topic name]
Language: [Catalan/English/Spanish]
Level: [Target educational level]

Concepts:
- [Concept 1]
- [Concept 2]
- ...

Use the master-topic-generator prompt to create theory + exam.
```

---

## 📌 NOTES

- All mathematical notation should follow standard conventions
- Visual elements (Venn diagrams, number lines) should use ASCII art
- Examples should progress from simple to complex
- Real-world applications should be age-appropriate
- Exams should test understanding, not just memorization
- Each concept should connect to previous learning where possible
- Theory should explain "why" not just "how"



## 📌 EXAMPLE

Genera lo siguiente:

**Topic Name:** Number Systems and Number Theory Foundations
**Language:** Catalan
**Educational Level:** Gifted students 9-10 years)
**Day 1**

Use the master-topic-generator prompt to create theory + exam.

Use the main-index to see the topics of the day.