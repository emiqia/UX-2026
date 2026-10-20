# Redo

*Feedback on assessments that students actually use*

Documentation repository for the UX project of **group 5**. The project aims to turn the feedback on an assessment into a concrete correction in the next submission, and to let students check their progress by rubric criterion.

## Team

| Member |
| --- |
| Cristian Sandova |
| Emilia Toro |
| Bastian Wenckhans |

## Selected project

Feedback on assignments and rubrics arrives late and scattered across PDF comments, spreadsheets and emails. This makes it hard for students to understand what failed and to apply the comments before their next submission.

The challenge is to **close the feedback loop**: identify the criterion that failed, understand which concrete action corrects it, and check whether there was an improvement over the previous submission. The functional surface is small, and the design focus is on the clarity of the information and on evidence that the feedback was used.

### Main user story

> As a student who got a low grade on the first submission, I need to see exactly which criterion failed and what I should do differently next time, so that I do not repeat the same mistake without noticing.

### Design goal

Design an experience that connects **evaluated criterion → detected difficulty → improvement action → evidence of application → result of the next submission**.

The value proposition is to help students turn the comments of an assessment into understandable and verifiable actions for their next piece of work.

The [project brief](docs/project-brief.md) develops the problem, the proposed scope and the questions to validate with users.

## UX Elements Architecture (Jesse James Garrett)

To ensure academic and methodological rigor, each UX Research and design technique in the project is anchored to one of the five planes of Jesse James Garrett's *The Elements of User Experience*:

| UX Element Plane | Research & Design Techniques | Associated Project Deliverables | Grounding & Objectives |
| :--- | :--- | :--- | :--- |
| **1. Strategy** *(Estrategia)* | Semi-structured interviews ($N=3$), qualitative thematic analysis, Persona modeling, Value Proposition Canvas. | [Research Report](docs/user-research-interviews.pdf), [UX Personas](docs/user-personas.pdf), [Value Canvas](docs/value-proposition-canvas-full.pdf), [Brief](docs/project-brief.md) | Identifies breakdowns in feedback comprehension and establishes core value proposition: closing the loop with evidence. |
| **2. Scope** *(Alcance)* | Competitive & analogous benchmarking, ERIC matrix, requirements prioritization, boundary definition. | [Benchmarking Report](docs/benchmarking-report.pdf), [Scope & UX Elements](docs/scope-and-ux-elements.pdf) | Constrains solution to 1 core flow and 2 secondary flows; establishes explicit justification for out-of-scope features. |
| **3. Structure** *(Estructura)* | Customer Journey Mapping, navigation flow diagrams, information architecture. | [Customer Journey Map](docs/Customer-Journey-Map.pdf), Navigation Flow Diagram, CJM-Interface Mapping | Structures transitions from receiving feedback to submitting evidence; binds journey stages to interface IDs (UI-01 to UI-07). |
| **4. Skeleton** *(Esqueleto)* | Paper Low-Fi sketching, interface evolution tracking, wireframing. | Low-Fi Paper Sketches, UI Evolution Log | Determines screen layout, hierarchy, and physical interaction controls (designed by Cristián). |
| **5. Surface** *(Superficie)* | High-Definition UI prototyping, design system, accessibility audit. | Figma HD Prototype, Classroom Printouts | Final sensory presentation in Spanish with accessible color tokens and consistent typography. |

*Detailed Document:* [View the Scope Delimitation, UX Elements & CJM Mapping PDF](docs/scope-and-ux-elements.pdf).

## Completed activities

### 1. UX personas

Three distinct profiles were created, with different fields, institutions and roles. Two represent the students who receive and apply the feedback. The third represents the instructor who gives it and reviews the evidence of correction.

The profiles are **empirical UX Personas grounded in qualitative user research** conducted through semi-structured in-depth interviews with undergraduate engineering students, design students, and university instructors. The full qualitative protocol, interview transcripts, and thematic syntheses are documented in the [User Research & Fieldwork Interviews PDF](docs/user-research-interviews.pdf).

| Persona | Age | Field and role | Institution | Relation to the solution |
| --- | --- | --- | --- | --- |
| Valentina Rojas | 20 | Computer engineering student, primary user. | Universidad de La Frontera | Identifies the failed criterion, follows a corrective action and compares her result in the next submission. |
| Samon Baker | 21 | Graphic design student and intern, primary user. | INACAP | Gathers comments by project, prioritizes revisions and links each action to evidence of the change in his design. |
| Martina Soto | 29 | University instructor in education, secondary user. | Universidad Católica de Temuco | Relates comments to criteria and actions, reviews the evidence of correction and compares results across submissions. |

The three profiles are set in Temuco, Chile. Their differences point to concrete interaction needs: clarity for Valentina, prioritization for Samon and follow-up on application for Martina.

#### Valentina Rojas

![Valentina Rojas, computer engineering student at Universidad de La Frontera: understanding and applying feedback](ux-personas/1.png)

#### Samon Baker

![Samon Baker, graphic design student at INACAP and intern: prioritizing revisions and evidence of changes](ux-personas/2.png)

#### Martina Soto

![Martina Soto, instructor at Universidad Católica de Temuco: corrective actions and progress verification](ux-personas/3.png)

- [View the PDF with the three UX personas](docs/user-personas.pdf).
- [View the User Research & Fieldwork Interviews PDF](docs/user-research-interviews.pdf).

The profiles are written in English and share a structure of personal information, biography, goals, frustrations, personality, interests and needs. The layout places the photo on the left and the information in two columns on the right. Only the name appears over the photos, while the field, institution and role appear in the personal information.

### 2. Value Proposition Canvas

The Value Proposition Canvas aligns user needs with the system's core capabilities. While the initial exploratory canvas focused solely on a generic student segment, the calibrated canvas explicitly accounts for **all three validated UX Personas (Valentina, Samon, and Martina)**, closing the loop from both the student remediation and the instructor verification perspectives.

* **Calibrated Canvas (3 Personas):** [View the Calibrated Value Proposition Canvas & Strategy Brief PDF](docs/value-proposition-canvas-full.pdf).
* **Initial Exploratory Board:** [View the original Student Canvas PDF](docs/value-proposition-canvas.pdf).

![Value Proposition Canvas of the assessment feedback project](images/value_proposition.png)

| Persona / Role | Addressed Customer Jobs | Pains Relieved | Gains Created | Core UI Capability |
| :--- | :--- | :--- | :--- | :--- |
| **Valentina Rojas**<br>*(Primary Learner)* | Identify exact rubric failure and execute verifiable corrections for subsequent submission. | Eliminates abstract comments ("elaborate more") and fear of uncredited fixes. | Transparency in criteria and certainty that evidence is linked to critique. | **Prescriptive Action Cards + Evidence-Binding Module** |
| **Samon Baker**<br>*(Primary Prioritizer)* | Triage revision tasks against tight deadlines and track design version adjustments. | Resolves unranked feedback overload and lost context between prototype versions. | Prioritized task list ranked by rubric weight; clear version labeling. | **Urgency / Rubric Weight Sorting + Version Tagging** |
| **Martina Soto**<br>*(Secondary Evaluator)* | Formulate actionable feedback and verify student compliance without manual re-reading. | Eliminates 20+ hours of manual side-by-side document comparison and empty checkbox claims. | Rapid, auditable verification of corrections in a single comparative view. | **Instructor Verification Queue + 1-Click Status Approval** |

> **Scope Note:** Auxiliary functions such as general campus timetables, exam calendars, and institutional gradebooks shown in early exploratory mockups are strictly excluded from the design scope to preserve functional focus and comply with course requirements.

### 3. Benchmarking

A comprehensive exploratory and competitive UX benchmark adapted from the *Fructus Iter* methodology, designed to evaluate how educational and collaborative platforms manage the feedback-to-remediation loop.

The benchmark integrates four methodological components demanded by the course rubric:
1. **Initial Exploration Protocol (*Pauta de Exploración*):** Standardized protocol evaluating 4 user tasks under Valentina's shared scenario (receiving 1/4 on a rubric criterion, formulating actions, binding evidence, and instructor verification).
2. **Annotated Interface Teardowns (*Capturas Anotadas*):** Detailed teardowns with positive `[+]` and negative `[-]` callouts analyzing direct competitors (Moodle, Canvas LMS, Google Classroom) and collaborative tools (Trello, GitHub PRs, Figma).
3. **Synthetic Comparison & ERIC Matrix:** Qualitative comparison of feature support alongside an Opportunity Matrix (*Eliminate, Reduce, Raise, Create*).
4. **Ideation & Concept Map (*Mapa de Ideas*):** Architectural diagram connecting competitor patterns to LoopFeedback's 4 core modules (*Interactive Rubric Breakdown*, *Prescriptive Action Cards*, *Evidence-Binding Module*, and *Instructor Verification Queue*).

* **Full Report:** [View the Comprehensive 9-page UX Benchmarking Report PDF](docs/benchmarking-report.pdf).
* **Synthesis Board:** [View the original Benchmarking Board PDF](docs/Benchmarking.pdf).

![Benchmarking of feedback tools for students](images/benchmarking.png)

| Tool | Category | Key Finding & Contribution to Design |
| --- | --- | --- |
| Moodle (Campus Virtual UFRO) | Direct Competitor | Clear rubric level highlighting, but comments are trapped inside small cells and resubmissions overwrite past history. |
| Canvas LMS | Direct Competitor | Criterion-level remarks via SpeedGrader, but lacks student-driven evidence binding and cross-submission comparison. |
| Google Classroom | Direct Competitor | Clean expandable score chips, but private feedback is separated from specific rubric criteria. |
| Trello | Analogous Reference | Strong mental model for checkable action cards and file attachments; adopted for our prescriptive action cards. |
| GitHub (Pull Requests) | Analogous Reference | Line-by-line granular critique and re-requesting review; inspires our bidirectional evidence binding. |
| Figma (Comments) | Analogous Reference | In-situ pinned feedback and version comparison history. |
| Intranet UFRO | Baseline Reference | Static grade display with no rubric or formative remediation mechanism. |

### 4. Customer Journey Map

A single general journey, not one per persona, in six stages: receive the result, find the feedback, understand it, revise, submit and check progress. It includes scenario, expectations, actions, touchpoints, instructor actions, thoughts, emotional curve, pain points and opportunities. It starts from Valentina Rojas and Samon Baker as primary users and Martina Soto as the secondary user.

![Customer Journey Map of the project](images/customer-journey-map.png)

* [View the Customer Journey Map PDF](docs/Customer-Journey-Map.pdf).
* [View the CJM & Interfaces Architecture Document](docs/scope-and-ux-elements.pdf).

#### Customer Journey Map to Interface Mapping

To ensure direct traceability between user fieldwork and interface screens, each CJM stage is formally bound to a specific interface designed by the team:

| CJM Stage | User Action (Valentina / Samon) | Emotional State | Interface ID | Screen Name & Core Interaction |
| :--- | :--- | :--- | :---: | :--- |
| **01 Receive** | Opens assessment result on the platform. | Concerned / Anxious | **UI-01** | **Assessment Overview Dashboard:** Summary card displaying total grade, delivery date, and color-coded status badges for all criteria. |
| **02 Find** | Locates rubric and identifies penalized criterion. | Reassured / Focused | **UI-02** | **Rubric Breakdown & Criterion Inspector:** Expandable rubric grid highlighting achieved level, points lost, and teacher comments. |
| **03 Understand** | Reads explanation and identifies concrete fix. | Confident | **UI-03** | **Prescriptive Action Card Drawer:** Dedicated card displaying instructor-approved tasks, prescriptive examples, and success conditions. |
| **04 Revise** | Updates deliverable and attaches revision evidence. | In control | **UI-04** | **Evidence-Binding Modal:** Upload/input modal where student anchors text snippets, screenshots, or URLs directly to the action card. |
| **05 Submit** | Sends correction with linked proof for teacher review. | Hopeful | **UI-05** | **Submission Confirmation & Status Tracker:** Moves action status from `Pending` to `Evidence Submitted`, awaiting instructor review. |
| **06 Compare** | Reviews subsequent submission to verify improvement. | Encouraged | **UI-06** | **Longitudinal Criterion Comparison View:** Side-by-side historical comparison of the same criterion between Deliverable 1 and 2. |
| *Evaluator Flow* | Reviews student evidence and validates correction. | Relieved / Efficient | **UI-07** | **Instructor Verification Queue:** Split inspection view allowing 1-click approval or re-prompting without manual document search. |

## Delimitation of Scope (Delimitación del Alcance)

In strict accordance with the project guidelines, functional exhaustiveness is avoided. The proposal is formally bounded to **one core flow** and **two secondary flows**, with an explicit written justification of capabilities left out of scope to avoid penalization.

### 1. Core Flow (Flujo Principal): Feedback-to-Remediation Loop
* **Actor:** Student (Valentina Rojas / Samon Baker).
* **Sequential Interaction Steps:**
  1. **Identify Weakness (`UI-01` & `UI-02`):** Student inspects returned deliverable and isolates a penalized criterion ($1/4$ points) along with the instructor's observation.
  2. **Access Prescriptive Guidance (`UI-03`):** Student opens the associated Action Card to review the concrete, instructor-approved remediation guideline (*"What to do"*, *"Example"*, *"Success condition"*).
  3. **Anchor & Submit Evidence (`UI-04` & `UI-05`):** Student uploads and binds proof of correction (revised paragraph, code link, or annotated design) and submits it, updating status from `Pending Revision` to `Evidence Submitted`.

### 2. Secondary Flow 1: Instructor Verification & Status Approval
* **Actor:** Course Instructor / Evaluator (Martina Soto).
* **Sequential Interaction Steps:**
  1. **Review Verification Queue (`UI-07`):** Instructor opens pending student remediation submissions.
  2. **Side-by-Side Inspection:** System displays the original rubric critique alongside the student's linked evidence.
  3. **1-Click Status Update:** Instructor approves the correction or requests further clarification without reading entire 40-page reports.

### 3. Secondary Flow 2: Longitudinal Criterion Comparison
* **Actor:** Student (Valentina/Samon) and Instructor (Martina).
* **Sequential Interaction Steps:**
  1. **Select Deliverables (`UI-06`):** User chooses comparable Milestone 1 and Milestone 2 submissions.
  2. **Inspect Evolution:** System displays side-by-side performance on the same rubric criterion to verify measurable academic growth.

### 4. Explicit Justification of Out-of-Scope Features (Qué queda fuera y por qué)

| Out-of-Scope Feature | Scope Decision | Pedagogical & UX Justification |
| :--- | :---: | :--- |
| **General Academic Timetables & Class Schedules** | Excluded | The initiative focuses exclusively on the formative evaluation loop. Campus scheduling creates interface noise and deviates from the core usability problem. |
| **Comprehensive Gradebook & Final GPA Calculator** | Excluded | Institutional platforms (UFRO Intranet) already calculate weighted averages. Duplicating gradebooks shifts focus away from criterion-level understanding. |
| **Unstructured Chat / Direct Messaging Channel** | Excluded | Fieldwork revealed open messaging threads cause evaluator fatigue and scatter feedback. Communication must remain strictly anchored to Action Cards and Evidence Attachments. |
| **Automated AI Grading / Generative Auto-Scoring** | Excluded | Course regulations mandate that Milestone 1 proves human UX design and research. AI grading is prohibited in Hito 1 (and will be explored under Human-in-the-Loop guidelines in Hito 2). |
| **Multi-Institution Account Synchronization** | Excluded | The prototype assumes a single course environment ($1$ course, $2$ related deliverables) to validate interaction mechanics before tackling institutional API interoperability. |

### Illustrative example

This example explains the proposal. It is not a finding and does not come from a test.

| Step | Example |
| --- | --- |
| Criterion | Justification of design decisions. |
| Difficulty | The first submission presents a decision without linking it to user evidence. |
| Concrete action | Add the evidence that supports the decision and explain how it relates to the user's problem. |
| Evidence of application | Point to the section of the second submission where that justification was added. |
| Check | Review the level reached on the same criterion in the second assessment. |

## Traceability of design decisions

The following table links needs described in the materials to design proposals and ways to validate them. It does not represent research results.

| Need or difficulty | Proposed response | Evidence to collect |
| --- | --- | --- |
| Not knowing which criterion failed | Present criterion, result and comment together. | The student correctly identifies the criterion and explains the difficulty. |
| Not understanding what to correct | Show a specific action and a relevant example. | The student explains in their own words what they will change. |
| Reviewing separate files and emails | Bring the feedback of the submission into one view. | They find the relevant comment without going through several sources. |
| Repeating mistakes | Link improvement actions to evidence in the next submission. | A concrete change linked to the earlier comment is identified. |
| Not recognizing progress | Compare the result of the same criterion across submissions. | They recognize whether performance improved, stayed the same or got worse. |
| Little time to review design projects | Prioritize actions and gather comments by version. | The student finds a relevant action and points to the change made. |
| Instructor difficulty verifying application | Link evidence in the next submission to each earlier comment. | The instructor identifies the correction and evaluates it against the same criterion. |

## Proposed validation

The proposal is to test the prototype with engineering and design students who have received feedback and must make a related later submission. Instructors would help review the clarity of the actions and the effort of verifying corrections. An initial test can ask participants to locate a weak criterion, explain the correction, record evidence and read the comparison across submissions.

| Dimension | Proposed indicator |
| --- | --- |
| Understanding of the problem | Share of participants who correctly identify the criterion to improve. |
| Clarity of the action | Share who describe a concrete correction consistent with the comment and the rubric. |
| Ease of use | Time, errors and help needed to find and understand the feedback. |
| Application | Share of actions with relevant evidence in the next submission. |
| Progress | Change in level or score on the same criterion across comparable assessments. |

**Opening a comment or marking a task as done does not show by itself that the feedback was applied.** Applying it requires evidence in the work. A better grade does not show by itself that the tool caused the improvement either. Numeric targets and test sizes will be defined when the research is prepared.

## Status and next steps

| Activity | Status |
| --- | --- |
| Initial definition of the problem and the user story | Available. |
| UX Elements Architecture | Completed. 5 planes of Jesse James Garrett documented with techniques and deliverables (docs/scope-and-ux-elements.pdf). |
| UX personas | Three validated empirical profiles grounded in qualitative fieldwork interviews. |
| Value Proposition Canvas | Completed. Calibrated for all three personas (Valentina, Samon, Martina) and focused on feedback loop without auxiliary clutter (docs/value-proposition-canvas-full.pdf). |
| Benchmarking | Completed. Full 9-page benchmark including exploration protocol, annotated teardowns, comparison matrix, ERIC matrix, and concept map (docs/benchmarking-report.pdf). |
| Customer Journey Map & UI Mapping | Completed. 6 stages formally mapped to interface IDs UI-01 through UI-07 (docs/scope-and-ux-elements.pdf). |
| Delimitation of Scope | Completed. 1 core flow, 2 secondary flows, and justified out-of-scope rationale table (docs/scope-and-ux-elements.pdf). |
| Research with students and instructors | Completed. Semi-structured interviews conducted with students and instructors; evidence attached in docs. |
| Flow and prototype design | In progress by Designer (Cristián). Navigation flowchart and paper low-fi sketches underway. |
| Usability testing and application tracking | Scheduled for Milestone 2. |
| High-fidelity interface proposal | In progress by Designer (Cristián). Figma HD prototype and printouts underway. |

The UX analysis and research deliverables for Milestone 1 are complete. The next step is for the designer (Cristián) to finalize the paper low-fi prototypes, navigation flowchart, and Figma HD screens based on the UI specifications established above.

## Repository contents

```text
.
├── README.md
├── docs/
│   ├── project-brief.md
│   ├── user-research-interviews.pdf
│   ├── user-personas.pdf
│   ├── value-proposition-canvas-full.pdf
│   ├── value-proposition-canvas.pdf
│   ├── benchmarking-report.pdf
│   ├── benchmarking.pdf
│   ├── Customer-Journey-Map.pdf
│   ├── scope-and-ux-elements.pdf
│   └── scope-and-ux-elements.md
├── ux-personas/
│   ├── 1.png
│   ├── 2.png
│   └── 3.png
└── images/
    ├── value_proposition.png
    ├── benchmarking.png
    └── customer-journey-map.png
```

The documentation is in English across all documents in `docs/` and the repository root. The next iteration of the canvas should consider the three current profiles.

This repository documents a UX proposal. The delivered files do not include a runnable application, so there are no installation or run instructions.
