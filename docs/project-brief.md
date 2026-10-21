# Project Brief: Redo

## Group 5

| Member | Role |
| --- | --- |
| Emilia Toro | Project Lead |
| Cristian Sandoval | Designer |
| Bastian Wenckhans | Analyst |

## Selected Challenge

**Assessment feedback that students actually use** (Initiative 03, HCI / UXD 2026-2).

Feedback on assessments reaches students as a grade plus comments scattered across PDF files, spreadsheets and emails. Rubrics are often published late, students cannot tell where they lost points, and they cannot place their result in the context of the course. When they disagree with a correction, there is no clear way to ask.

> As a student who received a low grade, I need to see exactly which criterion or question cost me points, and why, so that I can prepare better for the next assessment and ask my teacher about any correction I do not understand.

## Proposed Solution: Redo

Redo is a mobile app with a student side and a teacher side.

- **Student:** calendar of assessments; published rubric of upcoming assessments; result detail with points per criterion, or incorrect questions with the correct answer and a final teacher comment; course average, highest and lowest; progress over time with the biggest error; and a structured message to the teacher about a specific criterion or question. The student only views and asks; nothing has to be uploaded.
- **Teacher:** schedule assessments; publish a rubric (criteria and weights, or a file) or a test; review tests with a correct-answers sheet and a final comment; answer student queries, with the option to adjust the score once.

The prototype is set in a single institutional environment (UFRO). The 15 HD screens are in [Figma](https://www.figma.com/design/cwB8ZiCmUKTIgNYHercjWv) and listed in the [README](../README.md).

## Research Summary

Three semi-structured interviews (two students and one teacher, 30–40 minutes each, informed consent) were held on 14–16 October 2026 and analysed thematically. Details are in the [research report](user-research-interviews.pdf).

| Finding | What participants described | Design response |
| --- | --- | --- |
| F1. A number without a reason | The grade arrives as a single number; the criteria or questions that cost points are hard to find. | Points per criterion; incorrect questions with the correct answer (HD-06, HD-07). |
| F2. Rubrics arrive too late | Rubrics are published after the assessment or in a different place, so they are not used to prepare. | Rubric published before the assessment (HD-08, HD-13). |
| F3. No context | Students do not know how their result compares with the course or whether they are improving. | Course average, highest, lowest, chart and biggest error (HD-06, HD-10). |
| F4. Unstructured questions | Disagreements go through email or in person, without reference to the criterion, and students hesitate to ask. | Structured message anchored to a criterion or question (HD-09, HD-15). |
| F5. Teacher overload | The teacher repeats explanations, republishes rubrics and handles queries across several channels. | One place to schedule, publish, review and answer (HD-12 to HD-15). |
| F6. Calendar by hand | Students keep their own calendar of assessments and update it manually. | Calendar of assessments with state per day (HD-04, HD-05). |

## Audiences

**Primary:** students who receive graded feedback. Valentina Rojas (20, computer engineering, Universidad de La Frontera) and Samon Baker (21, graphic design student and intern, INACAP).

**Secondary:** Martina Soto (29, university instructor in education, Universidad Católica de Temuco), who publishes rubrics and tests and answers queries.

The three personas are set in Temuco. Their differences inform needs; the prototype uses a single institutional environment.

## Scope

The scope is everything built in the 15 screens:

- **Core flow:** the teacher publishes a rubric or test; the student prepares with it and later understands the result (HD-04 to HD-08, HD-12 to HD-14).
- **Secondary flow 1:** the student queries a correction and the teacher answers (HD-09, HD-15).
- **Secondary flow 2:** the student follows progress (HD-10).
- **Supporting:** welcome, sign in, profile choice and student profile (HD-01 to HD-03, HD-11).

**Out of scope:** evidence upload and action cards, integration with the intranet or Moodle, free chat, final-grade calculator, automated grading with AI, and multi-institution synchronization.

## Constraints and Open Questions

- How early must a rubric be published for students to use it to prepare?
- Should a score adjustment after a query be visible to the rest of the course?
- How many queries can a teacher answer without feeling overloaded?
- How should the app handle assessments without a rubric?
- Does comparison with the course average motivate or discourage students?

## Artifacts and Status

User research, personas, Value Proposition Canvas, benchmarking, Customer Journey Map, scope and UX elements, and the HD prototype are complete for Milestone 1. Paper low-fi digitization, the AI Usage Log and the presentation are being prepared by the team. Usability testing is planned for Milestone 2.

See the [README](../README.md) for the full list of deliverables.
