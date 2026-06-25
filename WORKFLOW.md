# AI Lesson Planner Workflow v1.3

## Purpose

The AI Lesson Planner is a modular workflow that generates classroom-ready teaching resources from a single chapter input. The system guides teachers from chapter analysis to lesson planning, student-friendly explanations, and assessment creation through a structured sequence of AI prompts.

---

# Workflow

```text
Teacher Input
(Subject + Class + Chapter)
            │
            ▼
Chapter Analyzer
            │
            ▼
Topic Lesson Generator
            │
            ▼
Student Explanation Simplifier
            │
            ▼
Quiz Generator
            │
            ▼
Complete Teaching Package
```

---

# Stage 1 – Chapter Analyzer

**Prompt**

`chapter-analyzer-v1.md`

### Input

* Subject
* Class
* Chapter

### Output

* Chapter Overview
* Estimated Teaching Periods
* Ordered Topics
* Topic IDs
* Key Concepts
* Prior Knowledge

### Purpose

Break a complete chapter into logical, teachable topics before lesson planning begins.

---

# Stage 2 – Topic Lesson Generator

**Prompt**

`topic-lesson-generator-v1.md`

### Input

* Subject
* Class
* Topic ID
* Topic Name
* Key Concepts
* Prior Knowledge

### Output

* General Objective
* Bloom's Taxonomy Objectives
* Prior Knowledge
* 5E Lesson Plan
* Homework Assignment

### Purpose

Generate a complete classroom-ready lesson plan for one selected topic.

---

# Stage 3 – Student Explanation Simplifier

**Prompt**

`student-explanation-simplifier-v1.md`

### Input

* Subject
* Class
* Chapter
* Topic
* Lesson Plan

### Output

* One-Sentence Explanation
* Simple Explanation
* Real-Life Analogy
* Step-by-Step Explanation
* Common Misconception
* Memory Trick
* Quick Recap
* Practice Question
* Understanding Check

### Purpose

Convert teacher-focused content into language that students can easily understand.

---

# Stage 4 – Quiz Generator

**Prompt**

`quiz-generator-v1.md`

### Input

* Lesson Plan

### Output

* Multiple Choice Questions (MCQs)
* Short Answer Questions
* Long Answer Questions
* Answer Key
* Common Student Mistakes

### Purpose

Generate an assessment aligned with the lesson objectives.

---

# Workflow Demonstration

The complete workflow has been tested using the following example:

**Subject:** Physics

**Class:** 11

**Chapter:** Motion in a Plane

**Topic:** Projectile Motion

The workflow successfully generated:

1. Chapter Analysis
2. Topic Lesson Plan
3. Student-Friendly Explanation
4. Topic-Based Quiz

The complete test is documented in:

* `tests/workflow-demo-projectile-motion-v1.md`
* `results/workflow-review-v1.md`

---

# Development Process

Each prompt follows an iterative improvement cycle:

1. Design the prompt.
2. Test using a real classroom example.
3. Save the generated output.
4. Review strengths and weaknesses.
5. Document improvements.
6. Update the prompt version.
7. Retest the prompt.
8. Integrate it into the complete workflow.

---

# Current Prompt Versions

* Chapter Analyzer v1.0
* Topic Lesson Generator v1.0
* Student Explanation Simplifier v1.0
* Quiz Generator v1.0

---

# Current Status

* Four prompts developed and tested.
* End-to-end workflow successfully demonstrated.
* Workflow review completed.
* Ready for Workflow v2 improvements focused on reducing manual input, improving data transfer between prompts, and preparing the workflow for future automation.

---

# Version History

## v1.3 (2026-06-26)

* Successfully tested the complete end-to-end AI Lesson Planner workflow.
* Added workflow demonstration using **Class 11 Physics – Motion in a Plane (Projectile Motion)**.
* Improved documentation to describe the purpose, inputs, outputs, and data flow of each stage.
* Documented the workflow review process and established priorities for Workflow v2.

## v1.2

* Added the Student Explanation Simplifier stage.
* Expanded the workflow from three stages to four stages.
* Improved the teaching workflow by simplifying concepts before assessment generation.

## v1.1

* Added the Quiz Generator stage.
* Expanded the workflow from lesson planning to lesson planning with assessment generation.

## v1.0

* Initial workflow containing the Chapter Analyzer and Topic Lesson Generator.
