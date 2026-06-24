# Test 01 Review

Topic:
Motion in a Plane

Prompt Version:
Lesson Plan Generator v1.0

Overall Verdict:
Partly Usable

Strengths:
- Generated a complete lesson plan.
- Included activities and assessment.
- Output was classroom relevant.

Weaknesses:
1. Did not follow the 5E instructional model.
2. Did not break the chapter into teachable chunks.
3. Did not generate Bloom's Taxonomy-based objectives.
4. General and specific objectives were not clearly defined.

Improvement Requirements:
- Add 5E lesson structure.
- Add chapter chunking before lesson planning.
- Generate Bloom's Taxonomy-based objectives.
- Use action verbs from the revised Bloom's Taxonomy.

Additional Observation:

The lesson planner should not generate a lesson plan for the entire chapter at once.

Instead:

1. Break the chapter into teachable topics.
2. Generate topic-specific metadata for each topic:
   - Topic Name
   - General Objective
   - Specific Objectives
   - Prior Knowledge
3. Generate a detailed 30-minute 5E lesson plan only for the selected topic.
4. Generate one topic lesson at a time to avoid clutter and improve usability.

Architecture Decision:

The system will be split into two prompts.

Prompt 1:
Chapter Analyzer

Output:
- Estimated teaching periods
- Topic names
- Duration per topic
- Key concepts
- Prior knowledge

Prompt 2:
Topic Lesson Generator

Input:
- Selected topic

Output:
- General objective
- Specific objectives (Bloom's Taxonomy)
- Prior knowledge
- 5E lesson structure (30 minutes total)
- Homework assignment

Final Chapter Analyzer Output Format

Chapter Overview
- Chapter Name
- Estimated Total Periods
- Total Topics

For Each Topic
- Topic ID
- Topic Name
- Duration
- Key Concepts
- Prior Knowledge