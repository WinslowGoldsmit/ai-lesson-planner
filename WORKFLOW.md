# AI Lesson Planner Workflow v1.2

## Purpose

Generate classroom-ready teaching resources using a structured four-stage AI workflow. The system analyzes a chapter, generates a lesson plan, simplifies difficult concepts for students, and creates assessments.

---

## Workflow

```text
Chapter Analyzer
        ↓
Topic Lesson Generator
        ↓
Student Explanation Simplifier
        ↓
Quiz Generator
```

---

## Stage 1: Chapter Analysis

**Prompt**

`chapter-analyzer-v1.md`

**Input**

* Subject
* Class
* Chapter

**Output**

* Estimated Total Periods
* Total Topics
* Topic IDs
* Topic Names
* Key Concepts
* Prior Knowledge

**Example**

Motion in a Plane

* T1 – Scalars and Vectors
* T2 – Vector Addition
* T3 – Resolution of Vectors
* T4 – Projectile Motion
* T5 – Uniform Circular Motion

---

## Stage 2: Topic Lesson Generation

**Prompt**

`topic-lesson-generator-v1.md`

**Input**

* Subject
* Class
* Topic ID
* Topic Name
* Chapter Analyzer Output

**Output**

* General Objective
* Bloom's Taxonomy Objectives
* Prior Knowledge
* 5E Lesson Plan
* Homework Assignment

**Example**

**Input**

T1 – Scalars and Vectors

**Output**

One complete classroom-ready lesson plan.

---

## Stage 3: Student Explanation Simplifier

**Prompt**

`student-explanation-simplifier-v1.md`

**Input**

* Subject
* Class
* Chapter
* Topic
* Concept to Explain

**Output**

* One-Sentence Explanation
* Simple Explanation
* Real-Life Analogy
* Step-by-Step Explanation
* Common Misconception
* Memory Trick
* Quick Recap
* Practice Question
* Understanding Check

**Example**

**Input**

Concept: Difference between Scalars and Vectors

**Output**

A student-friendly explanation with examples, misconceptions, memory aids, and understanding checks.

---

## Stage 4: Quiz Generation

**Prompt**

`quiz-generator-v1.md`

**Input**

* Topic Lesson Generator Output

**Output**

* 5 Multiple Choice Questions (MCQs)
* 3 Short Answer Questions
* 2 Long Answer Questions
* Answer Key
* Common Student Mistakes

**Example**

**Input**

Lesson Plan for *Scalars and Vectors*

**Output**

One classroom-ready quiz with answer key.

---

## Development Process

Each prompt follows the same iterative development cycle:

1. Create Prompt
2. Test the Prompt
3. Save Test Input and Output
4. Review the Output
5. Identify Improvements
6. Update the Prompt Version
7. Retest

---

## Current Workflow Versions

* Chapter Analyzer v1.0
* Topic Lesson Generator v1.0
* Student Explanation Simplifier v1.0
* Quiz Generator v1.0

---

## Version History

### v1.2 (2026-06-26)

* Added the **Student Explanation Simplifier** stage.
* Expanded the workflow from three stages to four stages.
* Improved the overall teaching workflow by including concept simplification before assessment generation.

### v1.1

* Added the **Quiz Generator** stage.
* Updated the workflow from lesson planning to lesson planning plus assessment generation.

### v1.0

* Initial workflow with **Chapter Analyzer** and **Topic Lesson Generator**.
