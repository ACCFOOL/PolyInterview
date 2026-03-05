<div align="center">
  <h1>PolyInterview</h1>
  <img alt="PolyInterview" src="./source/hero.png" width="900">
  <p><strong>AI-powered mock interviews with real-time feedback to help you land your dream job.</strong></p>
  <p>
    <img alt="Python" src="https://img.shields.io/badge/python-3.8%2B-blue">
    <img alt="Vue" src="https://img.shields.io/badge/vue-2.6-42b883">
    <img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen">
  </p>
</div>

> **⚠️ ATTENTION (PolyU Only)**  
> This platform is open to **PolyU students and staff**.  
> Please connect to **PolyUWLAN** first, then access:  
> **https://158.132.255.205/**

---
## Introduction 🌍
Job interview preparation is often high‑stress, fragmented, and ineffective. **93% of candidates experience anxiety before interviews.** Compounded by a lack of constructive feedback, many job seekers are left without a clear path to improvement.

PolyInterview is an end‑to‑end AI interview platform that bridges this gap. It delivers instant, structured, and multimodal feedback through an immersive real‑time **Digital Human Interviewer**.

We address the limitations of existing solutions:
- **Human Coaching:** costly ($100+/hr) and requires scheduling.
- **Peer Mock Platforms:** inconsistent quality and unreliable partners.
- **Text/Voice AI:** lacks visual immersion and “face‑to‑face” pressure.

Why now? The demand for scalable, realistic remote interview practice is surging. Only a real‑time digital human can provide the necessary immersive presence to truly prepare candidates for high‑stakes interactions, all while being affordable and available 24/7.

<div align="center">
  <img alt="Login Page" src="./source/SCR-20260131-rjnu.png" width="900">
</div>

---
## Features ✨
- 🤖 **Interview Simulation:** generate personalized question sets tailored to the company and role.
- 🗣️ **Immersive Digital Human:** experience real‑time lip‑sync interaction with a lifelike digital interviewer (powered by LiveTalking + Wav2Lip).
- 📝 **Actionable Reports:** get detailed, per‑question scoring and specific improvement guidance.
- 🔄 **Closed‑Loop Flow:** seamlessly move from question generation → interview practice → evaluation → iteration.

---
## Project Introduction & Theoretical Foundation 📚
PolyInterview is a comprehensive, AI‑powered job interview simulation platform. It goes beyond simple Q&A by leveraging a sophisticated **multi‑agent LLM architecture** to guide candidates through the entire preparation journey—from interview setup to final performance evaluation.

Our goal is to help candidates master both general interview techniques and position‑specific skills through personalized, multimodal feedback in a highly realistic simulated environment.

### Core System Workflow & Architecture 🧭
The platform operates on an intelligent multi‑agent architecture that orchestrates the entire preparation journey:

1. **Question Generation Agents**
   - **Interview Planner Agent:** builds the interview plan and question list.
   - **Interviewer Agent:** delivers questions and triggers follow‑ups.
2. **Performance Evaluation Agent:** performs **Feature Assessment** (Professional Performance, Way of Expression, Non‑verbal Behavior, Oral Expression), then aggregates results into **Aspect Assessment** and **Proficiency Assessment**, producing evaluation results and improvement suggestions.

<img alt="PolyInterview Workflow" src="./source/System_Level.drawio.png" width="900">

### Intelligent Question Generation Logic 🧩
The platform ensures practice relevance by dynamically generating interview questions that align inquiry types with KSA/STAR/Big‑Five dimensions, tailored to the specific job description (JD).

The system strategically deploys different question types:
- **Self‑introduction:** to establish a baseline for communication traits.
- **Behavioral Questions:** to probe past actions, assessing traits and cultural fit.
- **Skill QA:** to directly assess technical capabilities and domain knowledge.
- **Scenario Simulation:** to evaluate problem‑solving abilities in hypothetical job situations.

Example: for a technical role requiring programming expertise and collaboration, the system generates Skill QA questions targeting technical requirements and Behavioral questions targeting team‑oriented traits. Mapping follows the diagram: **KSA** emphasizes Skill QA, **STAR** structures scenario/behavioral responses, and **Big‑Five** supports trait‑focused behavioral analysis.

**Adaptive follow‑ups:** To maintain a smooth and natural interview process, the system will check **Consistency**, **Clarity**, and **Relevance** of the answers, and adaptively generate follow‑up questions to challenge contradictory answers, probe unclear points, and handle irrelevant responses.

### Theoretical Assessment Frameworks 🧠
To provide objective and structured feedback, the assessment engine is grounded in robust theoretical frameworks that define candidate competency and communication effectiveness.
KSA defines what is evaluated, STAR defines how responses are structured, and Big-Five provides a behavioral interpretation layer.

**KSA Competency Framework (Knowledge, Skills, Abilities)** [4]
- **Knowledge (K):** domain‑specific information applied to job tasks.
- **Skills (S):** learned proficiencies demonstrated through performance.
- **Abilities (A):** underlying capacity to perform observable behaviors.

**STAR Method (Expression Technique)** [5]
- **Situation (S):** the context or background of the scenario.
- **Task (T):** your responsibility or goal.
- **Action (A):** the specific steps you took.
- **Result (R):** the outcome and impact.

**Big‑Five Personality Model (Behavioral Traits)** [6]
- **Openness, Conscientiousness, Extraversion, Agreeableness, Neuroticism** as a trait lens for behavioral and communication assessment.

**🟦 Multimodal Interview Assessment Framework**  
This section explains the internal evaluation architecture and theoretical grounding of PolyInterview. [1–3]

- **Inputs:** **Text**, **Audio**, **Video** from the interview session.
- **Models:**  
  - **LLM** for text understanding  
  - **VLM** for visual/non‑verbal cues  
  - **Audio‑LLM** for speech and vocal delivery
- **Aggregation:** scores flow from **Feature → Aspect → Proficiency**, where features are per‑response signals, aspects summarize cross‑response dimensions, and proficiency provides the overall evaluation.

<img alt="Overall Assessment Framework" src="./source/overall-assessment-framework.png" width="900">

### References 📖
1. Hollandsworth Jr, J. G., Kazelskis, R., Stevens, J., & Dressel, M. E. (1979). Relative contributions of verbal, articulative, and nonverbal communication to employment decisions in the job interview setting. *Personnel Psychology*, 32(2), 359–367.
2. Martín‑Raugh, M. P., Leong, C. W., Roohr, K. C., & Chen, X. (2023). Perceived conscientiousness and openness to experience mediate the relationship between vocal and visual features and hiring decision in the interview. *Computers in Human Behavior Reports*, 10, 100272.
3. Martín‑Raugh, M. P., Kell, H. J., Randall, J. G., Anguiano‑Carrasco, C., & Banfi, J. T. (2023). Speaking without words: A meta‑analysis of over 70 years of research on the power of nonverbal cues in job interviews. *Journal of Organizational Behavior*, 44(1), 132–156.
4. U.S. Office of Personnel Management. *General Schedule Qualification Policies* (KSA definitions).  
5. Indiana University School of Public Health Career Services. (2018). *What is the STAR Interview Method?*
6. McCrae, R. R., & John, O. P. (1992). An introduction to the five‑factor model and its applications. *Journal of Personality*, 60(2), 175–215.
---
## Interface Preview 🖥️
### Interview Setting
<div align="center">
  <img alt="Interview Setting" src="./source/屏幕截图_31-1-2026_20045_localhost.jpeg" width="900">
</div>

### Interview
<div align="center">
  <img alt="Interview" src="./source/屏幕截图_31-1-2026_20239_localhost.jpeg" width="900">
</div>

### Assessment Report (Sample)
<div align="center">
  <img alt="Assessment Report" src="./source/屏幕截图_31-1-2026_2104_localhost.jpeg" width="900">
</div>

---
## Version Updates
<details>
<summary style="font-size: 1.5em; font-weight: bold;">Version 0.3.0 (2026-03-05)</summary>

### Added

**Core Platform**
- Implement CSRF protection with Flask-WTF and automatic token management for SPA
- Add Nginx reverse proxy configuration with one-click LAN deployment script and SSL certificate generator
- Add tiered rate limiting: strict for auth endpoints (30/15min), relaxed for authenticated routes (100/15min)
- Add ProxyFix middleware for correct client IP and HTTPS detection behind Nginx

**Digital Human**
- Support multiple avatars running on dedicated ports with per-avatar request routing
- Add WebRTC connection retry with exponential backoff for unstable networks

### Changed

**Core Platform**
- Enforce FLASK_SECRET_KEY as required environment variable with startup validation
- Replace hardcoded HTTPS protocol with environment-aware API URL resolution supporting both Nginx proxy and direct-connect modes
- Use cryptographically secure random IDs across all services
- Add wildcard route redirect to login page for unauthenticated paths

**Frontend**
- Create dedicated admin API axios instance to decouple from auth API base URL

### Fixed

**Digital Human**
- Resolve 504 gateway timeout errors on unstable networks by adding /offer request timeout and retry logic

**Frontend**
- Unify CV terminology and fix UI wording inconsistencies

</details>

<details>
<summary style="font-size: 1.5em; font-weight: bold;">Version 0.2.3 (2026-03-04)</summary>

### Added

**Core Platform**
- Migrate Auth Service database from SQLite to PostgreSQL with Docker Compose
- Add SonarQube project configuration for code quality analysis
- Enhance CORS settings to allow dynamic IP origins in development environment

**Interview System**
- Add recording processing state with visual feedback during transitions

### Changed

**Core Platform**
- Relax password validation rules to minimum 6 characters with no complexity requirements
- Replace password hash column with role tag in admin dashboard

### Fixed

**Core Platform**
- Update auth service port numbers for development and testing environments

**Interview System**
- Reset recording button state correctly after follow-up questions
- Disable recording button while loading next question

</details>

<details>
<summary style="font-size: 1.5em; font-weight: bold;">Version 0.2.2 (2026-03-03)</summary>

> **Concurrency & Security Audit:** This release focuses on a comprehensive concurrency
> and security review across all services, addressing thread-safety issues, authentication
> enforcement, and configuration hardening identified during the audit.

### Added

**Core Platform**
- Unify admin login with JWT-based role authentication, replacing the separate admin login page with automatic role-based redirect

**Interview System**
- Add recording processing state with visual feedback to prevent duplicate submissions during audio/video transitions

**Backend**
- Add `log_highlight` logger utility for formatted interview Q&A console display

### Changed

**Interview System**
- Migrate audio capture from deprecated ScriptProcessorNode to AudioWorkletNode for improved performance and browser compatibility

### Fixed

**Core Platform**
- Harden configuration security: enforce strong JWT secrets, move credentials to environment variables, disable Flask debug by default, and remove SSL private keys from version control
- Enforce JWT authentication middleware and role-based authorization across all API routes, eliminating IDOR vulnerabilities
- Add CORS origin validation, rate limiting, and security response headers
- Enforce secure cookie flags, password complexity policy, and token revocation support

**Backend**
- Add path traversal prevention and input validation for all file upload and retrieval operations
- Fix thread-safety issues: per-session data isolation, file locking, singleton service locking, UUID-based filenames, and bounded thread pool
- Fix AI service concurrency and user registration race conditions
- Remove Timer leak risk and add thread-safe singleton locking to evaluation services
- Sanitize error responses to prevent internal path and stack trace exposure

**Interview System**
- Fix STT WebSocket reconnect loop and audio upload race condition
- Remove JWT authentication from STT WebSocket to resolve connection failures
- Resolve audio recording race condition and ASR FINAL event timeout handling

**Frontend**
- Add missing score badge background colors in feedback evaluation views
- Reset auth form state when toggling between login and register modes

</details>

<details>
<summary style="font-size: 1.5em; font-weight: bold;">Version 0.2.1 (2026-02-26)</summary>

> **Architectural Refactor (In Progress):** This release begins a large-scale refactor
> across backend and frontend to reduce file size, improve modularity, and enforce
> separation of concerns. The refactor is not yet complete — remaining tasks (including
> replacing `print()` statements with structured logging) are deferred to future releases.

### Changed

**Backend**
- Split monolithic `interview.py` (2073 lines) into 7 focused route blueprints
  (`interview_session`, `interview_questions`, `interview_answers`, `interview_evaluation`,
  `interview_history`, `interview_report`, `interview_misc`) plus a new `domain/` layer
  (score rules, legacy converter, dir resolver) and `repositories/` layer
  (interview log read/write operations, evaluation repository)
- Split `evaluation_service.py` into focused service modules: `nonverbal_service.py`
  (+455 lines) and `pronunciation_service.py` (+102 lines), each handling a single
  evaluation concern
- Split `pdf_service.py` into a `services/pdf/` subpackage with 5 dedicated modules:
  `constants`, `styles`, `page_number`, `score_components`, and `table_builders`

**Interview System**
- Split `FeedbackStage.vue` from 2730 lines down to 579 lines by extracting 6
  sub-components for score display, dimension breakdown, improvement suggestions,
  and report actions
- Split `SurveyModal.vue` from 881 lines down to 409 lines by extracting
  `SurveyQuestionRenderer.vue` and a `useSurveyLogic` composable
- Extract session lifecycle and PDF export logic from `InterviewSimulation.vue` into
  dedicated `useSessionManagement.js` and `usePDFExport.js` mixins; add JSDoc to all
  mixins

**Resume Optimization**
- Split `CVRevise.vue` into 5 sub-components under `features/resume/`:
  `JobInputForm`, `AnalysisLoading`, `ScoreCard`, `ComparisonPanel`, and
  `SuggestionsList`, each with its own mixin

**Frontend**
- Complete migration from flat `components/` directory to feature-based `features/`
  directory structure covering all major modules
- Split `MaterialRecommendation.vue` and `PositionRecommendation.vue` into modular
  feature directories each containing sub-components (`CVUploadCard`, `ChatMessage`,
  `ChatInputArea`, `UserInfoBanner`, `JobCard`, `PreferencesForm`) and composable mixins
- Split `Profile.vue` into `AccountInfoCard`, `BasicInfoCard`, and
  `InterviewHistoryCard`; split `Main.vue` into `HeroSection`, `FeatureGrid`,
  `ProcessSteps`, `HomeHeader`, and `HomeFooter`; split `Landing.vue` into `AuthCard`
  and `LandingIntro`
- Unify repeated page header markup across views into a shared `PageHeader` component;
  extract `ResumeUploadSection` as a reusable shared component

### Fixed

**Security**
- Add DOMPurify XSS sanitization to all HTML rendering points in the interview module
  to prevent cross-site scripting vulnerabilities

**Backend**
- Replace bare `except` clauses with typed exception handlers across backend services
- Remove redundant `sys.path` manipulation and clean up dead code files introduced
  during the repository split

**Frontend**
- Remove all `console.log` statements from production frontend code
- Fix empty `catch` blocks by adding proper error handling or explicit ignores
- Remove dead code and unused imports; standardize API call patterns across components

</details>

<details>
<summary style="font-size: 1.5em; font-weight: bold;">Version 0.2.0 (2026-02-25)</summary>

### Added

**Core Platform**
- Centralize port configuration in `config/ports.json` with multi-environment support

**Frontend**
- Extract hardcoded frontend parameters (media, digital human, API) into centralized config modules
- Add delete history and sign out features to Profile page

### Changed

**Frontend**
- Redirect root path `/` to `/login` as the primary login entry point

### Fixed

**Interview System**
- Wait for ASR `[FINAL]` event before closing WebSocket on stop to prevent incomplete STT results
- Align video upload and heartbeat timeouts to 10 minutes to prevent premature upload failures

**Evaluation System**
- Remove legacy nonverbal analysis methods that were shadowing the updated implementation

**Digital Human**
- Fix ffmpeg-related function causing video processing errors

</details>

<details>
<summary style="font-size: 1.5em; font-weight: bold;">Version 0.1.0 (2026-02-11)</summary>

### Added

**Core Platform**
- Build AI-powered interview preparation platform with resume optimization and mock interviews
- Implement user authentication system with JWT, profiles, and admin dashboard
- Enable HTTPS across all services with SSL certificate generation
- Add maintenance page for graceful server updates

**Digital Human**
- Integrate digital human interviewer powered by LiveTalking, Wav2Lip, and WebRTC streaming
- Implement session pool for multi-user concurrent access
- Support multiple interviewer avatars with distinct voices and difficulty levels (Basic/Intermediate/Advanced)
- Add interviewer style selection with customizable prompts

**Interview System**
- Implement 5-stage interview flow: Setup, Queue, Loading, Live, and Feedback
- Generate personalized interview questions via LLM based on resume, position, and JD
- Add real-time speech-to-text using Qwen3-ASR
- Support adaptive follow-up question generation
- Add pronunciation assessment with WAV recording
- Display real-time audio waveform visualization during interview
- Play closing response from digital human after interview ends

**Evaluation System**
- Implement competency-based evaluation framework (V2) with 13 features, 10 aspects, and final scores
- Add VLM-based non-verbal behavior analysis (eye contact, facial expression, body posture, gesture)
- Enable real-time per-question evaluation during interview
- Unify scoring to 0-10 scale across all dimensions
- Generate aspect and feature summaries with improvement suggestions
- Add PDF evaluation report download
- Add JSON sanitizer for robust LLM response parsing

**Frontend**
- Add landing page with embedded login and welcome back card
- Display user avatar and profile navigation in header
- Support job position selection with company and JD input
- Add user survey in evaluation feedback page
- Add interviewer selector with info tooltips

**Backend**
- Add unified colored logging system with structured logging
- Centralize model configuration for one-click provider switching
- Support DashScope international endpoint (Singapore)
- Add unified service startup for digital human and STT
- Extract prompts to external template files for maintainability

### Changed
- Migrate STT from AssemblyAI to Qwen3-ASR with upgraded models
- Simplify interviewers from 5 to 3 with difficulty progression
- Unify question_index to 1-based throughout the system
- Replace transcript textarea with audio waveform visualization
- Make JD optional in interview setup

### Fixed
- Remove double division by 10 in oral expression score calculation
- Resolve VLM race conditions causing API 400 errors
- Correct score scaling for Logic and VLM dimensions
- Fix question scores showing 0 in feedback stage
- Prevent closing message audio cutoff on interview end
- Handle None scores in pronunciation assessment
- Prevent atexit from killing services on reloader restart
- Separate interview and media timestamps for unique filenames
- Wait for async question evaluations before finalizing results
- Fix digital human connection and video format conversion issues

</details>

<!-- - **2026-01-31** — Added high‑demand queue stage for interview sessions and improved session orchestration.
- **2026-01-30** — Added user‑facing workflow manual, updated architecture visuals, and refreshed hero assets.
- **2025-12-15** — Introduced real‑time digital human interviewer powered by LiveTalking + Wav2Lip.
- **2025-11-01** — Launched structured assessment reports. -->

