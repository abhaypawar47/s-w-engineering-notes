
# Software Engineering Study Notes

---

## Lesson 1: Introduction

* **Program:** A set of instructions or steps to perform a specific task.
* **Software (S/W):** A program along with its associated documentation.
    * `S/W = Program + Documentation`
* **Software Component:** A program, its documentation, and operating procedures.
* **Software Crisis:** Issues characterized by:
    * Overrun development costs.
    * Exceeding development time.
    * Failure to achieve desired quality.
* **Software Engineering:** The systematic application of engineering principles and methods to the design, development, testing, and maintenance of software products.

---

### 🌾 Characteristics of Software

* Developed through a defined software process.
* No physical wear and tear (unlike hardware).
* Often custom-built with specific features.
* Intangible; cannot be touched.

### 🌾 Major Problems in Software Development

* Inadequate requirements gathering.
* Lack of communication between stakeholders.
* Poor project management.
* Lack of risk mitigation.
* Wrong technology selection.
* Insufficient time and money (resource constraints).
* Lack of skill set within the development team.
* Less failure rate over time (implies initial robustness or early issue resolution).

### 🌾 Software Quality Attributes

* **Correctness:** Performs as specified.
* **Usability:** Easy to learn and use.
* **Reliability:** Performs consistently without failure.
* **Efficiency:** Uses resources (CPU, memory) optimally.
* **Maintainability:** Easy to modify and fix.
* **Portability:** Can be easily transferred to different environments.
* **Scalability:** Can handle increased load or data volume.
* **Security:** Protects against unauthorized access and attacks.

### 🌾 Software Process

A set of related activities leading to the production of software.
1.  **Feasibility Study:** Determine if the project is viable.
2.  **Requirement Analysis and Specification (SRS):** Define what the software needs to do.
3.  **Designing (SDD):** Plan how the software will be built.
4.  **Coding:** Write the actual program code.
5.  **Testing:** Verify the software meets requirements and is defect-free.
6.  **Implementation:** Deploy and install the software.
7.  **Maintenance:** Support and evolve the software after deployment.

### 🌾 Software Development Life Cycle (SDLC)

A procedure followed during the development of a software product in a well-defined and managed way.

---

### 🐶 Software Development Models

#### 🐶 Waterfall Model

* **Inspiration:** Manufacturing and construction processes.
* **Nature:** Linear, sequential, and simplest. Each step relies on the completion of the previous one.
* **Flow:** One-way progression; difficult to go back to previous phases.
* **Usage:** Typically used for small to medium-sized projects with well-defined and crystal-clear requirements.
* **Also known as:** Classical model.

**Steps:**
1.  Feasibility Study
2.  Requirement Analysis
3.  Design
4.  Coding
5.  Testing
6.  Maintenance

#### 🐶 Prototype Model

* **Nature:** Iterative approach.
* **Feedback:** Refines the software through continuous customer feedback.
* **Process:** Repetitive cycles until customer satisfaction is achieved.
* **Types:**
    * **Evolutionary:** The prototype evolves into the final system.
    * **Throwaway:** The prototype is discarded after serving its purpose (understanding requirements).
* **Flexibility:** Accommodates new requirements effectively.

**Steps:**
1.  Requirement Gathering
2.  Quick Design (of prototype)
3.  Build Prototype
4.  Customer Evaluation (of prototype)
5.  Refine Requirements (repeatedly until satisfied)
6.  (Final) Design
7.  Implement
8.  Test
9.  Maintain

#### 🐶 Spiral Model

* **Key Feature:** Introduces **risk analysis** at each iteration.
* **Phases (Iterative):**
    1.  **Objective Determination:** Define objectives, alternatives, and constraints.
    2.  **Identify and Resolve Risk:** Analyze risks and develop strategies to mitigate them.
    3.  **Development and Test:** Develop and test the next increment of the product.
    4.  **Plan Next Iteration:** Evaluate results and plan the next spiral (repeated until satisfaction).
* **Benefits:**
    * Provides early and frequent customer feedback.
    * Helps resolve all possible risks proactively.
    * Allows incremental release and testing.
* **Drawbacks:**
    * Not suitable for small projects due to its complexity.
    * Risk analysis requires significant expertise.

#### 🐶 Incremental Model

* **Nature:** Development of an initial implementation, which is then exposed to user feedback and evolves through several versions.
* **Benefits:**
    * Delivers working software at an early phase.
    * Easier to test and debug due to smaller iterations.
    * Supports agile development principles.
    * Facilitates continuous improvement.
* **Process:** Begins with a basic version (minimum functionality) and incorporates user feedback for subsequent improvements.

#### 🐱 V-Model (Verification & Validation in Parallel)

* **Key Principle:** Testing activities are planned and conducted in parallel with development activities.
* **Structure:** Rigid, V-shaped structure, where each development phase on the left side of the 'V' corresponds to a testing phase on the right side.

**Phases:**
* **Left Side (Development/Verification):**
    1.  Requirement Analysis (corresponds to Acceptance Testing)
    2.  System Design (corresponds to System Testing)
    3.  Architecture Design (corresponds to Integration Testing)
    4.  Module Design (corresponds to Unit Testing)
* **Bottom (Coding):**
    5.  Coding
* **Right Side (Testing/Validation):**
    6.  Unit Testing
    7.  Integration Testing
    8.  System Testing
    9.  Acceptance Testing

* **Benefits:**
    * Testing starts from the beginning, leading to early bug detection.
    * Strong discipline and documentation focus.
    * Suitable for small to medium-sized projects where requirements are stable.
* **Drawbacks:**
    * No overlap in phases, leading to a rigid structure.
    * Not flexible for changing requirements in later stages.

#### 🐰 Agile Model (Fast Delivery + Continuous Feedback)

* **Philosophy:** Emphasizes iterative development, frequent delivery of working software, and strong collaboration with customers.
* **Iterations:** Short cycles (typically 1-4 weeks) called "sprints" or "iterations."

**Phases (Iterative):**
1.  **Gather Minimal Requirements:** Collect requirements as user stories.
2.  **Plan Iteration (Sprint Planning):** Plan what to deliver in the current sprint.
3.  **Design, Develop, Test:** Complete development and testing within the sprint.
4.  **Deliver Working Product (Increment):** Release a functional piece of software.
5.  **Review & Get Feedback:** Present the increment to stakeholders and gather feedback.
6.  **Improve in Next Sprint:** Incorporate feedback and continue development in the next iteration.

* **Benefits:**
    * Customer involved in every step, ensuring alignment.
    * Highly flexible for accommodating changes.
    * Short iterations for quick feedback loops.
    * Better team collaboration.
    * Early delivery of working software.
* **Drawbacks:**
    * Requires active and consistent client participation.
    * Not ideal for highly critical systems (e.g., banking, aviation) where extensive upfront planning and rigid documentation are often mandated.

---

### 🌾 Verification vs. Validation

#### 🌾 Verification (Are we building the product right?)

* **Purpose:** Checks whether the software meets the specifications and internal standards.
* **Timing:** Happens *during* development (before actual execution).
* **Focus:** Documents, design, code, and plans.
* **Process:** It is a **static** process (does not involve running the code).
* **Examples:**
    * Reviews
    * Walkthroughs
    * Inspections
    * Checking SRS or Design Documents

#### 🧪 Validation (Are we building the right product?)

* **Purpose:** Checks whether the software meets the user's actual needs and expectations.
* **Timing:** Happens *after* development (post-coding).
* **Focus:** The actual product and user requirements.
* **Process:** It is a **dynamic** process (involves execution of code).
* **Examples:**
    * Functional Testing
    * System Testing
    * User Acceptance Testing (UAT)

---

## Lesson 2: Software Requirement Specification (SRS)

---

### 🌾 Requirement Analysis

* **Objective:** To determine "what is to be built."
* **Challenges:**
    * Requirements can be difficult to uncover fully.
    * Requirements often change throughout the project.
    * Tight project schedules.
    * Communication barriers between stakeholders and developers.

**Phases:**
1.  **Requirement Elicitation:** Gathering requirements from stakeholders.
2.  **Requirement Analysis:** Understanding and refining the gathered requirements.
3.  **Requirement Documentation (SRS):** Documenting the agreed-upon requirements.
4.  **Requirement Review:** Validating the documented requirements with stakeholders.

#### 🐶 Delphi Technique

* A structured communication technique that relies on a panel of experts to iteratively exchange written opinions (e.g., on pieces of paper or via surveys) to arrive at a consensus or revised requirements, often used to avoid direct confrontation and groupthink.

---

### 🐶 Software Quality Assurance (SQA)

* **Definition:** A systematic process to ensure that software products meet defined quality standards and requirements.
* **Objectives:**
    * Prevent defects.
    * Improve overall software quality.
    * Ensure customer satisfaction.
* **Techniques:** Code reviews, audits, testing.
* **Standards:** ISO 9000, IEEE 730, CMMI (Capability Maturity Model Integration).
* **Principles:** Continuous improvement, use of metrics, training, and documentation.

### 🐶 Validation (Black Box Testing)

* **Purpose:** To ensure the software product meets end-user requirements.
* **Question:** "Are we building the **right** product?"
* **Perspective:** Treats the system as a black box; focuses on inputs and outputs without concern for internal structure.

### 🐶 Verification (White Box Testing)

* **Purpose:** To ensure the software product is designed and developed according to standards and specifications.
* **Question:** "Are we building the product **right**?"
* **Perspective:** Concerned with the internal process and structure of the software.

### 🐶 CMM (Capability Maturity Model)

* **Purpose:** A framework for improving software processes to generate quality software. It describes an evolutionary path from an ad-hoc, chaotic process to a mature, disciplined process.
* **Maturity Levels:**
    1.  **Initial:** Processes are unpredictable, poorly controlled, and reactive.
    2.  **Managed/Repeatable:** Basic project management processes established; success depends on individual efforts.
    3.  **Defined:** Processes are documented, standardized, and integrated across the organization.
    4.  **Quantitatively Managed:** Processes are measured and controlled statistically.
    5.  **Optimizing:** Continuous process improvement driven by quantitative feedback and innovative ideas.

---

## Lesson 3: Software Designing

---

### 🐶 Design Phase

* **Input:** Software Requirement Specification (SRS).
* **Output:** Software Design Document (SDD).
* **Content:** The SDD contains all the architectural and detailed design points derived from the SRS.

---

### 🐶 The COCOMO Model (Constructive Cost Model)

* **Developer:** Barry Boehm.
* **Purpose:** A software cost estimation model that helps estimate:
    * Effort (in person-months).
    * Development time (in months).
    * Cost of a software project.

**Formulas:**
1.  **Effort (E) in person-months:**
    $E = a \times (\text{KLOC})^b$
2.  **Development Time (D) in months:**
    $D = c \times (E)^d$
3.  **People Required (P):**
    $P = E / D$

**Data/Variables:**
* **E:** Effort required (in person-months).
* **KLOC:** Thousands of Lines of Code.
* **a, b:** Constants based on the project type (e.g., organic, semi-detached, embedded).
* **D:** Development time (in months).
* **c, d:** Constants based on the project type.
* **P:** Average number of persons required.

---

## Unit 4: Software Testing

---

* **Reason for Bugs:** Human error during development often leads to bugs or faults in software.
    * **Error:** A human action that produces an incorrect result (detected during development).
    * **Bug/Fault/Defect:** A problem in the software that causes it to behave unexpectedly (detected during testing).

* **Unit Testing:** Testing individual software components or modules in isolation to ensure they function correctly.
* **Integration Testing:** Modules are combined and tested as a group to identify issues in their interactions.
* **System Testing:** The complete and integrated software system is tested as a whole against the specified SRS to verify all functional and non-functional requirements.
* **User Acceptance Testing (UAT):** The final testing phase, conducted by end-users or clients, to ensure the software works correctly in a real-world scenario and meets their business needs before deployment.
* **Regression Testing:** Ensures that previously developed and tested software continues to work well after making changes, updates, or bug fixes. It prevents new changes from introducing new defects or reactivating old ones.

* **Black Box Testing Approach (Validation):**
    * Checks the system as a whole based on requirements.
    * Focuses on inputs and outputs without knowledge of internal code structure.
    * Techniques: Boundary Value Analysis, Equivalence Partitioning.

* **White Box Testing Approach (Verification):**
    * Concerned with the internal process and structure of the code.
    * Tests internal logic, code paths, and loops.

* **Alpha Testing:** Testing conducted by internal development teams or a select group of testers at the developer's site, often simulating real user environments.
* **Beta Testing:** Testing conducted by real users in a real-world environment outside the developer's site. It helps discover defects that might not have been found by the in-house testing.

* **Boundary Value Analysis:** A black-box test design technique that tests values at the boundaries of valid and invalid input ranges.
* **Equivalence Partitioning:** A black-box test design technique that divides input data into partitions (classes) where all values in a partition are expected to behave similarly.

---

## Chapter 5: Software Maintenance

---

* **Corrective Maintenance:** Fixing defects or bugs discovered after the software has been deployed.
* **Adaptive Maintenance:** Modifying the software to adapt to changes in its environment (e.g., new operating system, hardware, or third-party software).
* **Perfective Maintenance:** Enhancing the software by adding new features, improving performance, or improving maintainability based on user feedback or evolving requirements.
* **Preventive Maintenance:** Modifying the software to prevent potential future problems, often by improving code structure, documentation, or maintainability.
```
