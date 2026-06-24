# AI Lesson Planner Workflow v1.0

## Purpose

Generate classroom-ready lesson plans using a two-stage workflow.

---

## Stage 1: Chapter Analysis

Prompt:

chapter-analyzer-v1.md

Input:

* Subject
* Class
* Chapter

Output:

* Estimated Total Periods
* Total Topics
* Topic IDs
* Topic Names
* Key Concepts
* Prior Knowledge

Example:

Motion in a Plane

T1 - Scalars and Vectors

T2 - Vector Addition

T3 - Resolution of Vectors

T4 - Projectile Motion

T5 - Uniform Circular Motion

---

## Stage 2: Topic Lesson Generation

Prompt:

topic-lesson-generator-v1.md

Input:

* Subject
* Class
* Topic ID
* Topic Name

Output:

* General Objective
* Bloom's Taxonomy Objectives
* Prior Knowledge
* 5E Lesson Plan
* Homework Assignment

Example:

Input:

T1 - Scalars and Vectors

Output:

One complete classroom-ready lesson plan.

---

## Development Process

1. Create Prompt
2. Run Test
3. Save Output
4. Review Output
5. Improve Prompt
6. Version Prompt
7. Retest

---

## Current Version

Chapter Analyzer v1.0

Topic Lesson Generator v1.0
