# VALOR — Veteran Adaptive Life-Assistance and Operations Robot System

> A distributed mobile robot fleet for comprehensive veteran support across all 20 domains of veteran life. This is a personal idea and project and this repository is not affiliated with the VA. Claude AI from Anthropic was used for this project.

[![System Status](https://img.shields.io/badge/status-concept--phase-blue)]()
[![Archetypes](https://img.shields.io/badge/robot%20archetypes-5-teal)]()
[![Capabilities](https://img.shields.io/badge/capability%20modules-20-purple)]()
[![Version](https://img.shields.io/badge/version-6.0-orange)]()
[![License](https://img.shields.io/badge/license-VA%20Research-green)]()
[![Future-Proofed](https://img.shields.io/badge/future--proofed-100yr%20mandate-gold)]()

---

## Table of Contents

1. [Vision](#vision)
2. [The Case for a Robot Fleet](#the-case-for-a-robot-fleet)
3. [System Overview](#system-overview)
4. [Design Principles](#design-principles)
5. [The Mobility Imperative](#the-mobility-imperative)
6. [Veteran Personalization Profile](#veteran-personalization-profile)
7. [VALOR-CORE Backbone](#valor-core-backbone)
8. [Robot Archetypes](#robot-archetypes)
   - [SENTINEL — Mental Health & Crisis Guardian](#sentinel--mental-health--crisis-guardian)
   - [NEXUS — Physical Health & Mobility Platform](#nexus--physical-health--mobility-platform)
   - [ATLAS — Social Life & Community Bridge](#atlas--social-life--community-bridge)
   - [HERALD — Benefits, Administration & Financial Guardian](#herald--benefits-administration--financial-guardian)
   - [PHALANX — External Environment & Safety Scout](#phalanx--external-environment--safety-scout)
9. [Humanoid Robot Options](#humanoid-robot-options)
10. [Inter-Robot Communication](#inter-robot-communication)
11. [Cascade Prevention — How the Fleet Works Together](#cascade-prevention--how-the-fleet-works-together)
12. [Robot Transfer & Reassignment Protocol](#robot-transfer--reassignment-protocol)
13. [Technology Architecture](#technology-architecture)
    - [Sensing Layer](#sensing-layer)
    - [AI & Compute Layer](#ai--compute-layer)
    - [Privacy & Security](#privacy--security)
14. [The 20 Veteran Challenges Addressed](#the-20-veteran-challenges-addressed)
15. [Implementation Roadmap](#implementation-roadmap)
16. [Build Roadmap & Development Plan](#build-roadmap--development-plan)
17. [Financial Case & ROI](#financial-case--roi)
18. [Policy Framework](#policy-framework)
19. [Top Development Challenges](#top-development-challenges)
20. [Day in the Life](#day-in-the-life)
21. [Future-Proofing the VALOR System](#future-proofing-the-valor-system)
    - [The Permanence Commitment](#the-permanence-commitment)
    - [Adaptive Technology Layer](#adaptive-technology-layer)
    - [Cultural & Values Evolution](#cultural--values-evolution)
    - [Shifting National Priorities & Policy Resilience](#shifting-national-priorities--policy-resilience)
    - [Emerging Veteran Demographics](#emerging-veteran-demographics)
    - [Long-Range Governance Model](#long-range-governance-model)
    - [Technology Succession Protocol](#technology-succession-protocol)
    - [The 100-Year Mandate](#the-100-year-mandate)
22. [VALOR vs. Current VA: The Gap Analysis](#valor-vs-current-va-the-gap-analysis)
    - [Where the VA Falls Short Today](#where-the-va-falls-short-today)
    - [How VALOR Closes Each Gap](#how-valor-closes-each-gap)
    - [Domain-by-Domain Comparison](#domain-by-domain-comparison)
23. [Research-to-Build Pipeline](#research-to-build-pipeline)
    - [Pipeline Philosophy](#pipeline-philosophy)
    - [Stage 1 — Research Discovery](#stage-1--research-discovery)
    - [Stage 2 — Reproducibility & Replicability Gate](#stage-2--reproducibility--replicability-gate)
    - [Stage 3 — VALOR Relevance Assessment](#stage-3--valor-relevance-assessment)
    - [Stage 4 — Integration Design Sprint](#stage-4--integration-design-sprint)
    - [Stage 5 — Prototype & Validation](#stage-5--prototype--validation)
    - [Stage 6 — Production Integration](#stage-6--production-integration)
    - [Stage 7 — Post-Integration Monitoring](#stage-7--post-integration-monitoring)
    - [Research Intake Registry](#research-intake-registry)
    - [Reproducibility Standards](#reproducibility-standards)
    - [Pipeline Governance](#pipeline-governance)
24. [Contributing](#contributing)
25. [The Standard Model of Physics — Applied to Veteran Care](#the-standard-model-of-physics--applied-to-veteran-care)

---

## Vision

VALOR addresses all 20 of the most prevalent challenges facing United States veterans through a coordinated fleet of purpose-built mobile robots. Rather than a single monolithic platform, VALOR operates as five specialized robot archetypes sharing data, context, and situational awareness across a unified AI backbone called VALOR-CORE.

> **The core insight:** Veteran suffering is systemic, not isolated. PTSD worsens sleep → deepens depression → drives addiction → destroys family and career → leads to homelessness. Single-point interventions produce marginal results. VALOR attacks the entire cascade simultaneously, in real time.

**Fleet at a glance:**

| Attribute | Value |
|---|---|
| Robot archetypes | 5 |
| Capability modules | 20 |
| Shared AI backbone | VALOR-CORE |
| Compute model | Edge + cloud hybrid |
| Integration targets | VA API, EHR, VA Schedule |
| Target population | 18.2M U.S. veterans |
| High-priority cohort | ~3M with PTSD, TBI, or MST |

---

## The Case for a Robot Fleet

A coordinated robot fleet is not a futuristic luxury — it is the most practical response to the scale, complexity, and persistence of the challenges veterans face. The following arguments support VALOR's approach.

### 1. The Human Caregiver Gap Is Structural, Not Temporary

The VA faces a chronic workforce shortage. In 2023, the VA reported over 50,000 unfilled clinical positions nationwide. Rural veterans — roughly 5 million — live in counties with no VA facility within a 60-minute drive. VALOR robots do not call in sick, do not relocate, and do not require a federal hiring process. They can be deployed to a rural veteran's home within days of need identification, filling gaps no amount of hiring can close at the current rate.

### 2. Continuity of Care Is the Hardest Problem — Robots Solve It Directly

The most dangerous moments for veterans are the gaps between appointments: the weekend after a difficult therapy session, the three weeks between refills, the night a nightmare returns and no one answers the phone. Human support is episodic; robot support is continuous. VALOR's always-present sensors detect crisis signals in the 168 hours between weekly check-ins that currently go completely unobserved.

### 3. The ROI Is Compelling at the National Scale

A single prevented psychiatric hospitalization saves $28,000–$45,000. A single prevented veteran suicide represents $1.5M in lifetime economic value and an immeasurable human cost. With ~6,000 veteran suicides per year and roughly 37,000 veteran hospitalizations annually attributable to mental health crises, even a 5% reduction in each metric funds the entire VALOR program many times over. Robots are not expensive — leaving veterans unsupported is expensive.

### 4. Stigma Is a Killing Field — Ambient Robots Bypass It

Research consistently shows that veterans underuse mental health services due to stigma. A 2021 RAND study found that fewer than half of veterans with PTSD sought treatment, with stigma cited as a primary barrier. Veterans are significantly more likely to disclose distress to a non-judgmental AI interface than to a human provider in a clinical setting. VALOR meets veterans in their own homes, on their own terms, before shame prevents them from reaching out at all.

### 5. Technology Readiness Is Now — This Is No Longer Speculative

The hardware required for VALOR — onboard LiDAR, biometric wrist sensors, edge-capable AI inference, mobile robot navigation, voice NLP, and robotic arms — is commercially available today. Boston Dynamics, Unitree, and a dozen other manufacturers produce capable mobile platforms at decreasing cost. NVIDIA's Jetson platform enables on-robot AI inference at the power envelope required. The VA already operates an EHR API and telehealth infrastructure that VALOR integrates with directly. This is an integration and deployment problem, not a research problem.

### 6. Veterans Deserve Support at the Scale of Their Sacrifice

The United States has spent over $2 trillion on post-9/11 veteran benefits and care — yet suicide rates, homelessness, and unemployment among veterans remain persistently higher than the civilian population. The gap between what veterans are owed and what they receive is not a funding gap alone — it is a systems gap. A fleet of intelligent, persistent, interconnected robots is the first intervention proposal that matches the complexity and duration of what veterans actually face.

### 7. Mobile Robots Close the Gap That Stationary Technology Cannot

Every assistive technology deployed in veteran homes to date — tablets, smart speakers, telehealth stations, medication dispensers — shares a fundamental limitation: it stays where it is placed. Veterans in crisis do not always go to where the device is. Veterans in pain do not always have the energy to walk to the medication station. Veterans with PTSD may freeze in the hallway, dissociate in the bedroom, or spiral in a room the device cannot see.

Mobile robots eliminate this gap. VALOR robots navigate to wherever the veteran is — not to where the designer assumed they would be. This is not an engineering optimization; it is the foundational design requirement that makes every other VALOR capability clinically viable. A stationary SENTINEL with the world's best biometric sensors is still useless if the veteran having a crisis is in the bathroom and the robot is docked in the living room.

---

## System Overview

VALOR is not a replacement for human caregivers, VA providers, or peer support specialists. It is the always-present connective tissue between a veteran and every support system that exists for them — lowering the barrier to access, preventing crises before they occur, and ensuring no veteran falls through the cracks because navigating the system requires more energy than they have on a given day.

Each robot in the fleet:
- **Navigates autonomously** throughout the veteran's home (and outdoors, for PHALANX) — bringing support to wherever the veteran is
- Operates independently when needed
- Shares state continuously with all other fleet members via VALOR-CORE
- Hands off tasks to the appropriate archetype when a situation spans domains
- Falls back to full offline-capable operation when connectivity is unavailable

---

## Design Principles

### 1. Distributed Intelligence
No single robot carries the full burden. Each archetype is optimized for its domain. A companion robot is not built to dispense medication — a clinical robot is. But they share state, so the companion knows when medication has been missed and responds accordingly.

### 2. Privacy by Architecture
Sensitive data — especially MST, mental health, and substance use — is processed on-device by default. Cloud sync is opt-in per module. Veterans retain data sovereignty. No data is shareable with DoD, employers, or law enforcement without explicit consent and a court order.

### 3. Ambient, Not Intrusive
VALOR robots are designed to fade into the background when not needed. They do not speak unless spoken to during low-activity periods. Form factors are chosen to avoid stigmatizing the veteran in social situations.

### 4. Cascade Prevention
Each robot continuously monitors upstream signals for downstream risks. The sleep robot's worsening data triggers a gentle nudge from the companion robot before depression deepens. Prevention is cheaper and kinder than crisis response.

### 5. Deep Personalization
Every veteran carries a unique combination of service history, diagnosis, cultural background, family structure, and personal preferences. VALOR-CORE is not a generic AI assistant — it is a continuously-learning model built around one person. The fleet adapts its behavior, communication style, and intervention strategies to that individual, not to a population average.

### 6. Mobility as Mission Architecture
VALOR robots are mobile by design because the veteran's life is mobile. Static support devices require veterans to come to the device; VALOR comes to the veteran. Mobility is what enables crisis response at any location in the home, medication delivery to a veteran in pain, companionship in the space where the veteran actually spends time, and outdoor escort beyond the front door. For every archetype except HERALD in its standard configuration, mobility is not a feature — it is the prerequisite for every other capability.

---

## The Mobility Imperative

> **Mobility is not a convenience feature. It is the architectural foundation that separates VALOR from every stationary assistive technology that came before it — and it is the single most important factor in whether a robot can actually help a veteran in crisis.**

A fixed device can inform, remind, or alert. A mobile robot can *intervene*. The distinction is not cosmetic — it is the difference between a system that waits for a veteran to come to it and a system that comes to the veteran, wherever they are in their home, at the moment they need it most.

---

### Why Mobility Is Mission-Critical

**1. Crises do not happen at desks.**

Veterans with PTSD, TBI, or depression do not enter crisis states in front of a display unit. They dissociate in the bedroom at 2 AM. They freeze in the hallway. They curl up on the bathroom floor. A robot that cannot reach those spaces cannot respond to what happens in them. The 30-second crisis escalation target that defines VALOR's safety guarantee is only achievable if the robot physically has line-of-sight, audio contact, and sensor proximity — none of which are possible from a fixed dock in another room.

**2. Medication, therapy, and assistance must come to the veteran — not the reverse.**

A veteran with limited mobility, a severe pain episode, or a PTSD freeze response cannot always walk to where help is stationed. NEXUS's dispensing arms, heat/cold therapy, and physical assist capabilities are only useful if the robot can navigate to where the veteran is. Requiring the veteran to travel to the robot during a health event inverts the purpose of the system.

**3. Physical presence affects therapeutic outcomes in ways that audio-video cannot replicate.**

Research on social robotics consistently demonstrates that embodied, proximate presence produces stronger rapport, trust, and therapeutic alliance than screen-based interaction — especially for populations with social withdrawal, hypervigilance, or trauma. SENTINEL's passive redirect capabilities (e.g., displaying a calming photo at the living room doorway during a dissociation episode) depend on the robot being *in the room*, positioned correctly, at the right moment. A wall-mounted screen cannot do this.

**4. The home is not a single room.**

A veteran's daily life spans bedroom, kitchen, living room, bathroom, yard, and vehicle entrance. A robot confined to one location monitors a fraction of that space. The full 20-domain support that VALOR promises requires continuous environmental awareness across the entire home — which requires robots that move.

**5. Outdoor mobility extends the perimeter of care.**

Isolation and agoraphobia are among the most debilitating secondary effects of PTSD and other service-connected conditions. A veteran who cannot safely leave their home without a trusted companion is effectively imprisoned by their own symptoms. PHALANX's outdoor mobility is not supplemental — it is the mechanism by which VALOR extends its care perimeter beyond four walls and reconnects veterans to the communities, green spaces, and physical activity that clinical evidence consistently links to mental health recovery.

---

### Mobility Requirements by Archetype

| Archetype | Mobility Requirement | Why It Matters |
|---|---|---|
| **SENTINEL** | Autonomous indoor multi-room navigation; silent drive motors; obstacle avoidance; docking with wireless charging | Must reach veteran anywhere in the home within 60 seconds; passive redirects require physical proximity; crisis detection requires unobstructed sensor proximity |
| **NEXUS** | Full indoor navigation including tight spaces (bathrooms, bedrooms); articulated arm reach augmented by position; fall-response co-location | Medication dispensing, pain therapy, and physical assist all require physical co-presence; fall detection response requires rapid co-location |
| **ATLAS** | Quiet rolling presence in living areas; autonomous docking when veteran has visitors; proximity-aware social modulation | Companionship effectiveness scales with proximity; social check-ins require in-room presence; docking behavior prevents social intrusion |
| **PHALANX** | Outdoor ruggedized mobility; GPS-guided route scouting; curb-climbing capability; sustained outdoor operation | Outdoor escort requires real-time physical co-navigation; trigger environment detection requires proximity-based environmental sensing; fall response in outdoor terrain requires robustness |
| **HERALD** | Optional mobile capability (see below) | Primary value is administrative; mobility unlocks important secondary capabilities |

---

### Mobility as a Safety Architecture

Beyond individual use cases, mobility is a **fleet safety architecture**. When NEXUS detects a fall, it broadcasts to the fleet — and PHALANX physically locks the perimeter while SENTINEL navigates to the veteran's location. When SENTINEL detects a crisis signal in the bedroom, it routes to the doorway rather than triggering a cold audio alert. These coordinated physical responses are only possible because the robots can move.

The VALOR 30-second crisis escalation guarantee implicitly requires mobility. A stationary SENTINEL in the living room that detects a crisis biometric signal from a wrist module cannot confirm the veteran's condition, cannot make physical contact, cannot visually confirm consciousness, and cannot serve as a co-located communications anchor for the 988 dispatcher. A mobile SENTINEL can do all of these things within the escalation window.

> **Mobility is not what makes VALOR a robot fleet. It is what makes the fleet capable of the promises it makes.**

---

### Mobility Standards and Specifications

All mobile VALOR archetypes are designed to meet the following baseline mobility standards:

| Standard | Specification |
|---|---|
| **Indoor navigation** | ROS 2 Nav2-based autonomous navigation; 2D LiDAR + stereo RGB-D obstacle avoidance; dynamic re-routing around people and pets |
| **Floor clearance** | Threshold traversal up to 15mm (handles standard door thresholds and transition strips); tested on hardwood, carpet, tile |
| **Speed** | Maximum 0.8 m/s indoors (designed for safe co-habitation); crisis-response sprint mode at 1.2 m/s |
| **Noise profile** | Target < 35 dB at 1m during normal navigation; silent mode < 25 dB for overnight operation |
| **Battery and availability** | 12-hour continuous operation (SENTINEL, NEXUS); 8-hour outdoor operation (PHALANX); autonomous return-to-dock before battery depletion; wireless charging dock standard |
| **Safe-stop protocol** | Immediate halt within 100ms of any obstacle within 200mm; force-limited contact detection on all exterior surfaces |
| **Outdoor specs (PHALANX)** | IP65 weather resistance; GPS + LiDAR; curb-climb up to 50mm; 8-hour outdoor battery; tested in rain, temperature range −10°C to 50°C |

---

## Veteran Personalization Profile

At enrollment, every veteran completes a **VALOR Personalization Intake** — a structured onboarding process that seeds VALOR-CORE with the context needed to serve them specifically. This profile is owned by the veteran, editable at any time, and stored under Tier-1 privacy protections.

### Core Profile Categories

| Category | Data Collected | Example Use |
|---|---|---|
| **Service history** | Branch, MOS/rate, deployment theaters, discharge type, combat exposure | SENTINEL calibrates PTSD trigger sensitivity; ATLAS finds peer matches by MOS |
| **Diagnoses & conditions** | VA-rated conditions, TBI severity, chronic pain locations, mobility limitations | NEXUS configures medication timing; PHALANX plans safe outdoor routes |
| **Communication style** | Preferred tone (direct/warm/clinical), language preference, humor tolerance, text vs. voice | All robots adapt interaction style; reduces friction and builds rapport |
| **Cultural & spiritual background** | Religious affiliation, cultural identity, spiritual practices | SENTINEL integrates preferred chaplain/spiritual care provider; ATLAS sources culturally relevant peer groups |
| **Family & relationship structure** | Spouse/partner, children (ages), caregiver relationships, next of kin | ATLAS family reintegration modules adapt to household; emergency contacts configured |
| **Triggers & sensitivities** | Known PTSD triggers (sounds, environments, topics), social anxiety thresholds | PHALANX reroutes around identified trigger environments; SENTINEL adjusts topic handling |
| **Goals & motivations** | Stated recovery goals, employment aspirations, education interests, personal values | ATLAS career coach aligns to veteran's own goals; HERALD prioritizes relevant benefit programs |
| **Hobbies & interests** | Activities the veteran enjoys, communities they belong to, topics they care about | SENTINEL uses familiar topics for grounding; ATLAS sources relevant social events |
| **Sleep patterns** | Preferred sleep/wake time, sleep medication use, known sleep disorder type | SENTINEL sleep module operates within veteran's established rhythms |
| **Medication preferences** | Pill vs. liquid aversion, side effect sensitivities, pharmacy preference | NEXUS dispenser configuration; HERALD pharmacy coordination |

### Continuous Profile Updates

The personalization profile is not static. VALOR-CORE updates it continuously based on:
- Explicit veteran input ("I want to stop getting sports updates")
- Behavioral inference ("Veteran consistently dismisses morning reminders — shift to evening")
- Clinical events (new VA diagnosis triggers module reconfiguration)
- Life transitions (job start, move, marriage, loss of family member)

> **Veteran control:** Every profile field includes a visibility toggle. Veterans can choose which robots see which data, and can audit VALOR-CORE's understanding of them at any time via the HERALD display unit.

---

## VALOR-CORE Backbone

All robots share a unified AI backbone: **VALOR-CORE**. This is a personalized, continuously-learning model trained on the veteran's health history, preferences, communication style, service record, and VA records. VALOR-CORE is the memory, the context, and the coordinator. Individual robots are its hands, eyes, and voice.

**VALOR-CORE responsibilities:**

- Persistent cross-robot memory of the veteran's full life context
- Real-time inter-robot state sharing (e.g., PHALANX sleep data informs SENTINEL mood assessment)
- VA API integration for claims, appointments, and benefits
- EHR read/write with VA and community providers
- Anomaly detection across all 20 data streams simultaneously
- Emergency escalation to Veterans Crisis Line (988), emergency contacts, or 911 within **30 seconds** of threshold breach

**Infrastructure:** VALOR-CORE runs as a cloud-native service on VA-owned, FedRAMP-High infrastructure. Edge modules on each robot handle latency-sensitive processing without cloud dependency.

---

## Robot Archetypes

### SENTINEL — Mental Health & Crisis Guardian

**Nickname:** "The Guardian"  
**Domain:** Continuous mood, crisis, and behavioral health monitoring  
**Form factor:** Mobile desktop companion (~tablet on wheeled base); **autonomous multi-room mobility is core to its crisis-response mission** — it navigates silently between rooms to maintain sensor proximity to the veteran at all times; warm non-humanoid curved display; always-on local-only wake detection; silent-mode drive motors for overnight navigation without sleep disruption  
**Mobility rationale:** SENTINEL's 30-second crisis escalation guarantee, passive redirect interventions, and real-time biometric monitoring all depend on physical proximity to the veteran. A stationary SENTINEL cannot fulfill its mission — a veteran in crisis in the bedroom is unreachable by a unit docked in the living room.  
**Humanoid option:** See [Humanoid Robot Options](#humanoid-robot-options) — SENTINEL-H variant available for veterans who respond better to embodied social presence

**Capability modules:**

| Module | Description |
|---|---|
| PTSD stress-detection | HRV, galvanic skin response, voice-pattern analysis, cortisol proxy via wearable wrist module; triggers grounding protocols in real time |
| TBI cognitive-support | Speech-to-text memory logging, facial recognition for name recall, task/calendar prompting with vibration reminders, cognitive load tracking |
| Depression & suicide risk monitor | NLP mood analysis of all verbal interactions, activity-level tracking, Veterans Crisis Line (988) escalation in under 30 seconds |
| Sleep environment management | Smart home IoT control of lighting and temperature, white noise/soundscape engine, sleep-stage tracking via mattress sensor pad, VA sleep clinic data export |
| Substance-craving intervention | Physiological pre-craving signal detection, distraction and peer-sponsor connection protocols, sobriety milestone reinforcement |
| Grief & moral injury module | Guided narrative journaling with AI reflection, chaplain/spiritual care video connection, memorial archive for fallen comrades |
| MST recovery support | Offline-only encrypted sessions, trauma-informed voice persona options, self-compassion exercises, confidential MST specialist video link |

**Key integration:** SENTINEL is the primary mood sensor for the fleet. Its depression and stress signals propagate to ATLAS (social scheduling), HERALD (appointment management), and NEXUS (medication adherence monitoring).

---

### NEXUS — Physical Health & Mobility Platform

**Nickname:** "The Medic"  
**Domain:** Integrated physical support, medication management, and therapeutic intervention  
**Form factor:** Largest fleet unit (~bedside clinical cart); articulated arms with soft-robotics grippers (3 kg payload); 12-hour battery; wireless charging dock; designed for indoor home environments; **full autonomous mobility throughout the home is essential** — NEXUS navigates to the veteran's location to deliver medications, pain therapy, and physical assistance rather than requiring a mobility-limited or pain-affected veteran to travel to a fixed station  
**Mobility rationale:** Veterans with limb loss, Parkinson's, chronic pain, or post-fall states cannot reliably come to a docked unit for time-sensitive care. NEXUS's value proposition collapses without the ability to navigate to wherever the veteran needs it — especially in fall-response scenarios where rapid co-location is a safety requirement.  
**Humanoid option:** See [Humanoid Robot Options](#humanoid-robot-options) — NEXUS-H variant provides upper-body assist in a form factor that transfers more intuitively to physical therapy exercises

**Capability modules:**

| Module | Description |
|---|---|
| Chronic pain management | TENS therapy delivery arms, heat/cold therapy pad dispensers, posture-correction vibration alerts via wearable harness, AI-optimized medication timing |
| Smart medication dispenser | Robotic pill sorting and scheduled dispensing, drug-interaction cross-reference against VA pharmacy database, missed-dose alerts to VA provider |
| Prosthetic interface coordinator | Bluetooth sync with myoelectric prosthetics, real-time calibration feedback, secondary grip-assist arm for fine motor tasks during prosthetic adjustment |
| Hearing support array | 360-degree directional microphone, real-time speech amplification and transcription to wrist display, tinnitus masking tones via bone-conduction earpiece |
| AI vision system | Ambient narration of surroundings, document reading aloud, facial identification, obstacle detection, high-contrast enlargement on companion screen |
| Mobility assist module | Laser-guided path planning for wheelchair/walker navigation, smart home integration for doors and height adjustment, morning item pre-positioning |
| Elder-care cognitive support | Gamified cognitive fitness exercises, validated dementia screening tools, fall detection via floor pressure sensors, caregiver alert system |

**Key integration:** NEXUS shares medication adherence data with SENTINEL (mood correlation) and HERALD (VA pharmacy auto-refill). Mobility and fall data propagate to PHALANX for outdoor escort planning.

---

### ATLAS — Social Life & Community Bridge

**Nickname:** "The Connector"  
**Domain:** Combating isolation, rebuilding relationships, and facilitating reintegration  
**Form factor:** Compact rolling unit (~large speaker on base); minimal display surface; **near-silent mobility throughout living areas is central to its therapeutic function** — ATLAS navigates to wherever the veteran is spending time rather than requiring social engagement to happen in a fixed location; quiet, slow-moving; designed for living rooms and common areas; docks autonomously when veteran has visitors  
**Mobility rationale:** The therapeutic value of companionship depends on presence in the same space as the veteran. An ATLAS docked in a hallway cannot provide ambient social engagement to a veteran in the kitchen. Mobility allows ATLAS to follow the veteran's daily rhythm rather than forcing the veteran to adapt their movement to where the robot is stationed.  
**Humanoid option:** See [Humanoid Robot Options](#humanoid-robot-options) — ATLAS-H variant for veterans whose primary challenge is social isolation; embodied presence shown to reduce loneliness metrics more effectively than screen-based interaction

**Capability modules:**

| Module | Description |
|---|---|
| Companionship AI | Persistent memory of life story, service history, preferences, and relationships; adapts conversation depth to detected energy levels |
| Social calendar management | Pulls local veteran events (VFW, DAV, VA Community), schedules weekly social contact, facilitates group video calls, tracks social health for VA records |
| AI career coach | Translates military service record to civilian job language, searches and matches job listings, runs mock interview sessions, tracks application pipeline |
| Family communication facilitator | Structured reintegration conversation guides, evidence-based family education modules, couples/family counseling booking, age-appropriate explanations for children of veterans |

**Key integration:** ATLAS receives SENTINEL mood scores to modulate social outreach intensity. Low social engagement scores trigger HERALD to book a VA community care referral.

---

### HERALD — Benefits, Administration & Financial Guardian

**Nickname:** "The Advocate"  
**Domain:** VA benefits navigation, financial management, legal support, and administrative burden reduction  
**Form factor:** Desktop-docked display unit with touchscreen interface; serves as the veteran's primary VALOR-CORE dashboard; **does not require mobility to fulfill its core mission** — HERALD's value is software, data, and communication, all of which function from a fixed station

> **HERALD and Mobility: A Design Deliberation**
>
> HERALD is the only VALOR archetype whose primary mission does not require physical mobility. Its core functions — benefits filing, document management, appointment coordination, financial monitoring — are fundamentally digital and can be delivered from a fixed display unit in the veteran's home. Mandating mobility for HERALD would add cost, mechanical complexity, and battery management burden without a proportionate clinical benefit.
>
> **However, mobility is a meaningful optional upgrade for HERALD**, and veterans or VA programs may elect to deploy a mobile HERALD variant based on the following documented benefits:
>
> **1. Room-to-Room Accessibility.** Veterans with limited mobility, chronic pain, or PTSD-driven room avoidance may not reliably travel to a fixed HERALD station. A mobile HERALD can navigate to wherever the veteran is — the bedroom after a difficult morning, the living room during a rest period — ensuring that critical administrative tasks (appointment reminders, claim deadlines, benefit alerts) are surfaced at the right moment, in the right space.
>
> **2. Dynamic Fleet Coordination.** In a mobile configuration, HERALD can physically co-locate with NEXUS or SENTINEL during multi-robot coordination events — for example, positioning itself near the veteran during a post-fall recovery sequence to surface insurance information or initiate a VA telehealth connection without requiring the veteran to move to another room.
>
> **3. Proactive Document Scanning.** HERALD relies on NEXUS's document scanner in the standard configuration. A mobile HERALD with an integrated document scanner module can navigate to where documents are kept (kitchen table, filing cabinet area, desk) and initiate scanning workflows without requiring the veteran to transport documents.
>
> **4. Home Visit Support.** When VA field workers, VSO representatives, or legal aid visitors come to the veteran's home, a mobile HERALD can navigate to the meeting location and serve as an interactive briefing station — displaying relevant records, claim summaries, and appointment histories in the room where the conversation is actually happening.
>
> **5. Aging-in-Place Adaptability.** As veterans age and their mobility declines, a fixed HERALD station can become inaccessible. A mobile variant future-proofs HERALD's accessibility for the aging veteran cohort without requiring a hardware replacement.
>
> The standard HERALD deployment remains fixed-dock. The mobile HERALD variant is offered as a VA-prescribed upgrade for veterans whose living situation, mobility status, or care complexity indicates a clinical benefit from in-room administrative access.

**Humanoid option:** Not applicable — HERALD's administrative function does not benefit from humanoid embodiment. A mobile cart variant with enhanced display and document scanner is the preferred upgrade path.

**Capability modules:**

| Module | Description |
|---|---|
| VA benefits navigator | Automated claims filing, status tracking, appeal support; continuously scans for unclaimed benefits matching the veteran's profile |
| Document vault | Encrypted secure storage for DD-214, medical records, legal documents; OCR scanning via NEXUS document scanner |
| Financial health manager | Benefit payment tracking, budgeting tools, VA debt resolution, financial counseling booking |
| Legal resource connector | VSO referral, JAG consultation scheduling, discharge upgrade tracking |
| Appointment coordinator | Pulls VA schedule API, manages all medical and benefits appointments across the fleet |

**Key integration:** HERALD is the administrative hub of the fleet. NEXUS feeds pharmacy data for auto-refills; SENTINEL feeds mental health appointment needs; ATLAS feeds career and education program bookings. In the optional mobile configuration, HERALD co-locates physically with the veteran or with other fleet members during multi-domain care events.

---

### PHALANX — External Environment & Safety Scout

**Nickname:** "The Scout"  
**Domain:** Outdoor navigation, environmental hazard detection, and emergency response  
**Form factor:** Ruggedized wheeled outdoor unit; weather-resistant; GPS + LiDAR; **PHALANX is the fleet's mobility-forward archetype — it exists precisely because veterans' lives do not end at the front door**; runs ahead of or alongside the veteran in outdoor environments; IP65-rated for rain and dust; operates in temperature extremes; built for sustained outdoor operation across varied terrain  
**Mobility rationale:** PHALANX's entire mission is physical co-navigation in the outdoor environment. Without mobility, it cannot scout routes, detect trigger environments before the veteran enters them, escort veterans with agoraphobia on gradual exposure walks, respond to outdoor falls, or extend the perimeter of VALOR's care into the world outside the home. PHALANX is immobile only when docked — and when docked, it is not fulfilling its mission.  
**Humanoid option:** See [Humanoid Robot Options](#humanoid-robot-options) — PHALANX-H for veterans who need physical outdoor escort support

**Capability modules:**

| Module | Description |
|---|---|
| Outdoor route planning | GPS + real-time hazard avoidance; stores veteran's trigger-environment map (avoids known PTSD trigger locations) |
| Environmental threat detection | Crowd density monitoring, noise level alerts, rapid egress route suggestion |
| Emergency response | Fall detection, medical alert to 911, GPS-pinned location transmission to emergency contacts |
| Home perimeter monitoring | Exterior camera feeds, motion alerts, door/window status — security for veterans with hypervigilance |

**Key integration:** PHALANX feeds GPS location to SENTINEL for context-aware mood monitoring; shares fall risk data with NEXUS; shares perimeter data with SENTINEL for overnight security-anxiety management.

---

## Humanoid Robot Options

For veterans who respond better to embodied social presence, humanoid (-H) variants of each archetype are available. These are based on commercially available humanoid platforms (e.g., Unitree H1, Agility Digit, or equivalent) with VALOR-CORE integration. Humanoid variants are not the default — they are prescribed based on clinical assessment of the veteran's social and therapeutic needs.

**Available -H variants:**

| Variant | Base Archetype | Primary indication |
|---|---|---|
| SENTINEL-H | SENTINEL | Veterans who need embodied grounding presence; severe PTSD with touch-based calming response |
| NEXUS-H | NEXUS | Veterans requiring physical therapy guidance or transfer assist |
| ATLAS-H | ATLAS | Veterans with severe social isolation; companion presence reduces loneliness more effectively |
| PHALANX-H | PHALANX | Veterans with significant mobility or agoraphobia challenges requiring physical escort |

---

## Inter-Robot Communication

All fleet units communicate via a local mesh network (Wi-Fi 6 + Bluetooth 5.3 fallback) and sync state to VALOR-CORE. Key inter-robot data flows:

| Sending Robot | Signal | Receiving Robot | Action Triggered |
|---|---|---|---|
| SENTINEL | Elevated stress / depression score | ATLAS | Reduce social demands; gentle check-in |
| SENTINEL | Sleep degradation trend | NEXUS | Review medication timing; adjust pain protocol |
| NEXUS | Missed medication | SENTINEL | Mood correlation alert; gentle escalation |
| NEXUS | Fall detected | PHALANX | Lock perimeter; summon to location |
| PHALANX | Trigger environment detected | SENTINEL | Pre-activate grounding protocol |
| HERALD | Missed VA appointment | SENTINEL + ATLAS | Mood check; reschedule outreach |

---

## Cascade Prevention — How the Fleet Works Together

VALOR's core differentiator is its ability to detect and interrupt the downward spirals that lead to veteran crises. The following example illustrates cascade prevention in action:

> **Scenario:** A veteran's sleep quality degrades over three nights (SENTINEL sleep module). SENTINEL flags a rising HRV stress trend and alerts NEXUS to evaluate medication timing. NEXUS adjusts the pain medication schedule to reduce nighttime disruption. ATLAS reduces its social outreach cadence to avoid over-taxing the veteran. HERALD checks for a pending VA sleep clinic appointment and confirms it. SENTINEL activates a pre-configured grounding soundscape at bedtime. The crisis does not materialize.

Without VALOR, this cascade would have continued unobserved until a breaking point — an ER visit, a crisis call, or worse.

---

## Robot Transfer & Reassignment Protocol

### When a Transfer May Occur

| Trigger | Description |
|---|---|
| **Veteran relocation** | Veteran moves to a region where shipping a replacement unit is faster than transit; local unit is reassigned, replacement ships to new address |
| **Veteran death** | Fleet is respectfully decommissioned; units enter refurbishment pool for reassignment after full sanitization |
| **Veteran upgrade** | Veteran qualifies for a newer hardware generation; existing unit returns to inventory |
| **Medical transition** | Veteran transitions to full-time VA residential or nursing care; unit reassigned to a community-based veteran |
| **Voluntary return** | Veteran chooses to return one or more units (e.g., significant recovery milestone, preference change) |
| **Reallocation priority** | VA triage identifies a higher-need veteran in the same region; with outgoing veteran's consent, unit is reassigned |

### Transfer Protocol Steps

**Phase 1 — Data Sanitization (automated, ~2 hours)**
1. VALOR-CORE initiates `TRANSFER_INITIATED` flag across all fleet units
2. All Tier-1 Private data (mental health sessions, MST disclosures, financial data, personal profile) is cryptographically wiped from on-robot storage — not archived, not transferred
3. Tier-2 Clinical data is transferred to the outgoing veteran's personal VALOR-CORE archive (accessible via VA MyHealtheVet portal), then wiped from the physical unit
4. Tier-3 Operational data (navigation maps of previous home, calendar data) is wiped
5. Hardware reset to factory state — firmware is reflashed, sensor calibrations are cleared
6. Sanitization certificate generated and logged in VA asset management system

**Phase 2 — Physical Transfer**
- Robot is transported via VA logistics partner with tamper-evident sealing
- All wearable accessories (wrist module, mattress sensor pad, bone-conduction earpiece) are replaced with new units — these are never transferred between veterans
- Physical inspection checklist completed at receiving VA facility before dispatch to new veteran

**Phase 3 — Incoming Veteran Onboarding**
- Unit arrives as a blank-slate robot with no prior veteran's data present
- Standard VALOR Personalization Intake is conducted with incoming veteran
- VALOR-CORE builds a new personalization model from scratch
- Fleet syncs and integration testing performed before veteran takes custody

> **Veteran assurance:** No outgoing veteran's data, voice recordings, behavioral patterns, or personal history exists on a unit after transfer. The incoming veteran receives a robot that is, in every meaningful sense, new to them.

### Partial Fleet Transfer

A veteran may return a subset of their fleet (e.g., return NEXUS after major recovery milestone, retain SENTINEL and HERALD). Partial transfers follow the same per-unit sanitization protocol. VALOR-CORE automatically reconfigures inter-robot communication topology to reflect the reduced fleet.

### Emergency Reallocation

In a declared veteran housing crisis or mass casualty event, VA may invoke **Emergency Reallocation Authority** to rapidly redeploy available fleet units. This process compresses Phase 2 to 24 hours but does not bypass Phase 1 sanitization — data integrity is non-negotiable even under emergency conditions.

---

## Technology Architecture

### Sensing Layer

**Biometric sensors (on-body / wrist module):**
- PPG (photoplethysmography) — HRV and pulse
- EDA (electrodermal activity) — stress arousal
- Accelerometer/gyroscope — movement and falls
- Ambient cortisol proxy via skin sensor
- Microphone array — voice-pattern NLP
- Mattress pressure sensor pad — sleep staging

**Environmental sensors (robot-mounted):**
- LiDAR and stereo RGB-D cameras
- Directional audio (360-degree pickup)
- Smart home integration (Z-Wave, Zigbee, Matter protocol)
- Floor pressure mat — fall detection
- Document scanner (300 DPI, auto-crop)
- Ambient light and temperature sensors

---

### AI & Compute Layer

**Edge (on-robot) — latency-sensitive, offline-capable:**
- Real-time biometric analysis
- Voice recognition & NLP (fully offline capable)
- Obstacle detection & navigation
- MST/mental health session encryption and processing
- Emergency escalation (does not require cloud connectivity)

**Cloud (VALOR-CORE) — long-horizon, cross-robot:**
- Persistent veteran memory model
- VA API & EHR integration
- Cross-robot state aggregation and coordination
- Long-horizon trend analysis and anomaly detection
- Model updates & fleet management

**Compute hardware target:** NVIDIA Jetson Orin-class (or equivalent) per robot for edge inference. VALOR-CORE deployed on VA-owned FedRAMP-High cloud infrastructure.

---

### Privacy & Security

All sensitive data categories are classified by tier:

| Tier | Data categories | Processing location | Cloud sync |
|---|---|---|---|
| **Tier-1 Private** | Mental health sessions, MST disclosures, substance use patterns, financial information, personalization profile | On-device only | Opt-in, per-session consent |
| **Tier-2 Clinical** | Biometric readings, medication adherence, sleep data | On-device + VA EHR (with consent) | Automatic with VA provider |
| **Tier-3 Operational** | Navigation, calendar, social scheduling | Local mesh + VALOR-CORE | Automatic |

**Security standards:**
- Encryption at rest: AES-256
- Encryption in transit: TLS 1.3
- Infrastructure: VA-owned FedRAMP-High
- Data access: Veterans retain full data sovereignty; deletion on request
- Third-party access: No access for DoD, employers, or law enforcement without court order and veteran notification
- Transfer sanitization: Cryptographic wipe with certificate of completion for all unit reassignments

---

## The 20 Veteran Challenges Addressed

| # | Challenge | Primary Robot | Category |
|---|---|---|---|
| 1 | PTSD & trauma | SENTINEL | Mental health |
| 2 | Traumatic brain injury (TBI) | SENTINEL | Physical |
| 3 | Chronic pain | NEXUS | Physical |
| 4 | Limb loss / amputation | NEXUS | Physical |
| 5 | Hearing loss & tinnitus | NEXUS | Physical |
| 6 | Vision impairment | NEXUS | Physical |
| 7 | Sleep disorders | SENTINEL | Mental health |
| 8 | Substance use & addiction | SENTINEL | Mental health |
| 9 | Depression & suicide risk | SENTINEL | Mental health |
| 10 | Social isolation | ATLAS | Social |
| 11 | Unemployment | ATLAS | Social |
| 12 | Homelessness risk | ATLAS + HERALD | Social |
| 13 | MST recovery | SENTINEL | Mental health |
| 14 | VA navigation & benefits access | HERALD | Administrative |
| 15 | Medication management | NEXUS | Administrative |
| 16 | Mobility limitations | NEXUS + PHALANX | Physical |
| 17 | Grief & moral injury | SENTINEL | Mental health |
| 18 | Family reintegration | ATLAS | Social |
| 19 | Financial instability | HERALD | Administrative |
| 20 | Cognitive decline (aging veterans) | NEXUS + HERALD | Administrative |

---

## Implementation Roadmap

### Phase 1 — Foundation (Years 1–2) · $120M

- [ ] VALOR-CORE architecture development and VA API integration
- [ ] SENTINEL prototype: biometric PTSD/depression monitoring + crisis escalation
- [ ] HERALD prototype: VA benefits navigation and claims automation
- [ ] Veteran Personalization Intake framework development and validation
- [ ] Transfer & Reassignment Protocol infrastructure and logistics partnerships
- [ ] 500-unit pilot at 5 VA Medical Centers (VAMCs) — high-need veteran cohort
- [ ] IRB-approved outcome study: hospitalization rates, crisis calls, housing stability, employment
- [ ] Policy work: VA DME reclassification for AI therapeutic tools; Veteran AI Bill of Rights
- [ ] **Research-to-Build Pipeline stood up**: Research Intake Registry initialized; Research Integration Committee (RIC) constituted; Work Stream Research Liaisons assigned; Stage 1–3 intake active for all five work streams
- [ ] **Minimum 10 findings processed through the full pipeline** before any clinical AI model enters the 500-unit pilot — no pilot module proceeds without a Confidence Tier A or B classification

### Phase 2 — Expansion (Years 3–4) · $280M

- [ ] NEXUS and ATLAS brought to production quality
- [ ] Full fleet integration: all 5 archetypes operating as coordinated system
- [ ] Humanoid variant pilot: 500-unit SENTINEL-H and ATLAS-H deployment with controlled comparison study
- [ ] 5,000-unit deployment across 25 VAMCs and rural outreach programs
- [ ] Outcome data published; VA and CMS reimbursement pathway established
- [ ] Commercial licensing discussions with allied nation VA equivalents (UK, Canada, Australia)
- [ ] **Pipeline at steady-state operation**: all seven stages active; Stage 7 post-integration monitoring producing outcome data for the first Phase 1 integrations; first annual pipeline audit completed
- [ ] **Phase 1 pilot data feeds back into the pipeline**: SENTINEL and HERALD real-world outcome data entered into the Intake Registry as first-party findings; any model updates required by Phase 1 outcomes processed through Stage 4–6 before Phase 2 deployment

### Phase 3 — Scale (Years 5–8) · $800M+

- [ ] PHALANX outdoor scout brought to production; PHALANX-H variant for eligible veterans
- [ ] 50,000+ units deployed nationwide; priority to rural and underserved veterans
- [ ] VALOR-CORE published as open API for VSOs, nonprofit caregivers, community health workers
- [ ] Cost per unit at scale: $18,000–$24,000 (comparable to power wheelchair)
- [ ] Full VA reimbursement for all veterans with qualifying disability ratings (50%+)
- [ ] Transfer pool operational: refurbished units available for rapid reallocation nationwide
- [ ] **Pipeline research output published**: VALOR internal research meeting the Reproducibility Standards published in peer-reviewed literature on a Phase 1 / Phase 2 / Phase 3 cadence as committed in the Research-to-Build Pipeline
- [ ] **Third-party API integrations subject to pipeline review**: any VSO or nonprofit application built on the VALOR-CORE Open API that incorporates clinical or behavioral AI must submit their underlying research evidence to the Intake Registry for Stage 3 relevance assessment before certification

---

## Build Roadmap & Development Plan

> *This section translates the high-level Implementation Roadmap into a concrete engineering and organizational development plan — defining the teams, technical work streams, key decision gates, and sequencing required to build VALOR from first code to national deployment.*

---

### Guiding Build Principles

Before diving into milestones, the following principles govern how VALOR is built:

**1. Build the backbone before the body.** VALOR-CORE must be designed and partially validated before any robot archetype goes into production. An archetype without a functioning backbone is just a robot; the coordination layer is VALOR's core differentiator.

**2. Two archetypes first, always.** SENTINEL and HERALD are chosen as the first two archetypes because they address the most time-critical needs (crisis and benefits access) and have the lowest hardware complexity relative to their impact. They establish the integration pattern for everything that follows.

**3. Real veterans, early.** Clinical co-design with veterans and VA clinicians begins in month 3 — not after the prototype is built. The intake framework, crisis protocols, and interaction design must be shaped by the people who will use this system.

**4. Safety and privacy are not features — they are preconditions.** No archetype enters pilot testing without a completed IRB protocol, a privacy threat model, a data classification audit, and a signed VA data sharing agreement.

**5. Open hardware where possible, proprietary only where necessary.** Chassis and sensor selection favors commercially available platforms. Proprietary investment is concentrated in VALOR-CORE software, integration middleware, and clinical AI models — the elements that cannot be bought off the shelf.

---

### Work Streams

The build is organized into five parallel work streams that run across all phases:

| Work Stream | Scope |
|---|---|
| **WS-1: VALOR-CORE Platform** | Cloud backbone, veteran data model, VA/EHR integrations, inter-robot protocol |
| **WS-2: Archetype Hardware** | Chassis selection, sensor integration, edge compute, mechanical design per archetype |
| **WS-3: Clinical AI & Modules** | Biometric models, NLP, crisis detection, sleep staging, mood inference, personalization engine |
| **WS-4: Safety, Privacy & Compliance** | IRB, FedRAMP, data tier enforcement, sanitization protocol, cybersecurity |
| **WS-5: Veteran Experience & Field Ops** | Co-design, onboarding UX, logistics, field support, transfer operations |
| **WS-6: Research-to-Build Pipeline** | Research Intake Registry, RIC governance, Research Integration Briefs, ADR oversight, Stage 5 pilot protocols, post-integration monitoring |

---

### Pre-Phase 0 — Team Formation & Technical Foundations (Months 1–6)

Before any hardware is ordered or code is committed to production, the following must be in place.

#### Organizational Setup

- Hire or designate a **Chief Medical Officer** and **Chief Privacy Officer** — these roles must exist before clinical work begins, not after.
- Stand up five small cross-functional teams aligned to the five work streams above. Minimum viable team per work stream at this stage: 2–3 engineers + 1 domain lead.
- Establish a **Veteran Advisory Board** (VAB): 8–12 veterans from diverse service backgrounds, including at minimum two veterans with PTSD, one with TBI, one with MST history (with appropriate support structures), and two from rural counties. The VAB reviews all major design decisions and has formal veto power over interaction design choices.
- Execute MOU with at least two VA Medical Centers for co-design access and eventual pilot partnership.

#### Technical Foundations

- Stand up development infrastructure: cloud dev environment on FedRAMP-Moderate (upgrade to High before Phase 1 pilot), CI/CD pipeline, security scanning, audit logging from day one.
- Publish the **VALOR Data Classification Standard v1.0** — the document that defines what data belongs in Tier-1/2/3, where it can be processed, and what consent is required. This document governs all subsequent engineering decisions.
- Select and procure three candidate mobile robot chassis for SENTINEL prototype evaluation. Recommended candidates: a low-cost wheeled base (e.g., Clearpath Dingo or equivalent), a mid-tier platform with arm options, and a humanoid candidate for -H variant evaluation. Evaluate on: onboard compute capacity, sensor mounting flexibility, battery life, noise profile, and VA facility navigability.
- Begin VA API integration spike: authenticate against VA Lighthouse API sandbox, confirm EHR read/write capability in test environment, document integration constraints.

#### Clinical Co-Design (begins Month 3)

- Conduct structured interviews with 30 veterans across the high-priority cohort (PTSD, TBI, MST). Focus: what does helpful look like, what does intrusive look like, how do they feel about a robot in their home, what would make them trust it.
- Run parallel interviews with VA clinicians (psychiatrists, social workers, care coordinators) on crisis escalation protocols, clinical data expectations, and liability concerns.
- Produce a **VALOR Interaction Design Brief** that establishes verbal persona guidelines, physical presence norms, wake-word and silence protocol, and crisis response UX — before any prototype is built.

**Gate 0 deliverables before Phase 1 build begins:**
- [ ] Five work stream teams staffed
- [ ] Veteran Advisory Board constituted and first review completed
- [ ] Data Classification Standard v1.0 published internally
- [ ] VA API integration confirmed in sandbox
- [ ] VALOR Interaction Design Brief published
- [ ] Chassis candidates received and evaluated
- [ ] FedRAMP-Moderate cloud environment operational
- [ ] IRB protocol drafted (not yet submitted — submission is Phase 1 milestone)
- [ ] **Research Integration Committee (RIC) constituted** — Chief Medical Officer, five Work Stream Research Liaisons (one per WS), Clinical AI Lead, IRB & Regulatory Specialist, Veteran Advisory Board representative, and Privacy Officer advisory seat filled
- [ ] **VALOR Research Intake Registry initialized** in `valor/docs/research/` — schema live, access controls set, at least five candidate research findings submitted to Stage 1 for inaugural triage

---

### Phase 1 Build Plan — Foundation (Months 7–30)

**Budget:** $120M  
**Primary deliverables:** VALOR-CORE v1, SENTINEL prototype, HERALD prototype, 500-unit pilot, IRB outcome study initiated

#### WS-1: VALOR-CORE Platform (Months 7–18)

The backbone is built in three increments:

**VALOR-CORE v0.1 — Data Model & Auth (Months 7–10)**
- Define and implement the veteran data schema: profile, clinical records, behavioral observations, inter-robot state
- Implement veteran identity management integrated with VA Login.gov / ID.me
- Build the data tier enforcement layer: runtime policy engine that prevents Tier-1 data from leaving the device under any condition without explicit veteran consent action
- Stand up the inter-robot state bus: lightweight pub/sub protocol (MQTT or similar) that allows archetypes to publish and subscribe to state signals without requiring cloud connectivity for time-critical events

**VALOR-CORE v0.5 — VA Integrations (Months 10–15)**
- Complete VA Lighthouse API integration: benefits status, appointments, pharmacy, EHR read
- Implement EHR write pathway for clinical data: medication adherence, biometric summaries, crisis events — with VA clinician review before any write is committed
- Build the VALOR Personalization Intake as a structured interview UI: runs on HERALD display during onboarding, seeds the veteran data model
- Implement anomaly detection framework: configurable threshold engine that monitors any data stream and fires events when thresholds are crossed or trends detected

**VALOR-CORE v1.0 — Full Coordination (Months 15–24)**
- Implement the cascade prevention engine: event graph that maps signals from one archetype to recommended responses in others, configurable per veteran profile
- Build the emergency escalation pipeline end-to-end: biometric threshold → local alert → veteran acknowledgment window (30s) → automatic escalation to 988/911 with GPS and veteran profile package
- Complete FedRAMP High authorization package (this is a 6–9 month process; begin Month 10)
- Build fleet management console: VA admin dashboard for unit status, veteran assignment, sanitization certificate tracking, and remote diagnostics

#### WS-2: SENTINEL Hardware (Months 7–18)

**SENTINEL Prototype v1 (Months 7–12)**
- Select chassis from Gate 0 evaluation. Required form factor: compact wheeled base with a curved OLED/LCD display panel, **silent drive motors rated below 35 dB at 1m** (critical for overnight operation), autonomous multi-room navigation via ROS 2 Nav2, and a docking station with wireless charging. **Mobility is not optional for SENTINEL** — the crisis response guarantee is only achievable with a robot that can navigate to wherever the veteran is within the home.
- Integrate NVIDIA Jetson Orin module as edge compute unit. Validate thermal envelope and battery life under continuous inference load including active navigation.
- Integrate the biometric wrist module as a separate companion device: select and validate a PPG + EDA + accelerometer module (e.g., based on MAX86150 or similar clinical-grade sensor IC). Commission custom wrist band enclosure.
- Integrate mattress pressure sensor pad for sleep staging (select from commercially available sleep mat options; validate sleep stage accuracy against PSG gold standard in a 20-subject sleep study).
- **Validate full autonomous room-to-room navigation** in a representative home floor plan with obstacles, pets, and threshold strips — navigation reliability must exceed 98% successful room transit before pilot deployment.
- Validate that all Tier-1 biometric processing runs fully on-device with zero cloud dependency for emergency escalation.

**SENTINEL Prototype v2 (Months 12–18)**
- Integrate VALOR-CORE v0.5 connectivity
- Implement the seven SENTINEL capability modules in software: PTSD detection, TBI cognitive support, depression/suicide risk monitor, sleep environment management, substance craving intervention, grief/moral injury, MST support
- Field test with 10 veteran co-design participants: observed sessions, usability interviews, interaction design iteration
- Submit IRB protocol for the 500-unit pilot study

#### WS-2: HERALD Hardware (Months 7–14)

HERALD is the simplest hardware archetype — a docked display unit in its standard configuration — which is intentional. Its primary value is software, not mobility. However, the hardware design must accommodate a **mobile HERALD variant** as a VA-prescribed upgrade path, so the chassis and compute architecture should be designed from the outset to accept wheels and a drive system without requiring a hardware redesign.

- Select commercial touchscreen display unit as base (10–13" tablet in ruggedized kiosk enclosure, or custom build with modular base that accepts both fixed-dock and wheeled-mobile configurations)
- Integrate document scanner module (USB or embedded, 300 DPI minimum, auto-crop)
- HERALD software implementation: VA benefits navigator, document vault, financial health manager, appointment coordinator, legal resource connector
- HERALD serves as the veteran's primary VALOR-CORE dashboard — implement the profile viewer, consent manager, and data audit interface here
- **Mobile HERALD variant specification (Month 12–14):** Define the wheeled base upgrade kit; validate that HERALD software navigation layer integrates cleanly with VALOR-CORE's inter-robot positioning system; document the clinical prescription criteria under which a mobile HERALD is indicated

#### WS-3: Clinical AI Models (Months 7–24)

This work stream runs in parallel with hardware and is the most technically risk-laden area. Key models to develop or adapt:

| Model | Approach | Validation requirement | Pipeline requirement |
|---|---|---|---|
| PTSD/stress detection from HRV + EDA | Fine-tune on veteran biometric dataset; baseline from published HRV-stress literature | 80%+ sensitivity at <5% false positive rate in held-out veteran cohort | Minimum Confidence Tier B before pilot deployment; Tier A required for any autonomous escalation action |
| Mood/depression inference from voice NLP | Adapt existing speech affect models (e.g., based on openSMILE feature set + fine-tuned transformer) | Validated against PHQ-9 scores in pilot cohort | Minimum Confidence Tier B; supporting findings must pass Stage 2 reproducibility gate |
| Sleep stage classification from mattress pressure | Train on pressure-PSG paired dataset; compare to commercial sleep mat accuracy benchmarks | AHI correlation r > 0.85 vs. PSG | Minimum Confidence Tier B; population alignment must be rated High or Moderate for veteran cohort |
| Substance craving pre-signal detection | Most speculative model; begin with HRV + EDA + activity pattern features; expect to iterate | Pilot validation only in Phase 1; do not deploy as clinical decision support without Phase 2 validation | Confidence Tier C maximum in Phase 1; advisory-only; Tier B required before any autonomous craving-triggered intervention |
| VA benefits eligibility classifier | Rules-based engine cross-referenced against VA VASRD and CFR Title 38; update quarterly | 99%+ accuracy on known-benefit test cases | Rules-based engine exempt from probabilistic pipeline tiers; regulatory source citations required in Registry |

All clinical AI models are subject to a **Model Risk Review** before deployment: bias audit across demographic subgroups, adversarial input testing, and sign-off from the Chief Medical Officer.

#### WS-4: Safety, Privacy & Compliance (Months 7–24)

- Submit IRB protocol to appropriate IRB (recommend VA Central IRB for multi-site pilot) — target submission Month 16, approval by Month 20
- Complete FedRAMP High authorization — begin Month 10, target authorization by Month 22
- Conduct penetration testing of VALOR-CORE and all robot communication interfaces — minimum annually; before pilot launch
- Implement and audit the sanitization protocol on 10 test units before any real veteran data is processed
- Produce the **VALOR Privacy Impact Assessment** per OMB Circular A-130 requirements
- Draft the **Veteran AI Bill of Rights** policy brief for Congressional staffers (co-author with Veteran Advisory Board)

#### WS-5: Veteran Experience & Field Ops (Months 16–30)

- Design and test onboarding workflow: from unit delivery to fully operational fleet in under 4 hours, with a VA-trained field technician present
- Build logistics infrastructure for 500-unit pilot: warehouse, staging, shipping, field support SLA (target: next-business-day field technician dispatch for critical failures)
- Train 25 VA clinical staff at 5 pilot VAMCs on VALOR dashboard, alert interpretation, and escalation protocols
- Stand up 24/7 VALOR support line for pilot veterans — staffed by trained VA social workers, not a call center
- Establish outcome data collection pipeline: pull hospitalization rates, crisis line calls, benefits claims, employment status from VA records for IRB study cohort

**500-unit pilot (Months 22–30):**
- 100 units per VAMC; cohort selected by VA clinicians from high-need veteran population
- Each veteran receives SENTINEL + HERALD (full fleet is Phase 2)
- Outcome data collection begins at enrollment; 12-month primary endpoint
- Monthly Veteran Advisory Board review of emerging field data; fast iteration on UX issues

**Phase 1 gate deliverables:**
- [ ] VALOR-CORE v1.0 deployed on FedRAMP-High infrastructure
- [ ] SENTINEL Prototype v2 and HERALD in 500-unit pilot
- [ ] IRB approved and outcome study active
- [ ] FedRAMP High authorization received
- [ ] VA DME reclassification petition submitted
- [ ] 12-month pilot outcome data showing statistically significant reduction in hospitalization or crisis events (minimum threshold for Phase 2 funding approval)
- [ ] **Research Intake Registry active with minimum 10 findings at Stage 3 or beyond** — all clinical AI models deployed in the 500-unit pilot traceable to at least one Confidence Tier A or B finding in the Registry
- [ ] **First Research Integration Brief (RIB) published** for each of the five primary clinical AI models deployed in Phase 1
- [ ] **RIC weekly cadence established and documented** — meeting notes and stage-transition decisions recorded in the Registry for auditability

---

### Phase 2 Build Plan — Expansion (Months 31–54)

**Budget:** $280M  
**Primary deliverables:** NEXUS and ATLAS production, full fleet integration, 5,000-unit deployment, humanoid pilot, reimbursement pathway

#### NEXUS Development (Months 31–42)

NEXUS is the most mechanically complex archetype due to its articulated arms, medication dispensing requirements, and **the full indoor mobility required to bring those capabilities to wherever the veteran needs them**.

- Hardware: Select or commission a wheeled bedside platform with two 3 DOF soft-robotic arms. Evaluate commercial options (e.g., Hello Robot Stretch, or custom build on mobile base). Key requirements: **full autonomous indoor navigation** (including tight bathroom and bedroom corridors), safe force limits (ISO/TS 15066 for collaborative robotics), FDA 510(k) pathway consideration for the medication dispensing module. **Mobility must be validated in the smallest rooms of a veteran's home** — a robot that cannot navigate to the bathroom cannot respond to the most common fall scenario.
- **FDA pathway:** The smart medication dispenser module likely requires FDA 510(k) clearance as a Class II medical device. Begin pre-submission meeting with FDA in Month 31; plan 18–24 months for clearance. Deploy Phase 2 NEXUS units with dispensing module in a non-dispensing monitoring-only mode until clearance is received.
- Integrate TENS therapy delivery arms, heat/cold pad dispensers, hearing support array, and AI vision system modules.
- Prosthetic interface coordinator: partner with two commercial prosthetic manufacturers (e.g., Ottobock, Össur) for Bluetooth SDK access and calibration API.
- Validate fall detection via floor pressure mat in a 30-unit home trial before broad deployment.
- **Validate NEXUS fall-response navigation:** when a fall is detected, NEXUS must navigate to the veteran's GPS-pinned location within 90 seconds from any point in the home. This is a hard safety requirement with no acceptable failure rate in production.

#### ATLAS Development (Months 31–40)

ATLAS is primarily a software problem on relatively simple hardware.

- Hardware: Compact rolling base with a small display for video calls. Key requirement: near-silent drive motors (target < 35 dB at 1m) so ATLAS does not disrupt household activity when docked.
- Software: Companionship AI built on a fine-tuned LLM with veteran-specific personalization layer from VALOR-CORE. Key requirement: long-term persistent memory across all conversations — ATLAS must remember a veteran's stories, not just the last session.
- Career coaching module: integrate with VA SkillBridge API, USAJobs API, and LinkedIn (where veteran consents). Build MOS-to-civilian skills translation engine from O*NET crosswalk data.
- Family communication facilitator: co-design with military family organizations (Blue Star Families, NMFA); validate reintegration curriculum with licensed family therapists.

#### Full Fleet Integration (Months 36–48)

With all five archetypes in hand, the integration work is:

- End-to-end cascade prevention testing: simulate the documented cascade scenarios with instrumented test fleets. Each cascade scenario must demonstrate that the appropriate archetype responds within the defined time window.
- Stress-test the inter-robot protocol with all five archetypes active simultaneously and intentionally degraded network conditions (simulating rural broadband).
- Build and validate the partial fleet configuration system: a veteran with only SENTINEL + HERALD must still have a fully functioning cascade prevention experience within that subset.
- Fleet management tooling for VA administrators: mass firmware update, health monitoring, remote diagnostic, sanitization queue management.

#### Humanoid Pilot (Months 40–54)

- Procure 500 humanoid platform units (SENTINEL-H + ATLAS-H variants). Recommended platform evaluation: Unitree H1, Agility Digit, or equivalent at price point under $30,000/unit.
- Conduct controlled comparison study: 250 veterans assigned to standard archetype, 250 to -H variant. Primary outcome: loneliness scale (UCLA-3), therapeutic alliance score, crisis event rate. IRB amendment required.
- Establish safety protocol specific to humanoid variants: fall-over detection with self-righting or soft-fail, safe force limits for any physical contact, veteran-controlled proximity boundary.
- Humanoid deployment requires additional VA field technician training: 8-hour certification course on humanoid maintenance, safe handling, and clinical escalation for interaction incidents.

#### Reimbursement Pathway (Months 36–54)

- Publish Phase 1 pilot outcomes in peer-reviewed journal (target: JAMA or NEJM for maximum policy impact)
- Submit VALOR reimbursement dossier to VA Health Economics team: cost-per-QALY analysis, hospitalization reduction data, ROI projection at scale
- Engage CMS for Medicare/Medicaid reimbursement pathway (relevant for aging veteran cohort and VA community care referrals)
- Begin allied nation licensing discussions: UK (Veterans UK), Canada (VAC), Australia (DVA)

**Phase 2 gate deliverables:**
- [ ] All 5 archetypes in production and passing integrated fleet tests
- [ ] 5,000 units deployed across 25 VAMCs
- [ ] Humanoid pilot 12-month outcome data published
- [ ] VA reimbursement for VALOR approved for veterans with 50%+ disability rating
- [ ] NEXUS medication dispenser FDA 510(k) clearance received (or timeline confirmed)
- [ ] Phase 1 outcomes published in peer-reviewed journal
- [ ] **All NEXUS and ATLAS clinical modules traceable to Confidence Tier A or B findings** in the Research Intake Registry before production deployment
- [ ] **Phase 1 pilot outcome data entered into the Registry** as first-party findings and processed through Stage 3 relevance assessment — any material discrepancy with pre-deployment Confidence Tier assignments documented and resolved
- [ ] **First annual pipeline audit completed** — RIC publishes audit report covering tier assignment accuracy, integration timeline adherence, and Stage 7 monitoring outcomes for all Phase 1 integrations

---

### Phase 3 Build Plan — Scale (Months 55–96)

**Budget:** $800M+  
**Primary deliverables:** 50,000-unit national deployment, PHALANX production, open API, transfer pool operations, cost reduction to $18,000–$24,000/unit

#### PHALANX Development (Months 55–66)

PHALANX is the most operationally challenging archetype due to outdoor autonomy requirements — and the most mobility-dependent archetype in the fleet. **PHALANX exists entirely because of its ability to move.** Every capability it provides — route scouting, trigger avoidance, fall response, outdoor escort — is a function of locomotion. A stationary PHALANX is not a degraded PHALANX; it is a non-functional one.

- Hardware: Ruggedized wheeled outdoor platform. Requirements: IP65 weather resistance, GPS + LiDAR + stereo cameras, **8-hour outdoor battery life**, curb-climbing capability (minimum 50mm), tested across grass, gravel, pavement, and wet surfaces. Evaluate platforms: Clearpath Husky, Boston Dynamics Spot (for -H variant), or custom outdoor UGV. **All platforms must demonstrate sustained outdoor co-navigation alongside a walking human** before procurement commitment.
- Outdoor autonomy stack: build on ROS 2 Nav2 as baseline; extend with veteran-specific trigger-environment routing (PTSD trigger map must be updatable by veteran at any time; route re-planning must complete in under 10 seconds).
- **Companion walking validation:** PHALANX must maintain a configurable follow distance (default: 10–15 meters ahead as a scout; or 1–2 meters alongside as escort) while adapting in real-time to the veteran's pace, stops, and direction changes. This is the primary navigation use case.
- Emergency response module: integrate with local 911 CAD systems via RapidSOS API for GPS-pinned incident reporting.
- Home perimeter monitoring: integrate with Matter/Zigbee smart home ecosystem; validate that SENTINEL PTSD hypervigilance module correctly de-escalates when PHALANX reports perimeter clear.

#### Manufacturing & Cost Reduction (Months 55–84)

Reaching $18,000–$24,000 per unit requires deliberate manufacturing investment:

- Negotiate volume contracts with chassis manufacturers — 50,000-unit committed order is sufficient leverage for 20–30% hardware cost reduction.
- Consolidate sensor bills of materials: standardize on a single wrist biometric module, single LiDAR model, and single edge compute platform across all archetypes where possible.
- Establish two regional refurbishment centers (East and West) for the transfer pool: incoming units are inspected, sanitized, repaired to functional spec, and reissued. Target refurbishment cost: under $2,000/unit, extending unit service life to 8 years.
- Commission an independent cost audit at Month 72 to verify the $18,000–$24,000 target is on track; if not, convene a cost reduction task force with 90-day mandate.

#### Open API & Ecosystem (Months 66–84)

- Publish VALOR-CORE Open API v1.0: documented REST + WebSocket interfaces allowing third-party VSOs, state veteran agencies, and nonprofits to build applications on the platform.
- Launch VALOR Developer Program: documentation, sandbox environment, certification process for third-party integrations.
- Pilot three third-party integrations before full API launch: a VSO chapter management tool, a state-level homeless veteran outreach app, and a peer support specialist coordination tool.
- Establish the VALOR API governance board: chaired by VA, including Veteran Advisory Board representatives, with authority to approve or reject third-party integrations based on privacy and safety review.

#### National Deployment Operations (Months 66–96)

At 50,000+ units, VALOR is a national logistics operation:

- Establish 10 regional staging and support hubs aligned with VA VISN (Veterans Integrated Service Network) boundaries.
- Each hub supports: unit storage, staging and configuration, field technician dispatch, repair and maintenance, transfer pool operations.
- Field technician workforce: estimate 1 FTE per 150 active units for maintenance and onboarding support. At 50,000 units: ~330 field technicians nationwide. Hire and train in cohorts aligned with deployment wave schedule.
- Build predictive maintenance into VALOR-CORE fleet management: failure prediction models trigger proactive unit swap before veteran experiences downtime.
- Establish a VALOR National Operations Center (NOC): 24/7 monitoring of fleet health, escalation pipeline status, and crisis response metrics. Target: any escalation failure (a crisis that should have triggered 911 but didn't) investigated within 24 hours and root cause corrected within 72 hours.

**Phase 3 gate deliverables:**
- [ ] 50,000 units deployed; 40%+ in rural/underserved counties
- [ ] PHALANX in production deployment
- [ ] Unit cost at or below $24,000 verified by independent audit
- [ ] VALOR-CORE Open API published; three third-party integrations certified
- [ ] Transfer pool operational with 5,000+ refurbished units in inventory
- [ ] VALOR National Operations Center operational 24/7
- [ ] Full VA reimbursement pipeline active; CMS pathway established
- [ ] **VALOR internal research published in peer-reviewed literature** on the Phase 1 / Phase 2 / Phase 3 cadence — all publications meeting the Reproducibility Standards defined in the Research-to-Build Pipeline
- [ ] **Third-party Open API integrations subject to pipeline review** — any certified VSO or nonprofit application incorporating clinical or behavioral AI must have supporting evidence submitted to the Intake Registry and assessed at Stage 3 before certification is granted
- [ ] **Stage 7 post-integration monitoring active for all production modules** — monitoring dashboards operational in the VALOR NOC; any module whose real-world performance diverges materially from pilot expectations flagged for RIC review within 30 days of detection

---

### Key Technical Risks & Mitigations

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Clinical AI model accuracy insufficient for safe deployment | Medium | Critical | Phase-gated validation requirements; models start as advisory-only before clinical decision support clearance |
| FedRAMP High authorization delayed | Medium | High | Begin process Month 10; run on FedRAMP-Moderate for development; no real veteran data until High authorized |
| FDA 510(k) clearance for medication dispenser denied or delayed | Medium | High | Design NEXUS to function without dispensing module; dispenser is additive, not required for fleet value |
| Veteran trust and adoption lower than projected | Medium | High | VAB co-design from Month 3; opt-in everything; never deploy features veterans did not ask for |
| Humanoid platform vendor delivers unreliable hardware | Medium | Medium | Evaluate 3 platforms before committing; pilot 500 units before scaling; maintain non-humanoid variant as default |
| Biometric wrist module accuracy insufficient for PTSD detection | Medium | High | Validate against clinical PTSD assessment tools in 100-person study before pilot deployment; publish results |
| Inter-robot coordination latency too high for cascade prevention | Low | Medium | Requires LAN-speed mesh; test under degraded rural broadband; design offline-capable fallback for all critical protocols |
| Robot mobility system failure in a safety-critical scenario | Medium | High | Mobility systems are the highest-stress mechanical component; design crisis escalation to initiate from wrist module independently of robot position; target 18+ month MTBF for drive systems; 48-hour replacement SLA required before Phase 3 |
| Cybersecurity breach of veteran Tier-1 data | Low | Critical | FedRAMP High; on-device only processing for Tier-1; penetration test every 6 months; breach response plan maintained and rehearsed |
| Research pipeline bottleneck delays clinical module deployment | Medium | High | RIC weekly cadence and defined stage timelines (Section 22) prevent queue buildup; Confidence Tier C findings may proceed to advisory-only deployment while full pipeline review completes, ensuring clinical value is not blocked by process overhead |
| Real-world pilot outcomes contradict pipeline Confidence Tier assignments | Low | High | Stage 7 post-integration monitoring designed specifically for this; any material discrepancy triggers mandatory RIC review and possible model rollback within 72 hours via the fleet management console |

---

### Team & Hiring Plan

| Phase | Headcount (cumulative) | Key hires |
|---|---|---|
| Pre-Phase 0 | 25–35 | CTO, CMO, CPO, 5 WS leads, 4 senior engineers per WS, 2 clinical researchers, **WS-6 Research Pipeline Lead** |
| Phase 1 | 80–120 | Clinical AI engineers (×6), VA integration engineers (×4), IRB/regulatory specialist, field operations lead, 25 field technicians for pilot, **5 Work Stream Research Liaisons** (one per WS, responsible for Stage 1 discovery and Registry submissions) |
| Phase 2 | 200–280 | Mechanical engineers for NEXUS arms (×4), ATLAS software engineers (×6), humanoid robotics specialists (×4), reimbursement/health economics analyst, 100 field technicians, **Clinical AI Replication Analyst** (responsible for Stage 2 reproducibility review and internal replication commitment) |
| Phase 3 | 500–700 | Manufacturing partnerships team, open API developer relations, 330 regional field technicians, NOC operators (×20), refurbishment center staff (×60), **Stage 7 Monitoring Analysts (×3)** (sustained post-integration monitoring across all production modules at national scale) |

---

### Summary Timeline

```
Year 1    [Pre-Phase 0 ──────────][Phase 1 begins ────────────]
Year 2    [Phase 1: VALOR-CORE + SENTINEL + HERALD ──────────]
Year 3    [Phase 1 pilot 500 units][Phase 2 begins ────────────]
Year 4    [Phase 2: NEXUS + ATLAS + 5,000 units ──────────────]
Year 5    [Phase 2 close][Phase 3 begins: PHALANX + open API ─]
Year 6    [Phase 3: scale to 50,000 units ───────────────────]
Year 7    [Phase 3: national ops + transfer pool ────────────]
Year 8    [Phase 3: full reimbursement + ecosystem maturity ─]
```

---

## Financial Case & ROI

| Metric | Current cost (no intervention) | VALOR projected impact |
|---|---|---|
| Veteran psychiatric hospitalization | $28,000–$45,000 per episode | $12,000–$20,000 prevented per veteran/year |
| Chronic homelessness (annual system cost) | $35,000–$50,000 per veteran/year | Prevention eliminates cost entirely |
| Untreated PTSD (lost productivity) | $17B/year nationally | 10% reduction = $1.7B/year recovered |
| Veteran suicide (lifetime economic loss) | $1.5M per life lost | 1% reduction = $450M/year saved nationally |
| VA benefits unclaimed per veteran | $4,200–$9,600/year left on table | Full recovery via HERALD auto-filing |

> All figures are estimates based on published VA and CBO research. See [VALOR System Vision v1.0](./VALOR_System_Vision.docx) for full citations and methodology.

### Research Pipeline Investment & Financial Justification

The Research-to-Build Pipeline is not a cost center — it is the financial risk management layer for the entire program. Every VALOR clinical module that reaches a veteran represents a capital investment that can be voided by a single failed deployment, a post-market FDA safety action, or a congressional inquiry triggered by a high-profile adverse event.

The pipeline adds an estimated **$8M–$12M in cumulative operating cost across Phases 1–3** (Research Pipeline Lead + 5 WS Research Liaisons + Clinical AI Replication Analyst + Stage 7 Monitoring Analysts + registry infrastructure). Against a total program budget of $1.2B+, this represents under 1% of total cost.

The financial return on that investment is:

- **Avoided failed deployments:** A clinical AI model deployed without adequate evidence review that causes a material adverse event (e.g., a missed crisis escalation in a module later shown to have a reproducibility failure in its foundational research) could result in a program funding suspension, an FDA enforcement action, and reputational damage that sets the program back 2–4 years. At a program burn rate of $280M in Phase 2, a 6-month suspension costs $140M — 14× the total pipeline operating cost over all three phases.
- **CMS reimbursement acceleration:** CMS reimbursement pathway development requires a body of peer-reviewed clinical evidence. The pipeline's Reproducibility Standards and publication cadence directly produces that evidence on a structured timeline — accelerating reimbursement approval and unlocking the sustainable funding pathway that reduces dependence on annual appropriations.
- **VA procurement confidence:** VA procurement officers and Congressional appropriators are more likely to fund subsequent phases when Phase 1 outcomes are published under the rigorous standards of the pipeline's Reproducibility Standards commitment, rather than appearing as self-reported internal metrics. Published, pre-registered outcome data is the strongest financial argument for Phase 2 and Phase 3 authorization.

**Pipeline budget allocation within phase budgets:**

| Phase | Total Budget | Pipeline Operating Estimate | % of Budget |
|---|---|---|---|
| Phase 1 | $120M | $3M–$4M | 2.5–3.3% |
| Phase 2 | $280M | $3M–$4M | 1.1–1.4% |
| Phase 3 | $800M+ | $2M–$4M | 0.3–0.5% |

---

## Policy Framework

Building VALOR requires parallel policy development alongside engineering. The following legislative and regulatory changes are prerequisites for full deployment:

**1. VA DME Reclassification**
Update the VA Schedule for Rating Disabilities (VASRD) and CMS reimbursement codes to classify AI-assisted therapeutic robots as Durable Medical Equipment, enabling VA purchase and veteran ownership for veterans with qualifying disability ratings (50%+).

**2. Veteran AI Bill of Rights**
Federal legislation establishing data sovereignty for therapeutic AI interactions — prohibiting DoD, employer, and law enforcement access without court order and veteran notification.

**3. VALOR Pilot Authorization**
Congressional authorization and $120M appropriation for Phase 1 pilot under 38 U.S.C. § 7303 (VA research authority), with mandatory 3-year outcome reporting to Congress.

**4. Rural Deployment Priority**
At least 40% of Phase 2 units directed to veterans in rural counties with VA facility access gaps exceeding 60 minutes drive time.

**5. Open-Source VALOR-CORE API**
After Phase 2 validation, VA required to publish open API enabling VSOs, state veteran agencies, and nonprofits to build on the VALOR-CORE platform — enabling a veteran-care ecosystem beyond the core fleet.

**6. Robot Transfer Liability Framework**
Federal regulations governing data sanitization standards for reassigned VA-issued AI systems, establishing legal liability for sanitization failures and certifying the Transfer & Reassignment Protocol as the federal standard for therapeutic robot reuse.

---

## Top Development Challenges

> *This section identifies the highest-priority obstacles to completing the VALOR fleet — technical, regulatory, organizational, and human. These are not hypothetical risks; they are the real walls that must be climbed for VALOR to reach veterans.*

---

### 1. Clinical AI Validation & FDA Regulatory Clearance

**Category:** Regulatory / Technical  
**Severity:** Critical

Every VALOR module that influences a clinical decision — SENTINEL's crisis escalation, NEXUS's medication dispenser, NEXUS's TENS therapy delivery — is a medical device under FDA jurisdiction. Each requires either 510(k) clearance or De Novo classification before it can be deployed with real veterans. The AI models underlying mood and PTSD detection must meet a standard of clinical evidence comparable to a medical diagnostic tool, not a consumer wellness app. This is a multi-year process per module.

**Why it's hard:** The FDA's AI/ML-based Software as a Medical Device (SaMD) framework is still maturing. Predicate devices for AI-powered robotic therapeutic companions do not yet exist in cleared form, which forces De Novo rather than 510(k) pathways — substantially longer timelines. Each software update to a cleared model may trigger a new review cycle under current guidance.

**Mitigation path:** Phase-gate every clinical module as advisory-only until cleared. Begin FDA pre-submission meetings in Month 6 of Phase 0. Design NEXUS and SENTINEL to deliver full non-clinical value independently, so regulatory delays on specific modules do not halt fleet deployment.

---

### 2. Veteran Trust, Privacy Perception, and Adoption

**Category:** Human / Social  
**Severity:** Critical

A robot in the home that monitors mood, biometrics, conversations, and daily behavior — even one with rigorous privacy protections — faces a deeply skeptical audience. Veterans have legitimate reasons to distrust data systems. The DoD and VA have a documented history of data breaches, disability rating disputes, and benefit denials. Many veterans fear that disclosing mental health struggles through a VA-connected device will affect their disability ratings, employment screenings, or gun rights.

**Why it's hard:** Trust cannot be engineered. It must be built through co-design, transparency, and consistent behavior over time. A single high-profile privacy failure — or even a credible rumor of one — could set adoption back by years. Veteran communities are tightly networked; negative word-of-mouth travels fast.

**Mitigation path:** Veterans Advisory Board co-designs every interaction pattern from Month 3 onward. Tier-1 data never leaves the device unless the veteran explicitly consents, per session. HERALD provides an always-accessible full audit log of what VALOR-CORE knows and what it has shared. Legal carve-outs banning DoD/employer access are written into the operating contract, not just policy guidance.

---

### 3. VALOR-CORE AI Accuracy, Drift, and Explainability

**Category:** Technical  
**Severity:** High

VALOR-CORE must simultaneously model a veteran's mood, medication adherence, social isolation, physical health trends, and crisis risk — and act on that model in real time. AI models degrade over time as the veteran's life changes. A model trained on a veteran in acute crisis may behave incorrectly for that same veteran in stable recovery two years later. Worse, when VALOR-CORE makes a wrong call — misses a crisis, over-escalates a benign event, recommends the wrong coping strategy — the consequences can be severe.

**Why it's hard:** Clinical-grade AI with a personalized, longitudinally updating model is at the frontier of what is practically achievable today. Explainability — the ability for the veteran or their VA provider to understand *why* VALOR made a given recommendation — is a technical challenge unsolved in production at this scale. Veterans and providers will not trust a black box.

**Mitigation path:** All VALOR-CORE outputs are advisory by default; escalation to crisis services requires a second sensor confirmation before automated action. Build an explainability layer that surfaces reasoning in plain language to the veteran and provider. Establish a continuous validation pipeline that flags model drift against real outcome data from the VA EHR.

---

### 4. VA System Integration and API Reliability

**Category:** Technical / Organizational  
**Severity:** High

VALOR's value proposition depends on deep integration with VA systems: the EHR (VistA/Oracle Health), benefits claims (eBenefits/VA.gov API), pharmacy, scheduling, and the Veterans Crisis Line. These systems are notoriously fragmented, inconsistently documented, and frequently unavailable during maintenance windows. Securing and maintaining the necessary API access, data permissions, and compliance approvals across all VA systems is a multi-year organizational effort that cannot be accelerated by engineering alone.

**Why it's hard:** The VA operates dozens of legacy systems across hundreds of facilities, many of which do not speak the same data standard. VA IT modernization (the Oracle Health EHR rollout) has been delayed repeatedly and is still incomplete as of the current planning horizon. A VALOR integration built against one VA system configuration may break silently when that facility migrates.

**Mitigation path:** Build VALOR's VA integration layer as a dedicated abstraction service with facility-level configuration. Engage VA's Digital Transformation Center (DTC) as a formal technical partner from Phase 0. Design all VALOR modules to degrade gracefully when VA API access is unavailable rather than failing outright.

---

### 5. Hardware Reliability, Maintenance, and Cost at Scale

**Category:** Engineering / Operations  
**Severity:** High

A robot operating 24 hours a day in a home environment — navigating pets, clutter, children, and elderly veterans with mobility limitations — will break. Articulated arms, wheels, drive motors, sensors, and batteries all have finite mean-time-between-failure (MTBF) ratings. **The mobility systems — drive trains, wheels, navigation sensors — are among the most mechanically stressed components in the fleet**, operating continuously across varied floor surfaces, thresholds, and obstacles. For a veteran who depends on NEXUS for daily medication dispensing or SENTINEL for crisis monitoring, a mobility failure is a safety event, not just a support ticket: a robot that cannot navigate cannot reach the veteran. Building and sustaining a field maintenance infrastructure capable of servicing tens of thousands of units nationwide is an operational challenge that rivals the engineering challenge.

**Why it's hard:** Consumer robotics companies have largely failed at the service model. The robots that require the most reliable support — those serving elderly, disabled, or high-need populations — are precisely the robots whose users cannot self-troubleshoot. Rural deployment makes dispatch logistics extremely expensive and slow. Mobility system failures (jammed wheels, navigation sensor degradation, dock alignment failures) are the most common failure mode across wheeled robot platforms in home environments.

**Mitigation path:** Design all critical safety functions (crisis escalation, medication reminders) to fail over to a smartphone app when robot hardware fails. Target MTBF of 18+ months for all critical components including mobility systems through supplier qualification in Phase 0. Build a certified remote technician program enabling over-the-phone guided repair for common failure modes. Establish a regional depot network with 48-hour replacement SLA as a Phase 3 deployment gate. Validate mobility systems specifically across floor surface types, threshold heights, and obstacle profiles representative of the veteran home environments in the pilot cohort.

---

### 6. FedRAMP High Authorization and Cybersecurity

**Category:** Regulatory / Security  
**Severity:** High

VALOR-CORE handles Tier-1 veteran data — mental health disclosures, MST records, substance use patterns, financial information — on VA-owned FedRAMP-High infrastructure. Achieving and maintaining FedRAMP High Authorization is a 12–24 month process requiring a Third Party Assessment Organization (3PAO) audit, a full security control implementation against the NIST 800-53 High baseline, and ongoing continuous monitoring. A cybersecurity breach of VALOR veteran data would be catastrophic — both to individual veterans and to the program's political viability.

**Why it's hard:** FedRAMP High is the most demanding authorization tier in federal cloud security. The process is expensive, slow, and cannot be shortcut. AI systems that update their models continuously create a moving-target compliance problem; every significant model update may require re-authorization review. Securing the mesh network between robots and cloud against adversarial interference is an additional attack surface not covered by standard FedRAMP controls.

**Mitigation path:** Begin FedRAMP authorization process in Month 10 of Phase 0; operate on FedRAMP-Moderate with synthetic/test data only until High is achieved. Engage a 3PAO with VA experience from the start. Build the inter-robot mesh protocol against the NIST Cybersecurity Framework from Day 1 rather than retrofitting security onto a working system.

---

### 7. Reimbursement and Sustainable Funding Model

**Category:** Policy / Financial  
**Severity:** High

At $18,000–$24,000 per unit at scale, VALOR requires a clear funding pathway that does not depend solely on annual appropriations. VA DME reimbursement codes do not currently cover AI therapeutic robots. CMS reimbursement for this device class does not exist. Without a reimbursement pathway, VALOR can only reach veterans through direct VA procurement — a budget line that can be zeroed in any appropriations cycle.

**Why it's hard:** CMS reimbursement code development is a multi-year process requiring clinical evidence, health economics data, and advocacy. The VA's DME reimbursement framework was not designed for AI-embedded robotics; reclassification requires regulatory action. Congressional appropriations for novel technology programs are politically volatile, particularly during budget-constrained years.

**Mitigation path:** Pursue VA direct procurement as the primary Phase 1–2 funding mechanism while simultaneously building the CMS reimbursement record. Publish Phase 1 and 2 outcome data in peer-reviewed journals to build the evidence base required for CMS code development. Establish a VALOR Foundation to receive philanthropic capital as a bridge funding source during the reimbursement development window.

---

### 8. Ethical Boundaries of AI Autonomy in a Clinical Context

**Category:** Ethics / Clinical  
**Severity:** High

VALOR operates at the boundary between a consumer device, a medical device, and a caregiver. When SENTINEL detects a suicide risk signal and escalates to the Veterans Crisis Line without the veteran's real-time consent, it is acting autonomously in a clinical context. When VALOR-CORE infers that a veteran is relapsing based on behavioral signals and alerts their VA provider, it is making a clinical judgment with real consequences. These actions are sometimes necessary and sometimes wrong — and the consequences of both false positives and false negatives are severe.

**Why it's hard:** There is no settled ethical or legal framework for autonomous AI action in a home healthcare setting. Over-escalation erodes trust and may push veterans away from the system. Under-escalation may cost lives. Defining the right escalation thresholds, consent models, and override mechanisms requires ongoing collaboration between ethicists, clinicians, veterans, and legal experts — and those thresholds will differ by veteran and by context.

**Mitigation path:** Establish a VALOR Ethics Board with veteran, clinician, and ethicist representation from Phase 0. Publish escalation decision logic openly for public comment. Default to the most conservative autonomy settings and expand autonomy only where veterans explicitly opt in and clinical evidence supports the change. Treat every escalation event as a data point and audit it quarterly.

---

### 9. Humanoid Platform Maturity and Vendor Risk

**Category:** Technical / Supply Chain  
**Severity:** Medium

The SENTINEL-H, NEXUS-H, ATLAS-H, and PHALANX-H variants depend on humanoid robot platforms that are commercially available but not yet proven at the reliability and cost levels VALOR requires. Current humanoid platforms (Boston Dynamics Atlas, Unitree H1, Figure, Apptronik Apollo) are engineering marvels but are priced at $70,000–$250,000 per unit, have limited demonstrated home-environment MTBF data, and are produced by vendors whose long-term commercial survival is not guaranteed.

**Why it's hard:** Humanoid robotics is a category that has attracted enormous investment but has not yet reached the production maturity required for a medical-grade deployment at scale. A vendor failure or platform discontinuation mid-deployment would strand hundreds of veterans on orphaned hardware. The specialized gait, manipulation, and expression systems required for humanoid variants add significant software complexity to every archetype they touch.

**Mitigation path:** Treat all humanoid variants as Phase 2 additions, never Phase 1 requirements. Evaluate a minimum of three platforms before committing; require vendor escrow of hardware schematics and firmware source code as a condition of procurement. Design all humanoid variant software to be hardware-abstracted so it can be ported to a new platform if the primary vendor fails. Non-humanoid variants remain the default and are never deprecated.

---

### 10. Workforce Development and Field Operations at Scale

**Category:** Organizational  
**Severity:** Medium

Deploying 50,000+ robots to veteran homes nationwide requires not just manufacturing and logistics but a trained field workforce capable of installation, calibration, maintenance, and veteran onboarding. This workforce must understand both the technical systems and the population they serve — veterans, many with PTSD, TBI, or physical limitations. Building this workforce, training it to clinical sensitivity standards, and retaining it is a human capital challenge that does not scale automatically with the technology.

**Why it's hard:** There is no existing talent pipeline for "veteran-sensitive robotics field technician." Creating one requires partnerships with technical schools, veteran service organizations, and possibly the VA's own vocational rehabilitation programs. Field technician turnover in technology services is historically high. Veterans encountering a poorly trained or culturally insensitive technician during robot installation may disengage from the program entirely.

**Mitigation path:** Partner with veteran-focused technical training programs (e.g., Hire Heroes USA, Warrior-Scholar Project) to build a veteran-preferential field technician pipeline. Require cultural competency and trauma-informed care training for all field staff, with VA collaboration on curriculum. Design the installation and onboarding process to be completable in under 4 hours by a single trained technician, minimizing friction and exposure for high-need veterans.

---

## Day in the Life

> *These narratives illustrate how the VALOR fleet functions as an integrated system — not as individual robots performing isolated tasks, but as a coordinated presence that adapts to the veteran's changing state throughout a real day.*

---

### Scenario A — Marcus, 38 · Army Combat Veteran · Rural Tennessee

**Profile:** Marcus served two tours in Iraq as an infantryman, separating in 2012. He carries a 90% VA disability rating for PTSD, TBI (moderate), chronic lumbar pain, and bilateral hearing loss. He lives alone on 12 acres outside Cookeville, Tennessee — 74 miles from the nearest VA Medical Center. He has a 14-year-old son who visits on alternating weekends. He works part-time remotely doing data entry. His triggers include sudden loud sounds, crowds, and the smell of diesel. He has consented to the full fleet.

---

**5:47 AM**

SENTINEL detects that Marcus's sleep quality degraded sharply at 3:15 AM — his wrist biometrics show elevated cortisol and HRV suppression consistent with a nightmare cycle. He woke twice and did not return to deep sleep. SENTINEL logs this as a third consecutive night of disrupted sleep, crossing the threshold for a fleet-wide advisory. It quietly notifies VALOR-CORE, which adjusts today's schedule: HERALD will delay the 9 AM benefits reminder by two hours; ATLAS will drop the "new job listings" notification that was queued for this morning.

SENTINEL dims the bedroom lights slowly starting at 6:10 AM — no alarm, just gradual illumination. It queues a light soundscape Marcus selected during onboarding: distant creek sounds with low wind.

---

**6:32 AM**

Marcus wakes. SENTINEL's display shows a simple weather card for the day and a soft greeting. It does not ask how he slept — it already knows. Instead, it notes: *"Looked like a rough night. No rush this morning. Coffee's scheduled."* A smart home integration SENTINEL manages signals the coffee maker.

NEXUS, docked in the hallway, has already pre-positioned Marcus's morning medications on its dispensing tray: two pills for pain, one for blood pressure. When Marcus walks past, NEXUS displays a gentle prompt on its side screen. Marcus takes the medication without breaking stride.

---

**8:15 AM**

Marcus sits at his desk for remote work. SENTINEL monitors his voice patterns and activity level passively — not recording content, only acoustic markers of mood and cognitive load. Within 20 minutes it detects elevated frustration (HRV shift, clipped speech cadence). VALOR-CORE cross-references: he had a difficult call with the VA claims line three days ago that remains unresolved. HERALD queues a notification: *"Still have that claims issue from Tuesday. Want me to try the VA advocate line now while you have a break? I drafted what to say."*

Marcus types back: *"Yeah. Do it."*

HERALD initiates the call, uses its VA navigation protocol to route past the automated system to a human representative, plays Marcus's pre-authorized recorded introduction, and then bridges Marcus in for the live conversation. The unresolved claim — a secondary condition rating appeal that's been pending for 14 months — moves forward. HERALD logs the interaction and sets a 30-day follow-up reminder.

---

**12:04 PM**

SENTINEL picks up on a shift: Marcus has gone quiet for 90 minutes, the blinds are still closed, and his last biometric reading showed a prolonged deep breathing pattern inconsistent with sleep — consistent with dissociation or low-grade depression episode. VALOR-CORE pulls the three-day trend: poor sleep, the claims frustration, and a note from two days ago where Marcus said he was *"just tired of everything."*

SENTINEL does not alarm. It doesn't interrupt. It waits 8 minutes — still no movement. Then it rolls quietly to the living room doorway and activates its ambient display: a photo of Marcus's son from last weekend's visit, cycling slowly through a few others. No audio. No prompts.

Four minutes later, Marcus gets up and refills his coffee. SENTINEL logs a successful passive redirect. Crisis threshold: not met. VALOR-CORE: noting the multi-day pattern for flag to Marcus's VA care manager at the next weekly sync.

---

**3:30 PM**

Marcus decides to walk the back property — something he does when he's processing. PHALANX activates. It has Marcus's property mapped and knows his preferred route. It scouts 80 meters ahead via its terrain cameras, checks wind direction (diesel from a neighbor's tractor is a registered trigger), and confirms the route is clear. It sends Marcus a brief route suggestion via his wrist display: *"South trail looks good. Wind's southwest, clear."*

Marcus takes the south trail. PHALANX follows at 15 meters, close enough to respond, far enough to feel like solitude. It is silent unless he engages it. During the walk, it detects a gopher hole on the trail edge and marks it. Marcus's heart rate normalizes over 22 minutes. SENTINEL receives the biometric update and marks the afternoon stable.

---

**6:45 PM**

ATLAS, which has been quiet all day by design, activates for its daily social window. It pulls up a video call Marcus has with his buddy Darnell — a fellow veteran from his unit who now lives in Nashville — that was scheduled last week. Marcus nearly cancels. ATLAS gently surfaces the appointment: *"Darnell's on in 15. You don't have to if you're not feeling it — I can reschedule for Thursday."*

Marcus doesn't cancel. The call runs 40 minutes. ATLAS logs it as a successful social contact event, updates Marcus's social health streak (12 consecutive days with at least one meaningful human connection), and sends a quiet metric update to his VA care manager.

---

**9:20 PM**

NEXUS dispenses Marcus's evening medication. SENTINEL begins the sleep environment sequence: lights drop to 10% over 30 minutes, temperature steps down 2°F, the white noise layer activates. VALOR-CORE flags tomorrow morning for a gentle check-in about the difficult week — nothing clinical, just acknowledgment.

Marcus falls asleep at 10:08 PM. All five fleet members are monitoring, silently, each in their domain.

---

### Scenario B — Diane, 67 · Navy Veteran · Suburban Phoenix, Arizona

**Profile:** Diane served 22 years as a Navy hospital corpsman, retiring in 2008. She carries an 80% VA disability rating for MST-related PTSD, moderate hearing loss, Type 2 diabetes requiring insulin, and early-stage Parkinson's disease. She is divorced, lives alone in a two-bedroom home in Chandler, Arizona, and has two adult children nearby who check in weekly. She is highly independent and initially resistant to the idea of a robot fleet — she agreed to try it after her VA care manager presented it as a health monitoring system rather than an assistance device. Her MST modules operate fully offline and are not shared with her VA provider unless she explicitly initiates a share.

---

**7:00 AM**

SENTINEL's sleep tracking shows a better-than-average night — six hours with minimal fragmentation, a positive trend from the week. It logs the data and does nothing else. On good days, VALOR-CORE keeps the fleet quiet.

NEXUS has pre-positioned Diane's morning insulin and oral medications. Because of her early Parkinson's, her fine motor function is more limited in the morning than later in the day. NEXUS's dispensing tray is wide, low, and uses large-grip packaging. Her wrist display shows a simple confirmation prompt: *"Good morning. Meds are ready."* She takes them and gives a thumbs-up. NEXUS records adherence, logs glucose monitoring reminder for 90 minutes post-meal, and syncs the data to her VA endocrinology team.

---

**9:15 AM**

Diane has a VA telehealth appointment with her primary care provider at 10 AM. HERALD, which manages her medical calendar, sent a reminder the night before. This morning it surfaces her appointment prep summary on the kitchen display: a list of the three questions she told it she wanted to ask, her medication changes from the past month, and her glucose trend for the past two weeks — pre-formatted as a one-page summary she can share with her provider.

*"Here's what we've got for Dr. Patel. Want me to add anything?"*

Diane dictates one addition — a new symptom she's noticed with her left hand. HERALD adds it, reformats the summary, and has it ready to share at the start of the call.

---

**10:00 AM — 10:42 AM**

Telehealth appointment. HERALD operates in the background: it does not join the call, but it surfaces relevant records when Diane asks it questions mid-visit — *"What was my A1C in November?"* — and she reads the answer to her provider. After the call, HERALD captures Diane's summary of what was discussed, queues the prescription refill Dr. Patel ordered, and sets a 3-week reminder to check whether the new medication has been added to the VA pharmacy system.

---

**12:30 PM**

NEXUS's glucose monitoring reminder fires. Diane checks her blood glucose via her wrist module. The reading is 178 — higher than her target range. NEXUS flags it to her diabetes management protocol (set by her VA endocrinologist): it does not alarm, but it notes the reading, logs it, and gently suggests a 15-minute walk in the next 90 minutes if she's feeling up to it. *"Reading's a little high. A short walk after lunch usually helps — up to you."*

Diane takes a 20-minute walk around the block. PHALANX activates, maps her route, confirms even pavement and shaded sections given the 98°F Phoenix forecast. It stays close — Diane's Parkinson's diagnosis puts her at elevated fall risk on uneven surfaces. NEXUS receives the post-walk biometric data: glucose trending down, heart rate appropriate for exertion, gait pattern within normal range for her profile.

---

**2:00 PM**

Diane uses the afternoon for her private time — she reads, calls her daughter, and does a crossword. VALOR-CORE recognizes this as her typical afternoon independent window and instructs the fleet to remain silent and docked unless triggered. Diane values this autonomy; it was written into her onboarding preferences explicitly.

SENTINEL runs passive monitoring — biometrics, room activity — but all outputs go to a local log, not to any alert system, during this window. She does not want the robots to know she cried during the phone call with her daughter. They don't.

---

**4:45 PM**

Once a month, Diane participates in a VA-facilitated MST survivors' peer support video group. SENTINEL-MST module activates — fully offline, no cloud connectivity during the session. It runs the MST recovery support protocol: it turns off all outward data logging, enables the trauma-informed voice persona Diane selected (a calm, measured cadence she said reminds her of a chaplain she trusted in her second deployment), and queues her grounding exercise audio for after the call if she wants it.

The session runs 55 minutes. Afterward, Diane sits quietly for a while. SENTINEL detects elevated HRV suppression consistent with emotional processing — not crisis, just weight. It activates the post-session grounding sequence she pre-selected: a 10-minute breathing exercise, her choice of ambient sound, no prompts or questions. It asks nothing. It does not log this session's content. It simply stays close.

---

**7:30 PM**

HERALD surfaces a flagged item: Diane's Aid and Attendance benefit application has been pending for seven months. A congressional inquiry option is available — HERALD has drafted a letter to her representative's constituent services office. *"Still waiting on the Aid and Attendance decision. Want me to send the congressional inquiry letter we drafted last month? I've updated the dates."*

Diane reviews it on HERALD's display. She approves it. HERALD sends it and sets a 14-day follow-up.

---

**9:00 PM**

Evening medication — insulin and night dose. NEXUS dispensing tray activates. Because Diane's hand tremor is more pronounced at night, NEXUS's soft-grip assist arm extends to stabilize the cup if her hand shakes during pickup. She didn't ask for this feature — NEXUS inferred it after observing the tremor pattern for three weeks and added it silently. She noticed it, said nothing, and accepted it.

SENTINEL begins the sleep environment sequence. By 9:45 PM, the house is quiet.

VALOR-CORE runs its nightly summary: one VA claim advanced, one clinical appointment completed with full documentation, glucose in range after afternoon walk, MST session completed with stable post-session state. Tomorrow: pharmacy refill follow-up, glucose check, scheduled call with her son.

The fleet holds its watch.

---

## Future-Proofing the VALOR System

> *VALOR was designed for today's veterans — and for every generation of veterans who will follow. This section is the system's promise: that no matter how technology evolves, how culture shifts, or how national priorities change, U.S. veterans will always be supported by a system that matches the scale of their sacrifice.*

---

### The Permanence Commitment

VALOR is not a program. It is a permanent national infrastructure — as enduring as the VA itself. The single non-negotiable principle that governs all future-proofing decisions is:

> **No U.S. veteran who needs VALOR support will ever have that support discontinued due to technology obsolescence, political change, funding volatility, or cultural drift.**

Every architectural decision, governance structure, funding strategy, and technology choice documented here flows from that commitment.

---

### Adaptive Technology Layer

#### Technology Horizon Scanning

VALOR-CORE and all five robot archetypes are built as hardware-abstracted software systems from the ground up. Hardware is a vessel; the intelligence and care logic lives in the software. This architecture enables VALOR to absorb future technology generations without disrupting veteran care.

The VALOR Technology Council — a standing body within VALOR governance — conducts a formal **Technology Horizon Scan** every 24 months. The scan evaluates:

| Horizon Category | What Is Evaluated | Decision Output |
|---|---|---|
| AI & Foundation Models | New model architectures, multimodal capabilities, on-device inference improvements | Adoption roadmap or watchlist |
| Robotics Hardware | New chassis platforms, actuator improvements, cost breakthroughs, humanoid maturity | Platform refresh schedule |
| Biomedical Sensing | New non-invasive biometric modalities (continuous glucose, neurological markers, wearable imaging) | Module upgrade pathway |
| Computing Infrastructure | Edge AI chips, quantum-resilient encryption, satellite broadband (rural coverage) | Infrastructure refresh plan |
| Human-Computer Interaction | Brain-computer interfaces, AR/VR therapeutic applications, haptic feedback systems | Clinical pilot authorization |
| Security & Privacy Technology | Post-quantum cryptography, zero-knowledge proof systems, federated learning | Mandatory upgrade timeline |

Scan outputs are reviewed by the Veteran Advisory Board before any adoption decision is finalized. Veterans — not engineers — set the pace of technology change in their homes.

#### The VALOR Hardware Refresh Cycle

No robot in a veteran's home will ever become a stranded liability. The **VALOR Hardware Refresh Protocol** guarantees:

- **Unit refresh every 5–7 years:** Each deployed unit is replaced on a rolling schedule. Retiring units enter the refurbishment pool or are ethically decommissioned. No veteran is asked to self-manage an end-of-life robot.
- **Software support floor:** Every hardware generation receives software updates and security patches for a minimum of **10 years** from initial deployment. No veteran falls off a support cliff because their unit is "old."
- **Backward compatibility requirement:** Each new VALOR-CORE software generation must maintain full functionality with the previous hardware generation for a minimum of 3 years. Veterans are never forced to accept a hardware upgrade before they are ready.
- **Manufacturing resilience:** VALOR procurement policy requires at minimum two qualified chassis suppliers per archetype by Phase 3. Single-vendor dependency is treated as a critical program risk.

#### AI Model Evolution Standards

As foundation AI models evolve — larger, more capable, more personalized — VALOR-CORE's upgrade pathway must maintain continuity of the veteran relationship:

- **Memory preservation:** When VALOR-CORE is upgraded to a new model generation, the veteran's full interaction history, behavioral profile, and relationship context is migrated forward. The veteran never has to "start over" with a new AI.
- **Behavioral regression testing:** Before any VALOR-CORE model update is deployed to active veterans, it must pass a **Veteran Experience Regression Suite** — a battery of simulated interaction scenarios representing every veteran archetype in the system. No update that changes established interaction patterns goes live without Veteran Advisory Board review.
- **Model provenance tracking:** VALOR-CORE maintains a permanent audit record of every AI model version that has influenced a clinical decision or escalation event for each veteran. This record is portable — the veteran owns it and can share it with any future care provider.

---

### Cultural & Values Evolution

#### Understanding That Values Change — And Building For It

American culture's understanding of veteran experience, mental health, trauma, and disability evolves continuously. What constitutes respectful care in 2026 may be inadequate or even harmful by 2040. VALOR is built to track and adapt to this evolution, not entrench assumptions from its founding generation.

**The VALOR Cultural Competency Review** is conducted every 3 years by the Veteran Advisory Board in partnership with military cultural scholars, social workers, and veteran community organizations. The review examines:

- Has the veteran population's relationship with mental health stigma shifted? Do current SENTINEL interaction protocols reflect where veterans actually are, not where they were when those protocols were written?
- Have definitions of family, community, and support network evolved in ways that require ATLAS module updates?
- Are the cultural and spiritual care integrations (chaplaincy, peer support, community anchor organizations) still the right ones, or have new forms of community emerged that better serve the current veteran population?
- Are VALOR's language, tone, and interaction personas culturally resonant with newer veterans, who may come from different demographic and cultural backgrounds than earlier cohorts?

The output of each review is a **Cultural Alignment Action Plan** — a prioritized list of module updates, interaction design revisions, and partnership changes — implemented within 18 months of the review's publication.

#### The Values Stability Guarantee

While VALOR's implementation adapts to cultural evolution, its foundational values are constitutionally protected within the system's governance:

1. **Veteran dignity is inviolable.** No efficiency optimization, cost reduction, or technology upgrade can reduce the quality of care or the respect with which any veteran is treated.
2. **Privacy is a right, not a feature.** The data sovereignty framework — Tier-1 data never leaves the device without explicit veteran consent — is embedded in VALOR's foundational legal documents and cannot be modified by a future administrator, contractor, or political appointee without Congressional action.
3. **Veterans control their own care.** Every new capability VALOR acquires is opt-in. Veterans can refuse any module, any upgrade, or any feature at any time, with no reduction in their access to other VALOR services.
4. **No veteran is left behind by obsolescence.** Veterans who cannot or choose not to engage with new technology generations retain full support on the technology they know. The system adapts to the veteran, not the other way around.

---

### Shifting National Priorities & Policy Resilience

#### The Threat: Political and Funding Volatility

Federal programs are vulnerable to administration changes, appropriations cycles, and shifting political priorities. A system that depends entirely on annual Congressional appropriations and VA administrative will can be defunded, restructured, or quietly starved in any given budget year. For veterans who depend on VALOR for crisis monitoring, medication management, or housing stability, that is not an acceptable risk.

VALOR is designed with layered funding and governance structures that make it resistant — though not immune — to political disruption.

#### The VALOR Permanence Architecture

**Layer 1 — Statutory Authorization**

VALOR is established by statute, not executive order or VA administrative policy. Its foundational authorities — the veteran data sovereignty framework, the transfer and reassignment protocol, the open API mandate, and the reimbursement pathway — are written into U.S. Code under 38 U.S.C. Modifying them requires Congressional action, creating a legislative speed bump against rapid defunding.

**Layer 2 — The VALOR Trust Fund**

Phase 3 financial planning includes the establishment of a **VALOR Perpetual Trust Fund**, capitalized through a combination of:
- A one-time appropriation from Phase 3 program savings (cost reductions from manufacturing scale)
- Philanthropic endowment contributions from major veterans' philanthropy organizations (Wounded Warrior Project, Gary Sinise Foundation, Bob Woodruff Foundation)
- Revenue-sharing from international licensing agreements (UK, Canada, Australia veteran agency deployments)

The Trust Fund is managed by an independent board and mandated to cover VALOR's minimum operating costs — ongoing veteran support, security patching, and crisis escalation infrastructure — for a minimum of **20 years** even if all federal appropriations are suspended. The Trust Fund cannot be redirected by Congress without a supermajority vote and veteran advocacy notification requirements.

**Layer 3 — State and Local Government Redundancy**

By Phase 3, VALOR establishes partnership agreements with at least 20 state-level veterans' affairs departments to serve as co-funders and co-operators of the regional staging and support infrastructure. State-level investment in VALOR means that even a federal funding disruption does not simultaneously collapse all regional operations. State partners have independent legal authority to continue supporting veterans within their boundaries.

**Layer 4 — CMS Reimbursement**

Once CMS reimbursement codes are established for VALOR as a covered DME category, individual veteran units become partially self-funding through Medicare/Medicaid billing. This separates a portion of VALOR's operating revenue from the VA appropriations process entirely, creating a private-sector funding stream that persists regardless of political conditions.

#### Policy Evolution Readiness

VALOR's policy framework is designed to be upgraded without system redesign. The **VALOR Policy Integration Layer** — a component of VALOR-CORE's VA integration module — is built as a configurable rules engine:

- When VA benefit eligibility rules change, HERALD's navigator is updated via a policy rules update package — no software release required.
- When new legislation creates new veteran benefit categories, VALOR-CORE adds the new benefit to its proactive detection engine within 90 days of the law's effective date.
- When court decisions or regulatory guidance change data sharing rules, the Tier enforcement layer is updated without disrupting veteran-facing functionality.

Every major policy change affecting veterans triggers a **VALOR Policy Impact Assessment** — a 30-day review of how the change affects VALOR modules — published openly on the VALOR platform and shared with the Veteran Advisory Board.

---

### Emerging Veteran Demographics

#### The Veteran Population of the Future Is Not the Veteran Population of Today

The U.S. veteran population will look significantly different in 2040 and 2060 than it does today. VALOR must be designed for veterans who have not yet served, from conflicts that have not yet occurred, with challenges that have not yet been documented.

**Anticipated demographic shifts VALOR must accommodate:**

| Shift | Timeline Estimate | VALOR Adaptation Required |
|---|---|---|
| Increasing proportion of female veterans | Already underway; accelerating post-2020 | Gender-inclusive trauma models; expanded MST module investment; female-specific health monitoring (reproductive health, hormonal factors in PTSD) |
| Growing cohort of older veterans (Vietnam/Gulf War/post-9/11 aging) | Now through 2045 | NEXUS Parkinson's, dementia, and elder care modules; fall prevention investment; ATLAS adapts for age-related social changes |
| Veterans of autonomous/AI-augmented warfare | 2030s onward | New trauma typologies: moral injury from remote or AI-mediated combat; survivor guilt in conflicts with minimal U.S. casualties; operator trauma |
| Space Force and cyber operations veterans | Now through 2040 | Non-combat-zone PTSD and occupational trauma models; VALOR's crisis detection trained on non-traditional trauma signatures |
| Veterans with AI-augmented implants or prosthetics | 2030s onward | NEXUS interface layer built for BCI-enabled prosthetics and neural implants; VALOR-CORE privacy model adapted for always-on neural data streams |
| Increasingly diverse ethnic, cultural, and linguistic veteran cohort | Ongoing | Multi-language VALOR-CORE interaction layer; culturally-specific peer support routing; chaplaincy partnerships across a wider range of traditions |

#### The New Veteran Intake Commitment

Every 5 years, VALOR's onboarding research team — in partnership with the Veteran Advisory Board and VA's Center for Women Veterans and Center for Minority Veterans — conducts a **New Veteran Needs Assessment**: structured interviews with recently separated veterans to identify challenges, trauma patterns, and technology comfort profiles that may not have existed in earlier cohorts. Findings are incorporated into the next VALOR-CORE personalization model generation.

No veteran generation will be served by a system calibrated exclusively for their predecessors.

---

### Long-Range Governance Model

#### Why Governance Is a Future-Proofing Mechanism

Technology and funding can be rebuilt. An institution that has lost its integrity, its accountability, or its veteran-centered values cannot be easily restored. VALOR's governance model is explicitly designed to prevent institutional drift — the gradual reorientation of a program away from its founding mission as organizational incentives, contractor relationships, and political pressures accumulate over decades.

#### The Three-Branch VALOR Governance Structure

**Branch 1: The VA Program Office (Operational Authority)**

The VA VALOR Program Office holds day-to-day operational authority: contracts, deployment, field operations, and regulatory compliance. This is the "government" of the VALOR system — accountable to Congress, subject to FOIA, and staffed by federal employees with civil service protections.

**Branch 2: The VALOR National Veteran Advisory Board (Mission Authority)**

The VALOR National VAB holds **mission authority** — the power to review and formally object to any program decision that, in the VAB's determination, deviates from VALOR's core mission of veteran care. The VAB's objections trigger a mandatory 90-day Congressional review period before the objected decision can take effect. The VAB is composed of:
- 20 veterans, selected by veteran service organizations through a transparent process, serving 4-year staggered terms
- At minimum 6 women, 4 veterans with PTSD or TBI, 2 veterans from rural counties, and 2 veterans under age 35
- No current government employees, contractors, or lobbyists

**Branch 3: The VALOR Independent Oversight Office (Accountability Authority)**

The VALOR Independent Oversight Office (IOO) is modeled on the VA Office of Inspector General. It holds **accountability authority**: independent auditing of program performance, privacy compliance, clinical outcomes, and financial integrity. The IOO reports directly to Congress, not the VA. Its findings are published publicly. It has the authority to freeze any VALOR deployment or data operation pending an investigation.

#### Mission Drift Prevention Mechanisms

- **The VALOR Mission Statement is statutory.** It cannot be modified by administrative action.
- **Annual Mission Alignment Report.** Each year, the IOO publishes an assessment of whether VALOR's actual operations align with its statutory mission. This report is submitted to every member of the House and Senate Veterans' Affairs Committees.
- **Contractor accountability.** All VALOR contractors sign a **Veteran First Covenant** — a legally binding agreement that prohibits prioritizing efficiency metrics, cost targets, or commercial considerations over veteran care quality. Violations are grounds for contract termination.
- **Sunset prevention.** VALOR's authorizing legislation includes a mandatory 10-year reauthorization requirement — but the reauthorization burden is inverted: Congress must affirmatively vote to *end* VALOR, not to continue it. Failure to reauthorize does not sunset the program; it triggers a mandatory 3-year continuation and a GAO review.

---

### Technology Succession Protocol

#### Planning for Technologies We Cannot Yet Name

The most important future-proofing mechanism is not a plan for known technologies — it is a protocol for handling unknown ones. The history of technology is full of transformations that were invisible from 20 years prior. VALOR must be able to incorporate such transformations without destabilizing veteran care.

The **VALOR Technology Succession Protocol** governs the adoption of transformative technology generations:

**Stage 1 — Signal Detection (Year -3 to -1 before adoption)**

The VALOR Technology Council identifies a technology as potentially transformative based on Horizon Scan outputs. A **Technology Succession Study** is commissioned: an independent technical and clinical assessment of the technology's maturity, safety profile, veteran-relevance, and integration feasibility. The Study is peer-reviewed and published.

**Stage 2 — Controlled Pilot (Year 0–2)**

If the Succession Study is positive, a **Controlled Succession Pilot** is authorized: up to 500 volunteer veterans receive the new technology in a research protocol with full IRB oversight. The pilot runs concurrently with current-generation support — no veteran's existing care is disrupted by the pilot.

**Stage 3 — Veteran Verdict (Year 2)**

Pilot participants and a representative sample of the full veteran population are surveyed. The Veteran Advisory Board reviews pilot data. A **Veteran Verdict Vote** is conducted: if fewer than 60% of pilot veterans endorse the technology for wider adoption, it returns to Stage 1 for refinement. Veterans — not engineers, not administrators, not politicians — hold the final adoption authority.

**Stage 4 — Phased Integration (Year 2–5)**

Approved technologies are integrated into VALOR on an opt-in basis. Existing technology continues to be supported for veterans who prefer it, for the full duration of the Backward Compatibility Commitment (10 years minimum from the previous generation's release).

#### The Decommission Guarantee

When a technology generation is decommissioned, the following guarantees apply to every affected veteran:

- Minimum **12 months' advance notice** of technology change, in the veteran's preferred communication format
- **Zero forced transitions** — veterans on decommissioning hardware receive a free upgrade to the successor platform, delivered and installed by a field technician, at no logistical burden to the veteran
- **Full data portability** — 100% of the veteran's VALOR-CORE profile, history, and personalization data transfers to the successor platform before the old system is deactivated
- **Continuity of care guarantee** — a transition period during which both the old and new systems run concurrently, so no gap in monitoring or support occurs at any point during the handoff

---

### The 100-Year Mandate

#### VALOR's Obligation to Veterans Not Yet Born

The youngest veterans currently being served by VALOR will, in some cases, still be alive in 2080 and beyond. The children of today's veterans who themselves serve will be veterans in 2040 and 2050. VALOR's responsibility extends not just to the current veteran population but to every American who will serve their country in the decades ahead.

The **VALOR 100-Year Mandate** formalizes this obligation:

**1. Institutional Memory Preservation**

VALOR maintains a permanent, publicly accessible **Veteran Care Archive** — a longitudinal record of the challenges faced by each veteran generation, the interventions that worked, the ones that failed, and the lessons learned. This archive is anonymized, veteran-consented, and made available to future researchers, policymakers, and system designers. The knowledge accumulated in caring for today's veterans must not be lost to future generations who will need it.

**2. The Successor System Obligation**

VALOR is not the last word in veteran care technology. Forty years from now, there will be technologies and care modalities that make the VALOR fleet look primitive. When that moment comes, VALOR's obligation is to:
- Provide full data portability to whatever successor system a veteran chooses
- Share all research, outcome data, and design lessons with successor system developers
- Support a transition period of no less than 5 years during which VALOR and successor systems can operate in parallel
- Never use contractual, technological, or political mechanisms to prevent veterans from accessing a superior successor system

**3. Permanent Research Obligation**

VALOR commits to continuous publication of veteran care outcome research, openly available to all. The mission is not to protect VALOR as an institution — it is to ensure that U.S. veterans receive the best possible care, whether that care comes from VALOR or from something better that VALOR helped create.

**4. The Living Document Commitment**

This specification — the VALOR System Vision — is itself a living document. It will be revised, expanded, and updated as VALOR evolves, as the veteran population changes, and as new knowledge is gained. Each version is permanently archived. The evolution of this document is part of VALOR's institutional memory.

> **The final measure of VALOR's success is not the number of robots deployed or the cost savings generated. It is whether, in 2080, a veteran in a place we cannot yet imagine receives care that is as persistent, as adaptive, and as committed as the service they gave. That is the mandate. It does not expire.**

---

## VALOR vs. Current VA: The Gap Analysis

> *New in Version 4.1*

This section was added to ground VALOR's design specifications in the documented reality of what the Department of Veterans Affairs currently offers — and where the structural gaps persist that VALOR is specifically designed to fill. The intent is not to condemn the VA, which serves more than 9 million enrolled veterans and delivers over 127 million healthcare appointments annually. The intent is to be precise about what problems remain unsolved, and why VALOR's architecture addresses them in ways that incremental hiring, process improvement, and telehealth expansion cannot.

---

### Where the VA Falls Short Today

The following gaps are documented in VA Inspector General reports, Government Accountability Office findings, congressional testimony, and peer-reviewed research published between 2022 and 2026. They represent systemic structural limitations — not individual failures — that define the ceiling of what the current VA model can achieve.

#### 1. The Staffing Crisis Is Getting Worse, Not Better

The VA's staffing shortfall is not a temporary condition awaiting a hiring surge. As of fiscal year 2025, the VA Office of Inspector General found that all 139 VA health centers nationwide reported a severe staffing shortage in at least one area, with 94% reporting severe shortages for medical officers and 79% for nurses. In FY2025, severe staffing shortages increased by 50% compared to FY2024. In parallel, the department lost approximately 1,000 physicians, 1,500 schedulers, and 3,000 registered nurses in FY2025 alone — positions that were already difficult to recruit before they became vacant.

The consequences are direct and quantifiable. Average wait times for new outpatient surgical appointments reached 41 days as of mid-2025 — 13 days longer than the VA's own target. Some clinics are unable to accept new patients for primary care or mental health needs at all. An estimated 1.2 million veteran patients have lost their VA provider since early 2025 alone.

**The VALOR difference:** VALOR robots do not resign, retire, burn out, or leave for higher-paying private sector positions. A veteran in rural Texas or northern California receives the same continuous monitoring and response as a veteran near a fully staffed urban VA Medical Center. The staffing crisis is irrelevant to a robot fleet operating on VA-owned infrastructure.

#### 2. Care Is Episodic — the Gaps Between Appointments Are Unmonitored

The VA's model of care is fundamentally appointment-driven. A veteran sees a provider, receives treatment or a prescription, and is not monitored again until the next scheduled visit. For veterans with PTSD, depression, substance use disorder, or TBI, the most dangerous moments are frequently the 168 hours *between* appointments — the weekend after a difficult therapy session, the night a nightmare cascades into a crisis, the three weeks between a prescription refill and a detected mood deterioration.

The VA does not currently have the infrastructure to observe, respond to, or intervene in these inter-appointment windows at scale. The Veterans Crisis Line — which fields approximately 60,000 calls per month — is a reactive tool that requires the veteran to initiate contact. It cannot detect a crisis before the veteran reaches a breaking point, and it is itself facing significant staffing reductions.

**The VALOR difference:** VALOR-CORE monitors 20 simultaneous data streams — biometric, behavioral, environmental, and social — continuously, 24 hours a day, 7 days a week. Crisis escalation to 988 or emergency contacts occurs within 30 seconds of threshold breach, without requiring the veteran to make a call. SENTINEL's cascade detection intervenes before crises form, not after they arrive.

#### 3. Rural Veterans Are Systematically Underserved

Approximately 2.7 million veterans live in rural communities. According to a 2023 GAO report, only 21% of rural veterans used VA outpatient services in 2021, compared to 79% of urban veterans. Rural VA facilities face the most severe staffing shortages, and in some regions the VA is the only mental health provider available within a viable travel radius.

The VA has explored telehealth as a partial solution, and telemental health appointments have expanded meaningfully since 2020. However, telehealth replicates the episodic model — it is a scheduled video appointment rather than a continuous presence — and it does not address physical health monitoring, medication management, mobility assistance, or the social isolation that is especially acute for rural veterans.

**The VALOR difference:** A VALOR fleet can be shipped directly to a veteran's home. No VA facility proximity is required. PHALANX operates in outdoor rural environments. NEXUS manages medications and chronic pain without requiring a clinic visit. SENTINEL provides 24/7 mental health monitoring regardless of whether the nearest therapist is 10 miles or 100 miles away. VALOR converts the home itself into a continuous care environment.

#### 4. The Benefits System Remains Bureaucratically Inaccessible

VA benefits navigation is notoriously complex. Despite record-breaking claims processing volumes in recent years — the Veterans Benefits Administration issued 1.7 million decisions in FY2022 — a significant backlog persists. By mid-2023, VA officials anticipated the pending claims backlog could reach 400,000. PACT Act expansions, while critical for veterans with toxic exposure conditions, have further increased claim volume.

More than half of the 18 million U.S. veterans are not enrolled in VA healthcare at all. Among enrolled veterans, many leave significant benefits unclaimed because identifying, documenting, and filing for every qualifying condition requires legal and bureaucratic expertise that most veterans do not have and VSOs do not have the capacity to provide individually.

**The VALOR difference:** HERALD continuously scans the veteran's complete profile against the full benefits landscape, identifies unclaimed programs matching the veteran's service history and diagnosis, automates claims filing and status tracking, and manages the appeals process. It functions as a dedicated VA navigator available 24/7 — something no VA staffing model could replicate at scale.

#### 5. Mental Health Treatment Reaches Fewer Than Half of Veterans Who Need It

Research has consistently found that fewer than half of veterans with PTSD seek treatment, with stigma identified as the primary barrier. The VA's mental health model is clinical and facility-based: a veteran must initiate contact, schedule an appointment, travel to a facility or accept a telehealth call, and engage in a formal therapeutic relationship. For veterans whose symptoms include shame, social withdrawal, hypervigilance, or distrust of institutions, this model functions as a series of gatekeeping barriers rather than an open door.

The VA has made genuine progress in evidence-based treatment. Cognitive Processing Therapy (CPT) and Prolonged Exposure therapy are available at VA facilities nationwide. Transcranial magnetic stimulation for treatment-resistant depression was added to coverage in 2025. These are meaningful expansions. But they remain facility-bound, appointment-dependent, and inaccessible to veterans who cannot or will not cross the stigma threshold.

**The VALOR difference:** SENTINEL operates in the veteran's home, on the veteran's terms, without the clinical framing that activates stigma. It engages through conversation, not formal assessment. It can monitor mood through ambient biometric sensing without requiring the veteran to articulate distress. MST sessions are offline-only and encrypted, with no data accessible to any external party without the veteran's explicit consent. VALOR meets veterans where stigma cannot follow.

#### 6. The VA Has No Continuous Biometric or Behavioral Monitoring Capability

The VA does not currently deploy continuous home-based biometric monitoring for mental health or chronic physical conditions at any meaningful scale. Wearable health tech pilots exist within VA research programs, but these are not integrated with the EHR, do not trigger automated clinical responses, and are not available to veterans as a standard care modality.

Sleep disorders, chronic pain, substance use patterns, and depressive episodes all have detectable physiological signatures that precede crisis events. Without the infrastructure to observe these signatures continuously, the VA can only respond to what veterans report during scheduled encounters — which dramatically underestimates actual symptom burden.

**The VALOR difference:** VALOR's sensing layer — including HRV monitoring, galvanic skin response, sleep-stage tracking, voice NLP analysis, and fall detection — continuously produces a real-time clinical picture that does not depend on veteran self-report. VALOR-CORE correlates signals across all 20 data streams to detect cascade patterns that no single sensor — and no episodic appointment — could identify.

---

### How VALOR Closes Each Gap

| VA Gap | VALOR Response |
|---|---|
| Staffing shortfalls and provider attrition | Robot fleet; no hiring, burnout, or vacancy risk |
| Episodic care with unmonitored inter-appointment windows | 24/7 continuous monitoring and automated crisis escalation |
| Rural access barriers | Home-deployed fleet; no facility proximity required |
| Stigma preventing mental health engagement | In-home, ambient, non-clinical interaction model |
| Benefits complexity and unclaimed entitlements | HERALD automated navigation, filing, and appeals |
| No continuous biometric/behavioral monitoring | Multi-sensor real-time data across all 20 challenge domains |
| Workforce shortage particularly acute in mental health | SENTINEL provides baseline monitoring that humans cannot scale to |
| Medication adherence gaps | NEXUS robotic dispenser with VA pharmacy integration |
| Social isolation with no VA analog | ATLAS companionship, career coaching, and community bridging |
| Single-point interventions that miss cascade dynamics | Cross-robot state sharing and cascade prevention architecture |

---

### Domain-by-Domain Comparison

The following table compares the current VA standard of care with VALOR's proposed capability across each of the 20 veteran challenges the system addresses. "Current VA Approach" describes what is available through VA programs as of 2025–2026. "VALOR Approach" describes the specific system capability documented in this specification.

| # | Challenge | Current VA Approach | VALOR Approach | Key Improvement |
|---|---|---|---|---|
| 1 | PTSD & trauma | CPT/PE therapy (appointment-based); telemental health available; PTSD Residential Rehabilitation Treatment Programs for severe cases | SENTINEL: continuous HRV/EDA monitoring, real-time grounding protocols, 30-second crisis escalation — no appointment required | Eliminates the inter-appointment gap; bypasses stigma barrier; operates continuously not episodically |
| 2 | TBI cognitive support | Neuropsychology evaluations (clinic-based); TBI Care teams at Polytrauma Centers; limited home-based follow-up | SENTINEL: speech-to-text memory logging, name-recall facial recognition, task/calendar prompting, continuous cognitive load tracking | Continuous in-home cognitive support vs. periodic clinical evaluation |
| 3 | Chronic pain | Pain clinics, opioid prescriptions, some physical therapy; limited home-based delivery | NEXUS: TENS therapy delivery, heat/cold therapy, AI-optimized medication timing, posture alerts | Active in-home pain management vs. clinic visits for adjustment |
| 4 | Limb loss / amputation | Prosthetics clinics; VA covers advanced computerized limbs as of 2025; rehabilitation programs | NEXUS: real-time prosthetic Bluetooth calibration, grip-assist arm for fine motor tasks during prosthetic adjustment | Continuous real-time calibration vs. scheduled prosthetics appointments |
| 5 | Hearing loss & tinnitus | Audiology appointments; hearing aids issued; tinnitus ratings under review as of 2025 | NEXUS: 360-degree directional microphone, real-time speech amplification and transcription, tinnitus masking tones | Continuous ambient compensation vs. issued hardware with periodic fitting |
| 6 | Vision impairment | Low vision clinics; white cane programs; limited assistive technology | NEXUS: AI vision narration of surroundings, document reading, facial identification, obstacle detection | Continuous intelligent environmental narration vs. assistive device issuance |
| 7 | Sleep disorders | Sleep clinics; CPAP prescriptions; sleep apnea rating changes under review | SENTINEL: real-time sleep staging, smart environment control, VA sleep clinic data export | Home environment management and continuous staging vs. clinic assessment |
| 8 | Substance use & addiction | Substance Abuse Residential Rehabilitation (SARRTP); outpatient counseling; telehealth | SENTINEL: physiological pre-craving detection, distraction protocols, sponsor connection, sobriety milestone reinforcement | Pre-craving intervention vs. scheduled counseling after symptoms emerge |
| 9 | Depression & suicide risk | Mental health appointments; crisis line (988); telemental health; TMS now available for treatment-resistant depression | SENTINEL: NLP mood analysis of all interactions, activity tracking, automated 988 escalation in 30 seconds without veteran initiating | Active monitoring vs. passive self-report model; sub-minute crisis escalation |
| 10 | Social isolation | Community-based outreach; Vet Centers; peer support programs; VSO events | ATLAS: persistent-memory companionship AI, social calendar management, veteran event discovery, community matching | Always-present social bridge vs. periodic program participation |
| 11 | Unemployment | VA Vocational Rehabilitation & Employment (VR&E); TAP transitional assistance | ATLAS: AI career coach with military-to-civilian translation, real-time job matching, mock interviews, application pipeline tracking | Active ongoing coaching vs. program enrollment with limited individual support |
| 12 | Homelessness risk | HUD-VASH vouchers; outreach programs; veteran homelessness reached record lows in 2023–2024 but rose for unsheltered veterans | ATLAS + HERALD: financial health tracking, housing instability early warning, automated benefits enrollment to prevent financial cascade | Predictive prevention vs. reactive outreach after housing loss |
| 13 | MST recovery | MST coordinators at VA facilities; free counseling regardless of discharge status; confidential services | SENTINEL: offline-only encrypted sessions, trauma-informed voice persona options, no data accessible externally without veteran consent | Complete on-device privacy; removes institutional trust barrier; accessible without travel |
| 14 | VA navigation & benefits access | VSO referrals; VA.gov self-service portal; benefits counselors | HERALD: automated claim filing, continuous benefits gap scanning, appeal management, document vault | Proactive identification vs. veteran-initiated navigation of a complex system |
| 15 | Medication management | VA pharmacy (mail and in-person); adherence counseling at appointments | NEXUS: robotic dispenser with drug-interaction cross-referencing, missed-dose alerts to VA provider, auto-refill coordination | Active in-home dispensing and tracking vs. prescription issuance |
| 16 | Mobility limitations | Wheelchair programs; home modifications grants; power wheelchairs including smart models as of 2025 | NEXUS + PHALANX: laser-guided path planning, smart home integration, door/height control, outdoor GPS escort | Active mobility assistance vs. issued equipment without intelligent guidance |
| 17 | Grief & moral injury | Chaplain services; group therapy; some peer support programs | SENTINEL: guided narrative journaling with AI reflection, chaplain video connection, memorial archive for fallen comrades | Continuous reflective support available at any hour, including acute grief moments |
| 18 | Family reintegration | VA family counseling; caregiver support programs; SAVE training for families | ATLAS: structured reintegration conversation guides, family education modules, age-appropriate explanations for children, family counseling booking | Active facilitation vs. referral to standalone programs |
| 19 | Financial instability | VA debt resolution; financial counseling at some facilities; caregiver stipends | HERALD: VA debt resolution, budgeting tools, benefit payment tracking, financial counseling booking | Continuous financial monitoring vs. crisis-triggered counseling |
| 20 | Cognitive decline (aging veterans) | Geriatric care clinics; dementia screenings; caregiver support | NEXUS + HERALD: gamified cognitive fitness, validated dementia screening tools, fall detection, caregiver alert system | Daily cognitive engagement and continuous fall monitoring vs. periodic clinical screening |

---

> **The fundamental distinction:** The VA delivers care in episodes. VALOR delivers care continuously. The VA requires veterans to navigate toward the system. VALOR deploys the system to veterans. For many of the 20 challenges documented in this specification — especially those involving mental health, crisis prevention, and rural access — the difference between episodic and continuous support is the difference between intervention and tragedy.

> *These comparisons are based on publicly available VA program documentation, VA Inspector General reports, GAO findings, and peer-reviewed research as of 2025–2026. The intent is constructive: to demonstrate that VALOR's design addresses precisely the gaps that the existing system, by its structure, cannot close.*

---

## Research-to-Build Pipeline

> *VALOR must never be built on assumption, institutional momentum, or engineering enthusiasm alone. It must be built on evidence — rigorously collected, independently verified, and cleanly integrated. This section defines the canonical pipeline through which any research finding, from any source, travels before it influences a VALOR design decision, capability module, or clinical protocol.*

---

### Pipeline Philosophy

Four principles govern how research becomes product in VALOR:

**1. No finding enters production without reproducibility evidence.** A result that cannot be reproduced by an independent team is not a finding — it is a hypothesis. VALOR does not build clinical AI on hypotheses.

**2. Replicability must span veteran population subgroups.** A result that holds in one demographic, service branch, or clinical context but not others is a partial finding. VALOR's veteran population is heterogeneous; effects must replicate across the subgroups that matter.

**3. Integration is explicit, not implicit.** Every research finding that influences VALOR is formally logged, mapped to a specific module, and reviewed by both an engineering lead and a clinical lead. Informal hallway-conversation integrations are prohibited.

**4. The pipeline is bidirectional.** VALOR's deployment data is itself research. The pipeline does not only import findings from the academic world — it exports observations back to it, closing the loop between clinical AI deployment and the literature it is built on.

---

### Stage 1 — Research Discovery

**Purpose:** Systematically identify research relevant to VALOR's 20 challenge domains and underlying technology stack.

**Sources monitored:**

| Source Category | Examples | Cadence |
|---|---|---|
| Peer-reviewed clinical literature | PubMed, PsycINFO, JAMA, NEJM, LANCET | Monthly automated digest |
| VA and DoD research outputs | VA HSR&D, DoD CDMRP, RAND Arroyo | Quarterly manual review |
| Robotics and HRI research | IEEE RAS, ACM/IEEE HRI, ICRA, IROS | Conference cycle (1–2x/year) |
| Clinical AI and ML | NeurIPS clinical track, ML4H, CHIL | Conference cycle (2x/year) |
| Regulatory and standards bodies | FDA SaMD guidance, ISO 13482, IEC 62443 | As published |
| Veteran community evidence | VSO reports, VA Inspector General findings, veteran-led research | Quarterly |

**Discovery ownership:** Each VALOR work stream (WS-1 through WS-5) designates one **Research Liaison** responsible for monitoring the sources relevant to their domain and submitting candidate findings to the Research Intake Registry (see [Research Intake Registry](#research-intake-registry)).

**Submission threshold:** A finding is submitted to the intake registry if it meets any of the following criteria:
- It proposes or validates a technique directly applicable to a VALOR capability module
- It contradicts an assumption currently embedded in VALOR design
- It introduces a safety signal relevant to a deployed or planned module
- It describes outcomes from a veteran-population intervention with effect sizes large enough to motivate a design change

---

### Stage 2 — Reproducibility & Replicability Gate

> *This is the most important stage in the pipeline. No downstream work begins until a finding has been evaluated against rigorous reproducibility and replicability standards.*

**Purpose:** Filter out findings that do not meet the evidentiary standard required for clinical AI integration.

---

#### Reproducibility Assessment

Reproducibility asks: *can the same team, using the same data, methods, and code, produce the same result?*

Every candidate finding is evaluated against the following checklist:

| Criterion | Requirement | Acceptable Evidence |
|---|---|---|
| **Code availability** | Analysis code is publicly available or provided on request | GitHub/OSF repository link; verified executable |
| **Data availability** | Raw data is publicly available, or a synthetic equivalent is provided, or the study uses a publicly available benchmark dataset | DOI-linked dataset; IRB-restricted but requestable data with documented protocol |
| **Environment specification** | Software versions, hardware, and execution environment are fully documented | Docker image, conda environment, or detailed dependency manifest |
| **Pre-registered hypothesis** | Primary outcomes were pre-registered before data collection or analysis | OSF, ClinicalTrials.gov, or AsPredicted registration with timestamp predating data |
| **Statistical transparency** | Reported effect sizes, confidence intervals, and raw p-values (not just significance flags) | Full results table; no selective outcome reporting evident |
| **Negative results reported** | Failed conditions and null results are reported alongside positive results | Methods section documents pre-specified analyses; supplementary negative results table |

**Scoring:** Each criterion is scored Pass / Conditional Pass / Fail. A finding with two or more Fails does not advance. A finding with one Fail may advance to a Conditional Track — see below.

**Conditional Track:** A finding that fails one reproducibility criterion but is otherwise compelling may enter the pipeline with a mandatory internal reproduction attempt before Stage 4. VALOR's Research Team must independently reproduce the key result using the authors' code and/or a re-implementation before integration design begins.

---

#### Replicability Assessment

Replicability asks: *does the finding hold when a different team, using different data or methods, attempts to produce the same result?*

| Dimension | Question | Evidence Required |
|---|---|---|
| **Independent replication** | Has another independent lab or group reported a consistent finding? | Two or more independent publications with consistent direction of effect |
| **Population generalizability** | Were the study populations representative of the VALOR veteran population? | Subgroup data available for: age (>55 for aging veterans), sex, race/ethnicity, service branch, PTSD/TBI comorbidity status |
| **Effect magnitude consistency** | Are effect sizes consistent across replications, or only directionally consistent? | Forest plot or meta-analytic estimate preferred; single-study claims discounted |
| **Context robustness** | Does the finding hold in home/community settings, not just clinical lab settings? | At minimum one ecologically valid study; lab-only findings are flagged |
| **Temporal stability** | Do effects persist at follow-up (3+ months)? | Longitudinal data preferred; cross-sectional findings restricted to lower-autonomy modules |

**Population alignment scoring:** VALOR weights replicability evidence by how closely the study population matches the veteran cohort it would be applied to. A finding replicated specifically in combat veterans with PTSD carries more weight for SENTINEL configuration than a finding replicated only in a civilian anxious-adult population. Alignment scores (High / Moderate / Low) are recorded in the Intake Registry and govern the confidence tier assigned to the integration.

---

#### Confidence Tier Assignment

After the Reproducibility and Replicability Assessments, every finding is assigned a Confidence Tier that governs how it may be used in VALOR:

| Tier | Criteria | Permitted Integration Level |
|---|---|---|
| **Tier A — Production Ready** | Full reproducibility (all criteria pass) + independent replication + high population alignment | May inform autonomous module behavior, clinical threshold settings, and default configuration |
| **Tier B — Supervised Use** | Full reproducibility + at least one replication + moderate population alignment | May inform module behavior with mandatory human-in-the-loop review; cannot set autonomous escalation thresholds |
| **Tier C — Advisory Only** | Partial reproducibility OR single study with no replication | May inform design discussions and prototype exploration; cannot ship in any production module without elevation to Tier B/A |
| **Tier D — Watch List** | Promising but insufficient evidence; fails reproducibility gate | Logged in registry with reason; reassessed when new evidence appears; no integration |

---

### Stage 3 — VALOR Relevance Assessment

**Purpose:** Translate a vetted finding into a specific, scoped VALOR integration proposal.

A finding that passes Stage 2 is handed off to a **cross-functional triage panel** consisting of:
- The submitting Research Liaison
- The engineering lead for the affected work stream
- A clinical reviewer (CMO, clinical researcher, or VA clinical partner)
- A veteran representative from the Veteran Advisory Board (for findings that directly affect veteran interaction or clinical protocols)

The panel produces a **Research Integration Brief (RIB)** — a one-page structured document containing:

```
RESEARCH INTEGRATION BRIEF — TEMPLATE

Finding ID:        [R-YYYY-NNN]
Source:            [Citation + DOI]
Confidence Tier:   [A / B / C]
Submitted by:      [Research Liaison, WS-X]
Triage date:       [YYYY-MM-DD]

SUMMARY OF FINDING
[2–3 sentence plain-language summary of what the research found]

VALOR RELEVANCE
Affected archetype(s):    [SENTINEL / NEXUS / ATLAS / HERALD / PHALANX / VALOR-CORE]
Affected module(s):       [specific capability modules]
Challenge domain(s):      [1–20]

INTEGRATION HYPOTHESIS
[What specific change to VALOR design, configuration, or behavior does this finding motivate?]

SCOPE ESTIMATE
Engineering complexity:   [Low / Medium / High]
Clinical risk:            [None / Low / Medium / High]
Data requirements:        [What veteran data is needed to implement this?]
Privacy implications:     [Any new Tier-1/2/3 data handling implications?]

VETERAN ADVISORY BOARD REVIEW REQUIRED?
[Yes — if change affects interaction patterns, escalation logic, or privacy]
[No — if change is infrastructure or internal model configuration only]

RECOMMENDED ACTION
[Proceed to Stage 4 / Hold pending replication / Reject with rationale]
```

Completed RIBs are published to the Research Intake Registry within 10 business days of Stage 2 completion.

---

### Stage 4 — Integration Design Sprint

**Purpose:** Produce a concrete, scoped engineering specification for the finding's integration into VALOR.

Findings approved in Stage 3 enter a time-boxed **Integration Design Sprint** — a structured 2–4 week design process led by the relevant work stream engineering team, with mandatory clinical and VAB review at completion.

**Sprint deliverables:**

| Deliverable | Description |
|---|---|
| **Architecture Decision Record (ADR)** | Documents *what* is being changed, *why* (linking to the RIB and the underlying finding), *alternatives considered*, and *consequences*. ADRs are version-controlled and permanent. |
| **Data flow diagram** | Shows exactly what veteran data is consumed by the new behavior, where it is processed (edge vs. cloud), and what privacy tier it falls under |
| **Failure mode analysis** | Documents what happens if the integrated finding turns out to be wrong for a specific veteran — what is the observable failure signal, and what is the fallback behavior? |
| **Validation criteria** | Pre-specifies the measurable outcomes that will confirm the integration is working as intended in pilot, before any production rollout |
| **Rollback specification** | Defines exactly how the change is reversed if validation fails or a safety signal appears post-deployment |

**Mandatory review gates before Stage 5:**
- Engineering lead sign-off on ADR
- Clinical reviewer sign-off on failure mode analysis and validation criteria
- VAB review and approval if Veteran Advisory Board review was flagged in the RIB
- Privacy review if new Tier-1 or Tier-2 data handling is introduced

---

### Stage 5 — Prototype & Validation

**Purpose:** Test the integration in a controlled setting before it reaches any live veteran.

Integrations are validated in a three-environment progression:

**5a. Simulation Environment**
VALOR maintains a continuously updated simulation environment — a software replica of each archetype's sensor stack, decision logic, and VALOR-CORE integration — against which all changes are tested before hardware contact. Simulation runs:
- Standard veteran scenario suite (30 scripted scenarios covering the 20 challenge domains)
- Adversarial scenario suite (edge cases, sensor failure, ambiguous signals)
- Regression suite (all previously validated behaviors must continue to pass)

Simulation must achieve >95% expected-behavior rate against the validation criteria defined in Stage 4 before hardware testing.

**5b. Controlled Hardware Testing**
The integration is deployed on physical prototype hardware with simulated veteran data (synthetic profiles, not real veterans). Testing focuses on:
- Sensor integration correctness
- Latency requirements (crisis escalation: <30 seconds end-to-end)
- Privacy tier enforcement (Tier-1 data must not leave device)
- Robot behavior coherence across multi-archetype scenarios

**5c. Supervised Pilot Testing**
The integration is deployed to a small cohort of consenting pilot veterans (minimum 10, target 30) with enhanced logging and a dedicated clinical monitor assigned. Pilot runs for a minimum of 90 days. All pilot data is reviewed against pre-specified validation criteria at day 30, day 60, and day 90. The pilot is halted immediately if:
- A safety signal appears
- Veteran satisfaction ratings fall below the pilot threshold
- Clinical outcomes move in an unexpected direction

**IRB requirement:** Any Stage 5c pilot with a new clinical AI behavior (e.g., a new crisis escalation model, a new mood inference algorithm) requires an IRB amendment before deployment. Infrastructure changes with no clinical AI behavior impact may proceed under the existing IRB protocol with clinical reviewer documentation.

---

### Stage 6 — Production Integration

**Purpose:** Cleanly and traceably merge the validated integration into the VALOR production system.

**Integration requirements:**

| Requirement | Description |
|---|---|
| **Merged to `main` via reviewed PR** | All production code changes are peer-reviewed before merge. The PR must reference the Finding ID, ADR, and pilot results. |
| **Changelog entry** | Every production integration receives a changelog entry in the VALOR-CORE release notes, linking the change to its originating Research Finding ID |
| **Module version bump** | The affected capability module version is incremented, and the new version is documented in the module manifest alongside the Research Finding ID |
| **Clinical documentation update** | If the integration changes clinical behavior visible to VA providers, the VALOR clinical documentation is updated before the release ships |
| **Fleet rollout gating** | Production rollouts follow a staged deployment: 1% of fleet → 10% → 50% → 100%, with 72-hour hold periods between stages and automated rollback on anomaly detection |

**Traceability guarantee:** At any point in time, a VALOR engineer, VA clinical partner, or auditor must be able to answer: *"Why does VALOR-CORE behave this way?"* — and trace the answer directly to a Research Finding ID, its confidence tier, its RIB, its ADR, its pilot results, and the PR that merged it. This chain of custody is non-negotiable.

---

### Stage 7 — Post-Integration Monitoring

**Purpose:** Close the loop — confirm that the finding holds in real-world deployment and feed observations back to the research record.

Every production integration is assigned a **Post-Integration Monitoring Plan** specifying:

| Monitoring Element | Description |
|---|---|
| **Primary outcome metric** | The specific measurable outcome the finding predicted (e.g., "30-day crisis escalation rate," "medication adherence rate," "veteran-reported grounding protocol effectiveness") |
| **Monitoring cadence** | How frequently the outcome metric is reviewed (weekly automated / monthly clinical / quarterly strategic) |
| **Drift threshold** | The statistical threshold that triggers a review — defined as a pre-specified deviation from pilot baseline |
| **Veteran feedback integration** | Systematic collection of veteran-reported experience with the new behavior, analyzed quarterly |
| **Disconfirmation trigger** | The specific signal that would cause the integration to be flagged for rollback review |

**Feedback to research community:** When VALOR's deployment data provides evidence that confirms, extends, or contradicts the originating research finding, the VALOR Research Team is responsible for:
1. Documenting the real-world outcome data in the Intake Registry alongside the original finding
2. Sharing aggregate (de-identified, VA-approved) findings with the originating research team when a data sharing agreement is in place
3. Publishing VALOR outcome data in peer-reviewed literature on a Phase 1 / Phase 2 / Phase 3 cadence, as committed to in the Implementation Roadmap

---

### Research Intake Registry

The **VALOR Research Intake Registry** is the canonical, version-controlled record of every research finding that has been evaluated for VALOR integration. It is maintained as a structured database within the `valor/docs/research/` directory of the project repository.

**Registry schema:**

| Field | Type | Description |
|---|---|---|
| `finding_id` | String | Unique identifier: `R-YYYY-NNN` |
| `citation` | String | Full citation with DOI |
| `submission_date` | Date | Date submitted to registry |
| `submitted_by` | String | Research Liaison and work stream |
| `stage` | Enum | Current pipeline stage (1–7) or terminal status (Rejected / Watch List) |
| `confidence_tier` | Enum | A / B / C / D |
| `reproducibility_score` | Object | Pass/Fail per criterion |
| `replicability_score` | Object | Assessment per dimension |
| `population_alignment` | Enum | High / Moderate / Low |
| `affected_archetypes` | Array | SENTINEL, NEXUS, ATLAS, HERALD, PHALANX, VALOR-CORE |
| `affected_modules` | Array | Specific capability module names |
| `challenge_domains` | Array | Integer 1–20 |
| `rib_link` | URL | Link to Research Integration Brief document |
| `adr_link` | URL | Link to Architecture Decision Record (if Stage 4+) |
| `pilot_results_link` | URL | Link to Stage 5c pilot summary (if Stage 5+) |
| `production_pr_link` | URL | Link to merged production PR (if Stage 6+) |
| `monitoring_plan_link` | URL | Link to Post-Integration Monitoring Plan |
| `notes` | Text | Free-text notes from triage panel or subsequent review |

**Registry access:** The registry is readable by all VALOR contributors. Write access requires Research Liaison role or higher. The registry is published publicly (with any sensitive clinical detail redacted) as part of VALOR's commitment to research transparency.

---

### Reproducibility Standards

VALOR maintains its own internal reproducibility standards that extend beyond requiring them in incoming research. These standards apply to research *produced by* VALOR:

**All VALOR internal research (IRB studies, pilot analyses, outcome publications) must:**

1. **Pre-register** primary and secondary outcomes on ClinicalTrials.gov or OSF before data collection begins
2. **Publish analysis code** in the `valor/research/` repository within 60 days of manuscript submission
3. **Publish de-identified datasets** or synthetic equivalents within 60 days of manuscript acceptance, subject to VA data sharing agreements
4. **Report all pre-specified outcomes**, including null results — selective reporting is prohibited
5. **Report subgroup results** for: age cohort (18–34, 35–54, 55+), sex, race/ethnicity, service era (Vietnam, Gulf War, Post-9/11), and primary diagnosis category (PTSD, TBI, MST, physical disability, no mental health diagnosis)
6. **Apply CONSORT (for RCTs) or STROBE (for observational studies)** reporting standards to all manuscripts
7. **Mandate effect size reporting** with confidence intervals for all primary outcomes — p-values alone are insufficient

**Replication commitment:** For every major finding VALOR publishes, the research team designates an independent internal team to attempt replication before public release. Discrepancies between original and replication are documented in a supplementary note published alongside the manuscript.

---

### Pipeline Governance

The Research-to-Build Pipeline is governed by the **VALOR Research Integration Committee (RIC)**, a standing body that reports to the Chief Medical Officer.

**Committee composition:**

| Role | Count | Responsibilities |
|---|---|---|
| Chief Medical Officer (chair) | 1 | Final authority on Tier A/B confidence classifications and clinical safety decisions |
| Work Stream Research Liaisons | 5 (one per WS) | Discovery, submission, and Stage 3 triage participation |
| Clinical AI Lead | 1 | Technical review of AI/ML findings; simulation environment ownership |
| IRB & Regulatory Specialist | 1 | Stage 5c protocol compliance; FDA pre-submission alignment |
| Veteran Advisory Board Representative | 1 (rotating) | Veteran perspective in triage and design sprint review |
| Privacy Officer (advisory) | 1 | Review of any finding that introduces new data handling |

**RIC cadence:**
- Weekly: Intake registry review — new submissions triaged, stage updates reviewed
- Monthly: Active Stage 4–6 integrations reviewed for timeline and risk
- Quarterly: Post-integration monitoring data reviewed; Watch List reassessed against new literature
- Annually: Full pipeline audit — Are confidence tier assignments still appropriate? Are any production integrations now contradicted by new evidence?

**Appeal and override process:** Any VALOR contributor may formally challenge a Confidence Tier assignment or an integration approval by submitting a written challenge to the RIC. The RIC must respond within 15 business days. If the challenge is sustained, the finding is re-evaluated from Stage 2. No integration that has received a formal challenge may proceed to production until the challenge is resolved.

---

> *The Research-to-Build Pipeline is how VALOR earns the right to operate in a veteran's home. Every intervention VALOR takes — every grounding protocol, every medication alert, every crisis escalation — is downstream of a finding that passed through this pipeline. The veteran trusts VALOR. VALOR must trust only evidence.*

---

## Contributing

VALOR is a public interest engineering project. Contributions are organized by archetype and layer:

```
valor/
├── valor-core/          # Shared AI backbone, VA API integrations, inter-robot protocol
├── sentinel/            # Mental health, crisis detection, sleep, MST modules
├── nexus/               # Physical health, medication, prosthetics, mobility modules
├── atlas/               # Social, career, family, housing modules
├── herald/              # VA navigation, financial, legal, document vault modules
├── phalanx/             # Outdoor navigation, environmental sensing, emergency response
├── humanoid/            # -H variant hardware specs, gait/expression systems, safety protocols
├── personalization/     # Intake framework, profile schema, adaptive behavior models
├── transfer/            # Sanitization protocol, logistics integration, reallocation systems
├── hardware/            # Robot chassis specs, sensor integration, form factor documentation
├── privacy/             # Data classification, encryption, consent management
├── research/            # Research Intake Registry, RIBs, ADRs, pilot results, published datasets
└── docs/                # System vision, architecture decision records, policy briefs
```

For architectural questions, design decisions, or policy collaboration, open an issue with the label `architecture`, `policy`, or the relevant archetype name.

---

---

## The Standard Model of Physics — Applied to Veteran Care

> **A deep understanding of the Standard Model of Particle Physics — the most precisely tested scientific theory in human history — is not an abstract academic exercise. It is the invisible substrate beneath every sensor, every semiconductor, every medical scanner, every material, and every communication technology in the VALOR System. The veterans who carry service-connected injuries, TBI, chronic pain, and invisible wounds deserve care built on the deepest possible understanding of the physical universe. This section demonstrates why.**

---

### What Is the Standard Model?

The **Standard Model of Particle Physics** is the theoretical framework that describes the fundamental constituents of matter and the forces that govern their interactions. It accounts for three of the four known fundamental forces — the electromagnetic force, the strong nuclear force, and the weak nuclear force — and classifies all known elementary particles.

**The particle zoo in brief:**

| Category | Particles | Role |
|---|---|---|
| **Quarks** | up, down, charm, strange, top, bottom | Constituents of protons and neutrons; define nuclear matter |
| **Leptons** | electron, muon, tau, and three neutrinos | Electrons form atoms; enable all chemistry and biology |
| **Gauge bosons** | photon (γ), W±, Z⁰, gluon (g) | Force carriers: EM, weak, strong forces |
| **Scalar boson** | Higgs (H⁰) | Gives mass to W±, Z⁰, and all fermions via the Higgs mechanism |

The Standard Model's predictive precision is extraordinary — the electron's anomalous magnetic moment (g-factor) is predicted to 12 decimal places and confirmed experimentally. This is not a model that merely approximates reality; it describes it with a fidelity unmatched in any other branch of science.

The practical implication: **every technology VALOR deploys — from MRI scanners to semiconductor chips to laser rangefinders to radiation therapy — is a direct engineering application of Standard Model physics.** The further our understanding of the Standard Model extends, the more precisely and powerfully we can build tools to serve veterans.

---

### 1. Electromagnetic Force — The Foundation of Every VALOR Sensor

The photon is the force carrier of electromagnetism. Every sensor in the VALOR fleet is, at root, a photon-interaction device.

**LiDAR and spatial navigation:** PHALANX and all mobile archetypes use LiDAR — time-of-flight photon measurement — to construct 3D maps of the veteran's environment. The physics of photon propagation at the speed of light, and the precision with which we can time those returns (thanks to quantum electrodynamics, or QED, which is the Standard Model's description of photon-electron interaction), directly determines VALOR's ability to navigate safely around a veteran in a wheelchair, avoid a service dog, or detect a veteran who has fallen.

**Photoplethysmography (PPG) — heart rate and HRV:** SENTINEL's biometric wrist module detects blood volume pulse by shining infrared photons through the skin and measuring the fraction absorbed by hemoglobin. The absorption spectrum of hemoglobin is a direct consequence of its quantum electronic structure — governed entirely by QED. Understanding the precise wavelength-dependent absorption cross-sections, how they shift under different physiological states, and how scattering in tissue affects signal quality all require fluency with Standard Model electromagnetism.

**Galvanic skin response (GSR):** Electron flow (current) through sweat-moistened skin is a PTSD stress proxy SENTINEL uses for crisis detection. The electron — a lepton in the Standard Model — is the charge carrier. Ionic conductance in electrolyte solutions, skin impedance models, and signal fidelity under motion artifact are all electromagnetic phenomena at the quantum level.

**Thermal imaging:** NEXUS uses infrared thermography to map pain-related inflammation. Thermal photons emitted by tissue (blackbody radiation, governed by Planck's law — itself a quantum mechanical result rooted in photon statistics) encode tissue temperature with millimeter-scale spatial resolution. The capacity to detect a veteran's inflamed joint before they report pain depends on the precision with which we understand photon emission and detection.

> **Applied to VALOR:** A SENTINEL team that deeply understands QED can design biometric sensors with better SNR, lower false positive rates in crisis detection, and greater accuracy under motion — directly reducing missed crisis escalations and false alarms that erode veteran trust.

---

### 2. Semiconductor Physics — The Engine of Every AI Inference Chip

The transistor is a quantum mechanical device. Without the Standard Model — specifically, the quantum theory of how electrons inhabit energy bands in crystalline solids (a direct consequence of quantum electrodynamics applied to periodic lattices) — there is no NVIDIA Jetson, no edge AI inference, and no VALOR-CORE running on-robot.

**Band gap engineering:** The distinction between a conductor, semiconductor, and insulator is entirely a consequence of how electrons (Standard Model leptons) interact with the periodic potential of an atomic lattice via the electromagnetic force. Silicon's 1.1 eV band gap — which makes it ideal for room-temperature electronics — is calculable from first principles using Standard Model inputs. Gallium nitride (GaN), used in high-efficiency power converters that extend VALOR's battery life, has a 3.4 eV band gap exploited precisely because engineers understood its quantum origin.

**Moore's Law ceiling and quantum tunneling:** As transistor gate lengths shrink below 5 nm (current commercial chips), electrons tunnel quantum mechanically through barriers — a distinctly Standard Model phenomenon with no classical analog. Understanding when tunneling leakage becomes device-limiting, and how to design around it (FinFETs, gate-all-around architectures, topological insulators), requires exactly the quantum field theory that underlies the Standard Model. VALOR's roadmap into its 50-year and 100-year mandate will witness multiple generations of post-silicon computing substrates, each exploiting deeper Standard Model phenomena.

**Spintronics and MRAM:** Emerging memory technologies that may eventually replace DRAM exploit *electron spin* — a purely quantum mechanical property that has no classical equivalent and emerges directly from the Dirac equation (relativistic quantum mechanics, the theoretical backbone of the Standard Model's fermion sector). MRAM offers non-volatile, radiation-hard memory with zero standby power — highly relevant to VALOR robots operating continuously in veteran homes. Understanding spin is understanding the Standard Model's description of fermionic angular momentum.

> **Applied to VALOR:** Hardware engineers on the VALOR team who understand semiconductor quantum mechanics at the Standard Model level are equipped to evaluate next-generation chip platforms, predict where thermal and quantum noise floors lie, and ensure VALOR-CORE's inference hardware remains state-of-the-art across the 100-year mandate without black-box vendor dependency.

---

### 3. Medical Imaging — The Standard Model in the Clinic

The most transformative diagnostic technologies in veteran healthcare are direct applications of Standard Model physics. Veterans carry some of the highest rates of TBI, musculoskeletal injury, and blast-exposure-related organ damage of any patient population — and imaging these injuries accurately determines treatment, benefits eligibility, and quality of life.

**MRI — Nuclear Magnetic Resonance:** MRI exploits the *nuclear spin* of hydrogen nuclei (protons) — a property described by the Standard Model's treatment of the strong and electromagnetic forces operating at the nuclear level. A proton placed in a strong magnetic field precesses at a Larmor frequency governed by its nuclear magnetic moment (a quantity calculable from QCD, the Standard Model's description of the strong force). RF photons at exactly this frequency flip the spin; the relaxation signal encodes tissue contrast. TBI — the "invisible wound" of post-9/11 veterans — is best characterized by diffusion tensor MRI, which maps white matter microstructure at a resolution that reveals axonal shear injuries invisible to CT. Every improvement in MRI resolution and contrast is downstream of deeper understanding of nuclear spin physics.

**PET scanning — Positron-Electron Annihilation:** PET imaging — used to assess TBI-related neuroinflammation and PTSD-related amygdala hyperactivity — operates on positron emission from radioactive tracers. The positron is the antiparticle of the electron, predicted by the Standard Model's Dirac equation and discovered in 1932. When a positron annihilates with an electron, two 511 keV photons are emitted at exactly 180° — a consequence of conservation of 4-momentum in Standard Model quantum electrodynamics. PET scanners detect these coincident photons to localize the tracer. Without Standard Model physics, PET is inexplicable; with it, it is engineerable to sub-millimeter accuracy.

**X-ray and CT — Compton Scattering and Photoelectric Absorption:** X-ray imaging of veteran musculoskeletal injuries (blast-fractured vertebrae, shrapnel-adjacent bone damage, prosthetic interface osseointegration) depends on differential photon absorption by tissue — governed by the photoelectric effect and Compton scattering, both QED processes. CT's ability to reconstruct 3D bone and soft tissue structure from 2D projection images applies the mathematics of the Radon transform to photon attenuation data with physics roots in the Standard Model.

**Radiation therapy for veteran cancer:** Veterans exposed to Agent Orange, burn pit emissions, or ionizing radiation during service carry elevated cancer rates. Radiation oncology delivers precisely localized photon or proton beams to tumors while sparing surrounding tissue. Proton therapy, in particular, exploits the Bragg peak — the sharp energy deposition maximum at the end of a charged particle's range — a consequence of the Bethe-Bloch equation, which describes charged particle energy loss through matter using Standard Model inputs. NEXUS's role as a health advocate means understanding which veteran diagnoses respond to which treatment modalities — and physics literacy enables the system to surface proton therapy candidacy where appropriate.

> **Applied to VALOR:** NEXUS's health-data integration modules, and HERALD's benefits eligibility navigation for service-connected conditions, both improve when the system can reason fluently about the diagnostic modalities veterans are undergoing — what they measure, what they miss, and how their outputs map to clinical decisions.

---

### 4. Materials Science — Prosthetics, Armor, and Biomechanics

The Standard Model governs the behavior of electrons in chemical bonds — which means it governs the properties of every material. For veterans with limb loss, blast injury, and chronic musculoskeletal damage, material science is not abstract.

**Prosthetic limbs and the physics of carbon fiber:** Modern below-knee prostheses use carbon fiber composites whose extraordinary specific stiffness and fatigue resistance emerge from the quantum mechanical bonding structure of the sp² carbon lattice — a consequence of how electrons hybridize according to QED and quantum chemistry. The energy-return properties of a running blade — the difference between a veteran returning to competitive athletics versus limping through daily life — are tunable precisely because materials engineers understand the electron-level physics that determines elastic modulus and failure modes.

**Osseointegration implants:** Titanium's biocompatibility — its ability to bond directly to bone without rejection — is a quantum surface effect. The native TiO₂ oxide layer that forms on titanium surfaces creates an electronic interface that resists protein denaturation and supports osteoblast adhesion. This is electron chemistry all the way down. Understanding it at the Standard Model level allows biomaterials engineers to tune surface oxide thickness, doping levels, and photon-activated surface treatments to improve osseointegration outcomes for veteran amputees.

**Smart textiles and wearable sensors:** SENTINEL's biometric wrist module and NEXUS's physiological monitoring depend on flexible electronics and smart textiles that maintain signal fidelity through motion. Conductive polymers (PEDOT, graphene-based inks) exploit conjugated electron systems — delocalized π electrons that form charge transport channels through molecular orbital overlap, calculable via quantum chemistry. The ability to design stretchable conductors that remain electrically stable through a veteran's full range of motion is a direct application of understanding electron behavior in non-crystalline soft-matter systems.

> **Applied to VALOR:** NEXUS's physical health modules — particularly prosthetic interface monitoring, pain management, and physical therapy guidance — benefit from a materials-physics-literate design team that can evaluate emerging prosthetic and sensor materials against first-principles performance criteria rather than relying solely on manufacturer specifications.

---

### 5. Quantum Sensing — The Next Frontier for Veteran Health Monitoring

The Standard Model's quantum mechanical framework is opening a new generation of sensors that will dramatically improve VALOR's capabilities within the 100-year mandate window.

**Quantum magnetometers (OPMs) for non-invasive brain activity:** Optically pumped magnetometers (OPMs) use quantum transitions of alkali metal atoms (rubidium, cesium) to detect magnetic fields 100× weaker than SQUID-based MEG scanners, and — critically — they operate at room temperature. The physics is Standard Model atomic spectroscopy: photons drive transitions between hyperfine energy levels split by the nuclear magnetic moment (strong force) and electron spin (QED). OPM-MEG systems are wearable, lightweight, and can map real-time neural activity with millisecond temporal resolution. For veterans with TBI and PTSD — whose neurological signatures are subtle and require high-sensitivity imaging — OPM technology could enable SENTINEL to monitor brain state continuously and non-invasively, detecting pre-crisis neural patterns before behavioral symptoms emerge.

**Nitrogen-vacancy (NV) centers in diamond for nanoscale sensing:** NV centers in diamond lattices are point defects whose spin state can be initialized and read optically — a quantum information system operating at room temperature. Their extreme magnetic field sensitivity (single-neuron-level field detection) and single-photon emission properties make them candidates for next-generation medical imaging and precision drug delivery tracking. Standard Model quantum optics and solid-state spin physics govern every aspect of their operation.

**Quantum communication and veteran data security:** HERALD handles sensitive VA benefits data, legal documents, and health records. Quantum key distribution (QKD), enabled by the no-cloning theorem of quantum mechanics (a theorem about photon quantum states, rooted in the Standard Model), makes eavesdropping on encrypted channels physically impossible — not merely computationally infeasible. As quantum computing matures, QKD becomes the gold standard for protecting veteran data from adversarial decryption. Understanding QKD at the physics level allows HERALD's privacy architecture to evolve appropriately over the 100-year mandate.

> **Applied to VALOR:** Quantum sensing represents the most significant near-future expansion of VALOR's diagnostic and monitoring capabilities. The team members capable of evaluating, integrating, and troubleshooting these systems are those who understand the Standard Model at a level deep enough to bridge physics and engineering.

---

### 6. Nuclear Medicine — Veteran-Specific Cancer and Toxin Exposure

Veterans of multiple service eras carry elevated radiological and chemical exposure burdens. Agent Orange (dioxin), burn pit particulates, depleted uranium, and nuclear test observation have produced cancer clusters in veteran populations that require sophisticated nuclear medicine responses.

**Alpha and beta decay for targeted radiotherapy:** Targeted alpha therapy (TAT) uses alpha-emitting isotopes (Bismuth-213, Actinium-225) conjugated to antibodies that seek specific tumor antigens. The alpha particle (a helium-4 nucleus — two protons and two neutrons, constituents described entirely by QCD and the strong force) deposits all its energy within ~100 microns of emission, sparing surrounding tissue. This extraordinary spatial precision — a direct consequence of the Standard Model's description of heavy charged particle energy loss — makes TAT particularly promising for the disseminated cancers that burn-pit and Agent Orange exposures produce. Veterans deserve oncologists and benefit advocates who understand why this matters.

**Neutron activation analysis for exposure documentation:** Depleted uranium exposure produces uranium deposits in bone and kidney. Neutron activation analysis — bombarding tissue or urine samples with neutrons (Standard Model strong-force mediated nuclear scattering) and detecting the characteristic gamma rays from activated isotopes — can quantify trace uranium loads at parts-per-billion sensitivity. Veterans seeking service-connection for DU-related kidney disease or cancer need diagnostic tools accurate enough to document the exposure; those tools are Standard Model applications.

> **Applied to VALOR:** HERALD's benefits navigation module and NEXUS's health-monitoring module gain substantive capability when the VALOR team understands the nuclear physics underlying veteran-specific exposure pathologies — allowing VALOR to intelligently surface diagnostic options, flag exposure-related symptom clusters, and connect veterans to the specialized oncology resources their conditions require.

---

### 7. The Weak Force — Beta Decay in PET and Neuroimaging

The weak nuclear force — mediated by the massive W± and Z⁰ bosons (whose masses arise via the Higgs mechanism) — governs radioactive beta decay. This is the physics behind PET tracers.

**FDG-PET for veteran neuroimaging:** [¹⁸F]-fluorodeoxyglucose (FDG) is the most widely used PET tracer for brain glucose metabolism. Fluorine-18 undergoes positron emission (β⁺ decay, a weak force process mediated by W⁺ boson exchange: a proton converts to a neutron, emitting a positron and a neutrino) with an 110-minute half-life — long enough for clinical imaging, short enough to minimize radiation dose. The design of PET tracers — choosing isotopes with the right half-life, decay energy, and chemical incorporation — requires fluency with weak force nuclear physics. Veterans with PTSD show characteristic FDG-PET hypometabolism in the prefrontal cortex and hypermetabolism in the amygdala; these patterns are diagnostic signatures that NEXUS's health data integration modules should recognize and surface for clinical review.

**Neutrino detection and future medical physics:** The Standard Model predicts three neutrino flavors, each interacting only via the weak force and gravity. While currently too weakly interacting to be clinically useful, coherent elastic neutrino-nucleus scattering (CEνNS) experiments are pioneering ultra-sensitive nuclear recoil detectors. The same detector technology that catches neutrinos is being adapted for dark matter searches and, prospectively, for medical isotope production monitoring. The 100-year mandate horizon means VALOR should be architected to incorporate technologies whose current form exists only in physics laboratories.

> **Applied to VALOR:** Understanding weak-force nuclear physics gives the VALOR clinical team the foundation to interpret PET neuroimaging findings accurately, communicate them to VA providers effectively, and evaluate next-generation brain imaging modalities as they transition from research to clinical application.

---

### 8. The Higgs Field — Mass, Inertia, and Why Matter Exists at All

The Higgs boson — discovered at CERN in 2012 — is the quantum excitation of the Higgs field, which permeates all of space and gives mass to the W±, Z⁰ bosons and all fermions through the Brout-Englert-Higgs mechanism. Without the Higgs mechanism, the weak force bosons would be massless (like the photon), the weak force would have infinite range, and nuclear chemistry as we know it would not exist — nor would atoms, molecules, biology, or veterans.

This is not merely philosophical. The Higgs mechanism tells us something deep about why matter has the properties it does — why hydrogen is stable, why carbon forms four bonds, why DNA stores information, why neurons fire. Every medical technology, every material, every drug, every diagnostic probe ultimately traces its properties back to the mass spectrum of elementary particles set by their Yukawa couplings to the Higgs field.

For a project operating on a 100-year mandate, understanding that VALOR's technologies are not arbitrary inventions but consequences of deep physical law is a source of long-term engineering confidence. The Standard Model will not be repealed. The electron's charge will not change. The speed of light will not shift. This stability of physical law is the bedrock on which century-scale engineering commitments can be made.

> **The design principle this unlocks:** VALOR's 100-Year Mandate is undergirded by physics that is genuinely permanent. The technological implementations change; the physics does not. A VALOR engineer who understands why the laws are what they are — not just that they are — is equipped to evaluate radically new technologies against stable physical constraints, distinguishing genuine innovation from speculative noise across the entire mandate horizon.

---

### 9. Summary — The Standard Model as a VALOR Design Resource

The table below maps Standard Model physics domains to specific VALOR capabilities:

| Standard Model Domain | Force / Particle | VALOR Application | Affected Archetype(s) |
|---|---|---|---|
| Quantum electrodynamics (QED) | Photon, electron | LiDAR navigation, biometric sensors (PPG, GSR), thermal imaging, semiconductor chips | All (especially SENTINEL, PHALANX) |
| Band structure / solid-state QM | Electron in periodic lattice | Transistors, edge AI inference chips, battery chemistry, spintronics memory | VALOR-CORE, all archetypes |
| Nuclear magnetic resonance | Proton spin (strong + EM) | MRI for TBI diagnosis, fMRI for PTSD neuroimaging | NEXUS, HERALD |
| Positron-electron annihilation | Positron (QED, Dirac) | PET scanning for neuroinflammation, cancer staging | NEXUS, HERALD |
| Compton scattering / photoelectric | Photon-electron (QED) | X-ray and CT imaging of blast injuries, prosthetic interface | NEXUS, HERALD |
| Charged particle energy loss (Bethe-Bloch) | Proton (QED) | Proton therapy for veteran cancers | NEXUS, HERALD |
| Quantum atomic spectroscopy | Photon, alkali atom hyperfine | OPM-MEG wearable brain imaging | SENTINEL, NEXUS |
| NV center spin physics | Electron spin (QED) | Next-generation nanoscale sensing | SENTINEL (future) |
| Quantum key distribution | Photon (QED no-cloning) | Veteran data security, HERALD document vault | HERALD, VALOR-CORE |
| Beta decay (weak force, W± boson) | W±, neutrino | PET tracer design, FDG-PET neuroimaging | NEXUS |
| Alpha decay (strong / QCD) | Alpha particle | Targeted alpha therapy for veteran cancers | NEXUS, HERALD |
| Higgs mechanism | Higgs field, mass generation | Why matter exists and has stable properties; 100-year design confidence | VALOR-CORE (philosophical / architectural) |
| Neutron activation analysis | Neutron (strong force) | DU exposure documentation, service-connection evidence | HERALD, NEXUS |
| Materials quantum chemistry | Electron bonding (QED) | Carbon fiber prosthetics, Ti osseointegration, smart textile sensors | NEXUS |

---

### 10. Conclusion — Why VALOR Teams Should Study Physics

The argument is simple:

1. Every sensor VALOR uses, every chip VALOR runs on, every medical scanner that images a veteran's wounds, every prosthetic limb that restores a veteran's mobility, and every encryption system that protects a veteran's most sensitive data is a direct consequence of Standard Model physics.

2. A team that understands this physics at depth — not merely as a user of technology products, but as practitioners who can reason from physical law — can evaluate new technologies more rigorously, identify failure modes earlier, and build systems that will remain technically coherent across the 100-year mandate.

3. Veterans who have sacrificed the most deserve care built on the deepest possible foundations. The Standard Model is the deepest foundation physics has yet found. VALOR should build from it, not just on top of it.

> **The Standard Model is not a section of a physics textbook. It is the operating manual for the universe in which veterans are injured, healed, remembered, and served. VALOR should read it.**

---

> *VALOR System Vision — Version 6.0*  
> *Claude AI was used in producing this system overview, README file, and build roadmap.*  
> *This document is a conceptual vision for public interest discussion and policy development. All cost figures are estimates based on published research. All technical capabilities described are based on existing or near-term commercially available technologies. VA comparison data in Section 22 is drawn from VA Office of Inspector General reports, GAO findings, and peer-reviewed research published through 2025–2026.*  
> *Version 5.1 adds the Research-to-Build Pipeline (Section 23) — the formal framework governing how external research findings and internal pilot outcomes are evaluated for reproducibility and replicability before integration into VALOR design, clinical protocols, and production modules.*  
> *Version 5.2 adds The Mobility Imperative (Section 5) — a dedicated analysis of why mobility is the foundational architectural requirement for the VALOR fleet. Mobility language has been strengthened throughout all archetype descriptions, the Design Principles, the Case for a Robot Fleet, the Build Roadmap, and the Top Development Challenges. HERALD's optional mobile variant benefits have been formally documented. PHALANX mobility-as-mission language has been elevated throughout.*  
> *Version 6.0 adds The Standard Model of Physics — Applied to Veteran Care (Section 25) — a comprehensive demonstration of how deep understanding of particle physics, quantum electrodynamics, nuclear forces, and the Higgs mechanism directly underlies every sensor, chip, medical imaging system, prosthetic material, and data security architecture in the VALOR System, with explicit mapping of Standard Model domains to VALOR archetypes and capabilities.*  
> *These veterans gave everything. VALOR's mission is to give something back that matches the scale of what they carry — a system that is as persistent, as adaptive, and as committed as they are.*
