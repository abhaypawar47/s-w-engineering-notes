
# Software Engineering Study Notes from video

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

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Software Engineering Study Notes from syllabus

## Unit I: Introduction to Software Engineering

### 📚 Nature of Software

* **Software:** More than just a program; it includes data structures, documentation, and configuration information.
* **Characteristics:**
    * **Developed, not manufactured:** Software doesn't "wear out" physically like hardware; it can deteriorate logically (becomes outdated, hard to maintain).
    * **Custom-built:** Often designed for specific needs, though reusable components exist.
    * **Intangible:** Cannot be touched or seen directly, making its development and quality assessment challenging.

### 🔄 Software Process

* A framework for the activities, actions, and tasks required to build high-quality software.
* **Purpose:** Provides a roadmap for developing software, ensuring systematic progress and quality control.

### 🛠️ Software Engineering Practices

* **Communication:** Effective exchange of information between stakeholders.
* **Planning:** Creating a roadmap for the project, including tasks, resources, and timelines.
* **Modeling:** Creating abstractions (diagrams, documents) to understand the problem and design the solution.
* **Construction:** Coding and testing the software.
* **Deployment:** Delivering the software to the user and providing support.

### 💡 Software Myths

Common misconceptions about software, often held by managers, customers, or even developers, that can lead to problems.
* **Management Myths:** E.g., "We have a book of standards, so quality is assured." (Standards aren't always followed or sufficient).
* **Customer Myths:** E.g., "General statements of objectives are sufficient to start writing programs; details can be added later." (Leads to incomplete requirements and rework).
* **Practitioner Myths:** E.g., "Once the program is working, our job is done." (Ignores maintenance and evolution).

### ⚙️ Generic Process Model

A general framework for software development, typically involving:
1.  **Communication:** Gathering requirements.
2.  **Planning:** Defining the project scope, resources, and schedule.
3.  **Modeling:** Designing the software architecture and components.
4.  **Construction:** Coding and testing.
5.  **Deployment:** Delivery and feedback.

### 📊 Analysis and Comparison of Process Models

Different approaches to organize and manage software development activities.

* **Waterfall Model:**
    * **Description:** Linear, sequential flow; each phase must be completed before the next begins.
    * **Characteristics:** Simple, easy to manage, good for small projects with stable, well-defined requirements.
    * **Drawbacks:** Inflexible, difficult to go back, risks detected late. (See Lesson 1 notes for more detail).

* **Incremental Model:**
    * **Description:** Builds the software in small, manageable increments, adding features with each cycle.
    * **Characteristics:** Delivers working software early, good for evolving requirements, reduces risk.
    * **Drawbacks:** Requires careful planning of increments, integration can be complex. (See Lesson 1 notes for more detail).

* **Evolutionary Models:**
    * **Description:** Develops software in an iterative manner, allowing the system to evolve over time based on feedback.
    * **Examples:** Prototyping Model, Spiral Model.
    * **Characteristics:** Handles changing requirements well, provides early user feedback.

    * **Prototyping Model:** (See Lesson 1 notes for more detail).
    * **Spiral Model:** (See Lesson 1 notes for more detail).

* **Concurrent Models:**
    * **Description:** Different activities (e.g., modeling, construction) can occur concurrently and are event-driven.
    * **Characteristics:** More flexible than sequential models, allows for parallel work.
    * **Example:** Concurrent Engineering Model.

* **Personal and Team Process Models (PSP & TSP):**
    * **PSP (Personal Software Process):** A structured framework for individual software engineers to improve their personal productivity and quality. Focuses on disciplined practices.
    * **TSP (Team Software Process):** A defined process for software engineering teams to develop self-directed, high-performance teams. Built upon PSP principles.

### 🧹 Clean Room Software Engineering

* **Goal:** To produce software with certified reliability and zero defects.
* **Approach:** Emphasizes formal methods, mathematical verification, and statistical process control rather than traditional debugging after coding. Focuses on preventing errors rather than finding them.

### 🛡️ Software Quality Assurance (SQA)

* **Definition:** A set of activities designed to ensure that software engineering processes, methods, activities, and work products are monitored and comply with defined standards.
* **Verification:** "Are we building the product right?" (Checks against specifications).
* **Validation:** "Are we building the right product?" (Checks against user needs).
* **SQA Plans:** Documents outlining the SQA activities, responsibilities, and procedures for a project.
* **Software Quality Frameworks:** Standardized approaches to managing and assuring software quality.
* **ISO 9000 Models:** International standards for quality management systems; provide a framework for organizations to ensure they consistently meet customer and regulatory requirements.
* **CMM Models (Capability Maturity Model):** (See Lesson 1 notes for more detail on maturity levels). A framework for assessing and improving the maturity of an organization's software processes.

---

## Unit II: Requirement Analysis

### 📝 Requirements Capturing (Requirements Engineering)

The process of defining, documenting, and maintaining software requirements.

* **Elicitation:** The process of gathering requirements from stakeholders through various techniques (interviews, workshops, brainstorming).
* **Specification:** Documenting the gathered requirements clearly, unambiguously, and completely (e.g., in an SRS).
* **Validation:** Confirming that the documented requirements are correct, complete, consistent, and reflect stakeholder needs.
* **Negotiation:** Resolving conflicts among stakeholders' requirements and reaching a consensus.

* **Prioritizing Requirements (Kano Diagram):**
    * A model that classifies customer preferences into five categories:
        * **Must-be Quality:** Basic features customers expect (dissatisfaction if absent, no satisfaction if present).
        * **One-dimensional Quality:** Performance features (satisfaction increases with presence, dissatisfaction with absence).
        * **Attractive Quality:** Unexpected features that delight customers (high satisfaction if present, no dissatisfaction if absent).
        * **Indifferent Quality:** Features that don't impact customer satisfaction.
        * **Reverse Quality:** Features that lead to dissatisfaction if present.
    * Helps prioritize features based on their impact on customer satisfaction.

* **Real-life Application using Case Study:** Requirements capturing often involves analyzing real-world scenarios and business processes to extract functional and non-functional requirements. Case studies help illustrate how this process works in practice.

### 🔍 Requirements Analysis

The process of refining, structuring, and understanding the gathered requirements.

* **Basics:** Involves breaking down high-level requirements into detailed, unambiguous specifications.
* **Scenario-based Modeling:** Describes how users interact with the system to achieve specific goals.
    * **Use Case Diagrams:** Visual representations of user interactions with a system. They show external actors and the use cases (functions) they perform.
    * **Use Case Description:** Textual detailing of a use case, including actor, precondition, post-condition, normal flow, and alternative flows.

* **UML Models (Unified Modeling Language):** A standardized graphical notation for modeling object-oriented software systems.
    * **Use Case Diagram:** (As above) Illustrates functional requirements from the user's perspective.
    * **Class Diagram:** Shows the static structure of a system, including classes, their attributes, operations, and relationships between classes.

* **Data Modeling:** Defines the structure and organization of data.
    * **Data Flow Model:** Shows how data moves through a system (Data Flow Diagrams - DFDs). Focuses on what data flows between processes and data stores.
    * **Control Flow Model:** Describes the sequence of operations or events in a system.

* **Behavioral Modeling using State Diagrams:**
    * **State Diagrams (State Machine Diagrams):** Describe the behavior of a system or an object in response to events. They show all possible states an object can be in and how it transitions between these states.
    * **Purpose:** Useful for modeling the dynamic aspects of a system, especially for reactive systems.

* **Real-life Application Case Study:** Applying these analysis techniques to practical scenarios to derive detailed system specifications.

### 📄 Software Requirement Specification (SRS)

* **Definition:** A comprehensive document that describes the functional and non-functional requirements of a software system.
* **Purpose:** Serves as a contract between the customer and the development team, ensuring shared understanding.
* **Qualities:** Clear, unambiguous, complete, consistent, verifiable, traceable, modifiable.
* **(See Lesson 2 notes for more detail on Requirement Analysis and SRS).**

---

## Unit III: Agile Development Process

### 🚀 Agile Development

* **Definition:** An iterative and incremental approach to software development that focuses on collaboration, customer feedback, and adapting to change.
* **Agile Manifesto:** A set of four core values and twelve guiding principles for agile software development.
    * **Values:**
        * Individuals and interactions over processes and tools.
        * Working software over comprehensive documentation.
        * Customer collaboration over contract negotiation.
        * Responding to change over following a plan.
* **Agility and Cost of Change:** Agile methods aim to reduce the cost of change by making changes early and frequently, rather than accumulating them for a large, late-stage overhaul.
* **Agility Principles:** Derived from the Manifesto, emphasizing continuous delivery, customer satisfaction, welcoming change, frequent delivery, collaboration, motivated individuals, face-to-face conversation, sustainable development, technical excellence, simplicity, self-organizing teams, and regular reflection.
* **Myth of Planned Development:** Challenges the idea that all aspects of a software project can be accurately planned upfront. Agile acknowledges uncertainty and embraces adaptive planning.
* **Toolset for the Agile Process:** Tools that support agile practices, such as project management software (Jira, Trello), version control (Git), continuous integration tools, and communication platforms.

### 🧪 Extreme Programming (XP)

* **Definition:** An agile software development framework that emphasizes a set of specific practices for high-quality, rapidly delivered software.
* **XP Values:** Simplicity, Communication, Feedback, Courage, Respect.
* **XP Process:** Follows a cyclical process of planning, designing, coding, and testing, with constant feedback loops.
* **Industrial XP:** Adapts XP principles and practices for larger, more complex organizational contexts.

### 🏃 SCRUM

* **Definition:** A popular agile framework for managing complex adaptive problems, while productively and creatively delivering products of the highest possible value.
* **Scrum Process Flow (Scrum Cycle):** Iterative cycles called "Sprints" (typically 1-4 weeks).
    1.  **Product Backlog:** A prioritized list of features, functions, requirements, enhancements, and fixes for the product.
    2.  **Sprint Planning Meeting:** Team selects items from the Product Backlog to work on during the sprint and creates a Sprint Backlog.
    3.  **Sprint Backlog:** A subset of the Product Backlog, containing the items chosen for the current sprint, along with the plan for delivering them.
    4.  **Sprint Execution:** The development team works on the Sprint Backlog items.
    5.  **Daily Scrum Meeting (Daily Stand-up):** A short (15-minute) meeting where the Development Team synchronizes activities and plans for the next 24 hours. (What did I do yesterday? What will I do today? Any impediments?)
    6.  **Maintaining Sprint Backlog:** The Sprint Backlog is dynamic and updated daily by the Development Team.
    7.  **Burn-down Chart:** A chart that shows the amount of work remaining in a sprint or project over time. Used to track progress.
    8.  **Sprint Review:** An informal meeting at the end of the sprint where the Development Team demonstrates the completed increment to stakeholders and gathers feedback.
    9.  **Retrospective:** A meeting where the Scrum Team inspects itself and creates a plan for improvements to be enacted during the next sprint.

* **Scrum Roles:**
    * **Product Owner:** Represents the voice of the customer and stakeholders; manages and prioritizes the Product Backlog.
    * **Scrum Master:** Facilitates the Scrum process, removes impediments, and ensures the team follows Scrum rules. (Servant-leader).
    * **Development Team:** A self-organizing, cross-functional team responsible for delivering the product increment.
```

