# 🟦 GENERAL THEORY GENERATOR PROMPT

**LANGUAGE:** Generate all content in **CATALAN**.

You will receive:
1. **Topic/Module name** - The subject to create theory for
2. **Concepts to cover** - List of specific concepts, definitions, and skills
3. **Target level** (optional) - Educational level or age group

Based on these inputs, generate a comprehensive theory document in Markdown format.

---

## 📥 INPUT FORMAT

When using this prompt, provide:

### 1. Topic/Module Name
```
[Name of the mathematical topic or module]
Example: "Sets and Number Types"
```

### 2. Concepts to Cover
```
[List all concepts, definitions, operations, or skills that should be explained]
Example:
- What is a set
- Set operations (union, intersection, difference)
- Prime and composite numbers
- etc.
```

### 3. Target Level (Optional)
```
[Educational level: primary, secondary, high school, university]
[Or age range: 10-12 years old, 13-15 years old, etc.]
```

### 4. Weekly Session Planning (Optional)
```
[Specify if the module should be divided into weekly sessions]
Default: Single comprehensive document
Alternative: Divide into 5-7 daily sessions (10 min theory + 10 min exercises each)
```

---

## 📋 THEORY STRUCTURE REQUIREMENTS

### Document Organization Options

#### Option A: Comprehensive Single Document (Default)
```markdown
# 🟦 MODULE [NUMBER] — [Topic Name] (Theory)

## 🔹 [Concept 1 Name]
[Content for concept 1]

## 🔹 [Concept 2 Name]
[Content for concept 2]

[...continue for all concepts...]
```

#### Option B: Weekly Session Structure (For Progressive Learning)
When a module has many concepts, divide into 5-7 daily sessions that fit into one week:
- **Each session:** 10 minutes theory + 10 minutes exercises
- **File structure:** Create separate files for each day

```markdown
# 🟦 MODULE [NUMBER] — [Topic Name] (Weekly Plan)

## 📅 Session Structure

### Day 1: [Sub-topic Name] (20 min total)
**Theory (10 min):**
- [Concept 1.1]
- [Concept 1.2]

**Exercises (10 min):**
- [2-3 quick exercises to practice the concepts]

### Day 2: [Sub-topic Name] (20 min total)
**Theory (10 min):**
- [Concept 2.1]
- [Concept 2.2]

**Exercises (10 min):**
- [2-3 quick exercises to practice the concepts]

[...continue for 5-7 days...]

### Weekly Review (Optional Day 7)
- Summary of all concepts
- Mixed practice exercises
- Connections between concepts
```

**When to use weekly sessions:**
- Complex modules with 15+ concepts
- Students need gradual concept building
- Daily practice is preferred over intensive study
- Module covers multiple related sub-topics

**When to use single document:**
- Fewer than 10 concepts
- Concepts are closely related
- Intensive study session is appropriate
- Quick reference document needed

### For Each Concept Include:

#### 1. **Clear Definition**
- Start with a precise, understandable definition
- Use bold for key terms
- Keep language appropriate to the target level

#### 2. **Multiple Examples**
- Provide at least 2-3 concrete examples
- Use diverse scenarios (numbers, real-world contexts, visual representations)
- Progress from simple to more complex
- Show both what IS and what IS NOT the concept (counterexamples)

#### 3. **Mathematical Notation**
- Introduce symbols clearly with explanation
- Show notation in context with examples
- Use consistent notation throughout
- Provide both symbolic and verbal forms

#### 4. **Visual Representations** (when applicable)
- ASCII diagrams
- Number lines
- Tables
- Venn diagrams
- Step-by-step illustrations

#### 5. **Key Properties or Rules**
- List important properties, rules, or patterns
- Explain WHY they work (intuitive reasoning)
- Highlight special cases or exceptions

#### 6. **Common Misconceptions** (when relevant)
- Address typical errors or confusions
- Clarify distinctions between similar concepts
- Provide notes to prevent misunderstandings

#### 7. **Connections to Other Concepts**
- Show relationships to previously learned material
- Indicate how this concept will be used later
- Build conceptual bridges

#### 8. **Practical Applications & Memory Tricks**
- Include 1-2 real-world applications (keep brief, 1-2 sentences)
- Add memory tricks or mnemonics when helpful ("Truc:", "Recorda:")
- Share interesting anecdotes or curiosities ("Curiositat:", "Sabies que...?")
- Keep each addition concise (max 2-3 lines) to avoid lengthy content

---

## 🎯 CONTENT REQUIREMENTS

### Language and Clarity:
- **Simple and precise**: Avoid jargon unless necessary; define technical terms
- **Active voice**: "We use this to..." rather than "This is used to..."
- **Conversational yet rigorous**: Friendly tone while maintaining mathematical accuracy
- **Age-appropriate**: Adjust complexity to target level

### Pedagogical Principles:
- **Concrete to abstract**: Start with tangible examples before formal definitions
- **Incremental complexity**: Build understanding step by step
- **Multiple modalities**: Text, symbols, visuals, examples
- **Why before how**: Explain reasoning and intuition, not just procedures
- **Engage with context**: Add brief real-world applications, memory tricks, and fun facts
- **Keep it concise**: Every addition should be purposeful and brief (avoid lengthy tangents)
- **Engage with context**: Add brief real-world applications, memory tricks, and fun facts
- **Keep it concise**: Every addition should be purposeful and brief (avoid lengthy tangents)

### Mathematical Rigor:
- **Precise definitions**: Use standard mathematical terminology
- **Correct notation**: Follow conventional mathematical symbols
- **Complete explanations**: Don't skip logical steps
- **Verify examples**: Ensure all calculations and examples are correct

### Formatting Standards:
- Use **bold** for key terms and definitions
- Use `code formatting` for numbers, sets, and inline math expressions
- Use bullet points for lists
- Use proper hierarchy (##, ###) for sections
- Include emoji icons (🔹) for visual organization
- Leave blank lines between sections for readability

---

## 📝 OUTPUT TEMPLATE

### Template A: Single Comprehensive Document

```markdown
# 🟦 MODULE [N] — [Topic Name] (Theory)

## 🔹 [Concept 1 Title]
- **[Key term]:** [Clear definition in simple language]
  - Example 1: [Concrete example with explanation]
  - Example 2: [Different type of example]
  - Counterexample: [What this is NOT]
- **Notation:** [Symbol or mathematical notation with explanation]
  - Example: [Notation in use]
- **Key property:** [Important rule or pattern]
  - Explanation: [Why this is true]

## 🔹 [Concept 2 Title]
- **[Key term]:** [Definition]
  - Example: [Visual or numerical example]
  - Real-world context: [Applied situation]
- **How to identify:** [Practical method or test]
- **Special cases:** [Exceptions or edge cases]
- **Truc:** [Memory trick or quick recognition method - keep to 1 line]
- **Curiositat:** [Brief interesting fact or anecdote - max 2 lines]
- **Note:** [Important clarification or common mistake to avoid]

[...continue with all concepts...]
```

### Template B: Weekly Session Structure

```markdown
# 🟦 MODULE [N] — [Topic Name] (Weekly Learning Plan)

**Total duration:** 5-7 days × 20 minutes = 100-140 minutes
**Structure:** 10 min theory + 10 min exercises per day

---

## 📅 DAY 1: [Sub-topic Name]

### 📖 Theory (10 minutes)

#### 🔹 [Concept 1.1]
- **Definition:** [Concise, clear definition]
- **Key example:** [One main example with explanation]
- **Quick tip:** [Memory aid or recognition method]

#### 🔹 [Concept 1.2]
- **Definition:** [Concise, clear definition]
- **Key example:** [One main example]
- **Connection:** [How it relates to previous concept]
- **Aplicació pràctica:** [One real-world use - 1 sentence]
- **Truc:** [Quick memory aid - 1 line, if applicable]

### ✏️ Exercises (10 minutes)

**Exercise 1:** [Quick practice problem for concept 1.1]
**Solution:** [Brief answer with key reasoning]

**Exercise 2:** [Quick practice problem for concept 1.2]
**Solution:** [Brief answer with key reasoning]

**Exercise 3:** [Combined problem using both concepts]
**Solution:** [Brief answer showing integration]

---

## 📅 DAY 2: [Sub-topic Name]

### 📖 Theory (10 minutes)

#### 🔹 [Concept 2.1]
[Content structured like Day 1]

#### 🔹 [Concept 2.2]
[Content structured like Day 1]

### ✏️ Exercises (10 minutes)
[2-3 exercises like Day 1]

---

[...continue for Days 3-6...]

---

## 📅 DAY 7: Weekly Review & Integration (Optional)

### 📖 Review (10 minutes)
- **Summary of key concepts:**
  - Day 1: [Brief summary]
  - Day 2: [Brief summary]
  - [Continue for all days]
- **Concept map:** [Visual connections between all concepts]
- **Key formulas/rules:** [Quick reference list]

### ✏️ Mixed Practice (10 minutes)
**Exercise 1:** [Combines concepts from Days 1-2]
**Exercise 2:** [Combines concepts from Days 3-4]
**Exercise 3:** [Combines concepts from Days 5-6]
**Challenge:** [Uses all concepts from the week]

---

## 📊 Module Summary
[Overall learning outcomes and next steps]
```

### Guidelines for 10-Minute Theory Sections:
- **Focus on essentials:** 1-2 main concepts maximum
- **One strong example each:** Quality over quantity
- **Clear definitions:** Simple language, bold key terms
- **Visual aids:** Use diagrams/tables when possible (ASCII art)
- **No fluff:** Every sentence adds value

### Guidelines for 10-Minute Exercise Sections:
- **2-3 exercises:** Can be completed in 10 minutes
- **Progressive difficulty:** Start easy, build up
- **Immediate feedback:** Solutions provided right after
- **Purposeful practice:** Each exercise targets specific concept
- **Variety:** Different problem types (calculation, conceptual, applied)
- **Include practical problems:** At least 1 exercise should have real-world context
- **Add solution tricks:** In solutions, mention shortcuts or memory aids when relevant (1 line max)

---

## 📝 ORIGINAL OUTPUT TEMPLATE (for reference)

## 🔹 [Concept 1 Title]
- **[Key term]:** [Clear definition in simple language]
  - Example 1: [Concrete example with explanation]
  - Example 2: [Different type of example]
  - Counterexample: [What this is NOT]
- **Notation:** [Symbol or mathematical notation with explanation]
  - Example: [Notation in use]
- **Key property:** [Important rule or pattern]
  - Explanation: [Why this is true]

## 🔹 [Concept 2 Title]
- **[Key term]:** [Definition]
  - Example: [Visual or numerical example]
  - Real-world context: [Applied situation]
- **How to identify:** [Practical method or test]
- **Special cases:** [Exceptions or edge cases]
- **Note:** [Important clarification or common mistake to avoid]

## 🔹 [Concept 3 with Visual Representation]
[Brief introduction]

**Visual representation:**
```
[ASCII diagram, number line, or table]
```

**Explanation:**
- Point 1: [What the visual shows]
- Point 2: [Key observation]

**Examples:**
- Example 1: [Detailed walkthrough]
  - Step 1: ...
  - Step 2: ...
  - Result: ...
- Example 2: [Different scenario]

## 🔹 [Concept 4 with Operations/Procedures]
**Definition:** [What this operation does]

**How it works:**
1. [Step 1 with explanation]
2. [Step 2 with explanation]
3. [Step 3 with explanation]

**Examples:**
- Simple case: [Easy example]
  - Calculation: [Show work]
  - Result: [Answer with interpretation]
- Complex case: [Challenging example]
  - Setup: [Initial information]
  - Process: [Detailed solution]
  - Verification: [Check the answer]

**General form:** [Algebraic or abstract representation if applicable]

[...continue with all concepts...]
```

---

## 🎓 QUALITY CHECKLIST

### For Single Document Format:
- [ ] All requested concepts are covered completely
- [ ] Each concept has: definition, examples, notation, explanation
- [ ] Examples are diverse and progress in difficulty
- [ ] Mathematical notation is introduced and explained
- [ ] Language is appropriate for target level
- [ ] No logical gaps or unexplained jumps
- [ ] Visual elements enhance understanding
- [ ] Common errors or misconceptions are addressed
- [ ] Concepts are connected to each other
- [ ] Formatting is consistent and clear
- [ ] All mathematical statements are accurate
- [ ] Language is CATALAN throughout

### For Weekly Session Format (Additional Checks):
- [ ] Module is divided into 5-7 manageable daily sessions
- [ ] Each session has exactly 10 min theory + 10 min exercises
- [ ] Theory sections are focused (1-2 concepts max per day)
- [ ] Exercises are completable in 10 minutes (2-3 problems)
- [ ] Progressive difficulty across the week
- [ ] Each day builds on previous days
- [ ] Day 7 provides comprehensive review (if included)
- [ ] Solutions are provided for all exercises
- [ ] Total weekly time: 100-140 minutes
- [ ] Clear learning objectives for each day
- [ ] Concepts are logically grouped by day

---

## 💡 USAGE EXAMPLE

### Example 1: Single Document Request

```
I need theory for the following topic:

**Topic:** Fractions and Operations
**Target level:** Primary school (10-12 years old)
**Format:** Single comprehensive document

**Concepts to cover:**
- What is a fraction (numerator, denominator)
- Visual representation with diagrams
- Equivalent fractions
- Comparing fractions
- Addition of fractions with same denominator
- Real-world applications

Please generate the theory document following the general theory prompt.
```

### Example 2: Weekly Session Request

```
I need theory for the following topic:

**Topic:** Introduction to Algebra
**Target level:** Secondary school (12-14 years old)
**Format:** Weekly sessions (5-7 days, 10 min theory + 10 min exercises each)

**Concepts to cover:**
- Variables and expressions
- Evaluating expressions
- Like terms and combining them
- Writing expressions from word problems
- Simple equations
- Solving one-step equations
- Solving two-step equations
- Checking solutions
- Word problems to equations

Please divide this into a weekly learning plan with daily 20-minute sessions following the general theory prompt.
```

**Expected output for Example 2:**
- Day 1: Variables and expressions + evaluating (3 exercises)
- Day 2: Like terms and combining (3 exercises)
- Day 3: Writing expressions from words (3 exercises)
- Day 4: Introduction to equations + one-step (3 exercises)
- Day 5: Two-step equations + checking (3 exercises)
- Day 6: Word problems to equations (3 exercises)
- Day 7: Weekly review + mixed practice

---

## 📤 OUTPUT FORMAT

**First:** Confirm understanding:
```
Creating theory document for: [Topic Name]
Target level: [Level]
Format: [Single document / Weekly sessions]
Concepts covered: [List]
[If weekly: Expected duration: X days × 20 min = Y minutes total]
```

**Second:** Generate complete theory document in CATALAN following the appropriate template structure (single document or weekly sessions).

---

## 🌟 ADDITIONAL GUIDELINES

### For Different Levels:

**Primary (6-12 years):**
- Very concrete examples (apples, toys, everyday objects)
- Simple language, short sentences
- Lots of visual representations
- Hands-on activities suggestions
- Connection to play and daily life

**Secondary (12-16 years):**
- Balance concrete and abstract
- Introduce formal notation gradually
- Real-world applications and contexts
- Problem-solving strategies
- Conceptual connections between topics

**High School/University (16+ years):**
- Formal definitions and proofs
- Abstract reasoning emphasis
- Rigorous mathematical notation
- Theoretical foundations
- Advanced applications and generalizations

### Special Considerations:

- **Build vocabulary gradually**: Define terms when first introduced
- **Use analogies**: Compare to familiar concepts when possible
- **Scaffold complexity**: Start simple, add layers of sophistication
- **Provide context**: Explain why this matters and where it's used
- **Encourage exploration**: Pose questions that prompt deeper thinking
- **Add engagement elements**: Include brief practical applications, memory tricks ("Truc:"), and fun facts ("Curiositat:", "Sabies que...?")
- **Maintain brevity**: Keep additions concise - each trick/anecdote should be 1-3 lines maximum to avoid bloating the document
- **Add engagement elements**: Include brief practical applications, memory tricks ("Truc:"), and fun facts ("Curiositat:", "Sabies que...?")
- **Maintain brevity**: Keep additions concise - each trick/anecdote should be 1-3 lines maximum to avoid bloating the document
