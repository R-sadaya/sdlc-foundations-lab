# STUDENT WORKSHEET: SDLC, AGILE, DEVOPS & GIT FOUNDATIONS

**Course Code / Subject:** NTC_PC14 -Software Engineering  
**Student Name:** Rhafael J. Sadaya  
**Date:** August 28,2026 **Section:** 3.5 BSIT  
**GitHub Repository URL:** [[https://github.com/________________________/sdlc-foundations-lab](https://github.com/________________________/sdlc-foundations-lab)
](https://github.com/R-sadaya/sdlc-foundations-lab)
---

## PART 1: GITHUB ONBOARDING & SETUP VERIFICATION

### Part 1: GitHub Account Creation & Onboarding

**Objective:** Set up a centralized remote repository environment for future CI/CD and GitFlow collaboration.

#### 1. Account Registration
* Go to [github.com](https://github.com) and click **Sign Up**.
* Enter your academic email address, create a strong password, and select a professional username (e.g., `j-perminola`).
* Complete the verification puzzle and enter the launch code sent to your email.

#### 2. Profile & Security Setup
* Set your display name to your full name and upload a profile picture.
* Go to **Settings > Password and authentication** and enable Two-Factor Authentication (2FA) using an authenticator app or SMS.

#### 3. Verification Task
* Click the **+** icon in the top right and select **New repository**.
* Name the repository `sdlc-foundations-lab`, set visibility to **Public**, check **Add a README file**, and click **Create repository**.
* Copy your public repository URL to submit alongside Part 2.

#### Task Checklist
- [ ] Created GitHub account using academic email.
- [ ] Enabled Two-Factor Authentication (2FA) in Settings.
- [ ] Created public repository named `sdlc-foundations-lab` with a README.md.
- [ ] Pasted public repository link in the header above.

---

## PART 2: REAL-WORLD ENGINEERING SCENARIOS

### Scenario A: SDLC & Framework Selection

**Context:** A fintech company wants to release a new peer-to-peer payment feature. A government regulatory agency requires complete compliance auditing before release, but competitors are rapidly capturing market share.

**Task:**
1. Compare Waterfall vs. Agile (Scrum) for this launch using the criteria below:
   * Adaptability & Time-to-Market
   * Regulatory & Compliance Risk Handling
2. Choose a hybrid or primary framework (e.g., Scrum vs. Waterfall vs. Spiral). Explain your reasoning in 2–3 sentences.

#### 1. Framework Comparison Table

| Criteria | Waterfall | Agile (Scrum) |
| :--- | :--- | :--- |
| **Adaptability & Time-to-Market** | Low adaptability; features are released all at once at the end of a long development cycle. | High adaptability; delivers working features iteratively in short 1–4 week sprints for faster market entry. |
| **Regulatory & Compliance Risk Handling** | Excellent for strict compliance because documentation, design, and audits are completed upfront. | Requires continuous compliance checks per sprint, increasing the risk of missing regulatory sign-offs if audits aren't built into user stories. |

#### 2. Framework Recommendation & Justification
Which primary or hybrid framework (e.g., Scrum, Waterfall, or Spiral) do you recommend for this fintech regulatory project? Explain your choice in 2–3 sentences.

**Answer:** 

I recommend a Hybrid Framework (Agile-Waterfall) for this project. This approach allows the development team to use Agile (Scrum) for rapid, iterative feature updates and fast time-to-market, while utilizing Waterfall’s structured phase gates for upfront regulatory compliance and final formal auditing before public release.

### Scenario B: DevOps & CI/CD Pipeline Breakdown

**Context:** A team merges code, but the production app breaks during deployment because testing was done manually on individual laptops rather than in an automated pipeline.

#### 1. Gap Analysis
Identify where the communication and process breakdown occurred between Dev and Ops.

**Answer:** 

The breakdown occurred because developers tested code manually in isolated local environments rather than through a standardized, automated continuous integration system. This created an environment discrepancy ("it works on my machine") where untested deployment configurations passed into production without Ops validation or automated regression testing.

#### 2. Pipeline Stage Identification
Fill in the missing stages of the continuous assembly line and circle/bold the stage that catches local testing bugs before production release:

Plan → Code → Build →  Test  → Release → Deploy → Operate → Monitor

---

### Scenario C: Git Lifecycle & Branching Strategy

#### 1. Data Movement Command Mapping
Write the standard Git command used to transfer code between each environment:

* **Working Directory → Staging Area:** `git` add .
* **Staging Area → Local Repository:** `git` commit -m "your message"
* **Local Repository → Remote Repository (GitHub):** `git` push origin <branch-name>  
* **Remote Repository → Working Directory:** `git` pull origin <branch-name>

#### 2. GitFlow Collision Prevention
Explain how utilizing Feature Branches and a Develop branch prevents two developers from overwriting each other's code on Main. (2 to 3 sentences)

**Answer:** 

Isolated feature branches allow developers to write and test code independently without modifying the core codebase directly. Changes are merged into a shared develop branch via Pull Requests, which trigger code reviews and automated tests to resolve merge conflicts and bugs before anything is safely deployed to main.

---

## FINAL SUBMISSION CHECKLIST
- [ ] Part 1 checklist completely verified.
- [ ] All scenario questions answered clearly.
- [ ] Repository set to Public for grading access.
