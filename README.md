# VALOR — Veteran Adaptive Life-Assistance and Operations Robot System

> A distributed mobile robot fleet for comprehensive veteran support across all 20 domains of veteran life. This is a personal idea and project and this repository is not affiliated with the VA. Claude AI from Anthropic was used for this project.

[![System Status](https://img.shields.io/badge/status-concept--phase-blue)]()
[![Archetypes](https://img.shields.io/badge/robot%20archetypes-5-teal)]()
[![Capabilities](https://img.shields.io/badge/capability%20modules-20-purple)]()
[![License](https://img.shields.io/badge/license-VA%20Research-green)]()

---

## Table of Contents

1. [Vision](#vision)
2. [The Case for a Robot Fleet](#the-case-for-a-robot-fleet)
3. [System Overview](#system-overview)
4. [Design Principles](#design-principles)
5. [Veteran Personalization Profile](#veteran-personalization-profile)
6. [VALOR-CORE Backbone](#valor-core-backbone)
7. [Robot Archetypes](#robot-archetypes)
   - [SENTINEL — Mental Health & Crisis Guardian](#sentinel--mental-health--crisis-guardian)
   - [NEXUS — Physical Health & Mobility Platform](#nexus--physical-health--mobility-platform)
   - [ATLAS — Social Life & Community Bridge](#atlas--social-life--community-bridge)
   - [HERALD — Benefits, Administration & Financial Guardian](#herald--benefits-administration--financial-guardian)
   - [PHALANX — External Environment & Safety Scout](#phalanx--external-environment--safety-scout)
8. [Humanoid Robot Options](#humanoid-robot-options)
9. [Inter-Robot Communication](#inter-robot-communication)
10. [Cascade Prevention — How the Fleet Works Together](#cascade-prevention--how-the-fleet-works-together)
11. [Robot Transfer & Reassignment Protocol](#robot-transfer--reassignment-protocol)
12. [Technology Architecture](#technology-architecture)
    - [Sensing Layer](#sensing-layer)
    - [AI & Compute Layer](#ai--compute-layer)
    - [Privacy & Security](#privacy--security)
13. [The 20 Veteran Challenges Addressed](#the-20-veteran-challenges-addressed)
14. [Implementation Roadmap](#implementation-roadmap)
15. [**Build Roadmap & Development Plan**](#build-roadmap--development-plan) ← *New in v3*
16. [Financial Case & ROI](#financial-case--roi)
17. [Policy Framework](#policy-framework)
18. [Contributing](#contributing)

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

---

## System Overview

VALOR is not a replacement for human caregivers, VA providers, or peer support specialists. It is the always-present connective tissue between a veteran and every support system that exists for them — lowering the barrier to access, preventing crises before they occur, and ensuring no veteran falls through the cracks because navigating the system requires more energy than they have on a given day.

Each robot in the fleet:
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
**Form factor:** Mobile desktop companion (~tablet on wheeled base); moves autonomously between rooms; warm non-humanoid curved display; always-on local-only wake detection  
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
**Form factor:** Largest fleet unit (~bedside clinical cart); articulated arms with soft-robotics grippers (3 kg payload); 12-hour battery; wireless charging dock; designed for indoor home environments  
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
**Form factor:** Compact rolling unit (~large speaker on base); minimal display surface; quiet, slow-moving; designed for living rooms and common areas; docks autonomously when veteran has visitors  
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
**Form factor:** Desktop-docked display unit with touchscreen interface; serves as the veteran's primary VALOR-CORE dashboard; does not need to move

**Capability modules:**

| Module | Description |
|---|---|
| VA benefits navigator | Automated claims filing, status tracking, appeal support; continuously scans for unclaimed benefits matching the veteran's profile |
| Document vault | Encrypted secure storage for DD-214, medical records, legal documents; OCR scanning via NEXUS document scanner |
| Financial health manager | Benefit payment tracking, budgeting tools, VA debt resolution, financial counseling booking |
| Legal resource connector | VSO referral, JAG consultation scheduling, discharge upgrade tracking |
| Appointment coordinator | Pulls VA schedule API, manages all medical and benefits appointments across the fleet |

**Key integration:** HERALD is the administrative hub of the fleet. NEXUS feeds pharmacy data for auto-refills; SENTINEL feeds mental health appointment needs; ATLAS feeds career and education program bookings.

---

### PHALANX — External Environment & Safety Scout

**Nickname:** "The Scout"  
**Domain:** Outdoor navigation, environmental hazard detection, and emergency response  
**Form factor:** Ruggedized wheeled outdoor unit; weather-resistant; GPS + LiDAR; runs ahead of or alongside the veteran in outdoor environments  
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

### Phase 2 — Expansion (Years 3–4) · $280M

- [ ] NEXUS and ATLAS brought to production quality
- [ ] Full fleet integration: all 5 archetypes operating as coordinated system
- [ ] Humanoid variant pilot: 500-unit SENTINEL-H and ATLAS-H deployment with controlled comparison study
- [ ] 5,000-unit deployment across 25 VAMCs and rural outreach programs
- [ ] Outcome data published; VA and CMS reimbursement pathway established
- [ ] Commercial licensing discussions with allied nation VA equivalents (UK, Canada, Australia)

### Phase 3 — Scale (Years 5–8) · $800M+

- [ ] PHALANX outdoor scout brought to production; PHALANX-H variant for eligible veterans
- [ ] 50,000+ units deployed nationwide; priority to rural and underserved veterans
- [ ] VALOR-CORE published as open API for VSOs, nonprofit caregivers, community health workers
- [ ] Cost per unit at scale: $18,000–$24,000 (comparable to power wheelchair)
- [ ] Full VA reimbursement for all veterans with qualifying disability ratings (50%+)
- [ ] Transfer pool operational: refurbished units available for rapid reallocation nationwide

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
- Select chassis from Gate 0 evaluation. Recommended form factor: compact wheeled base with a curved OLED/LCD display panel, silent drive motors, and a docking station with wireless charging.
- Integrate NVIDIA Jetson Orin module as edge compute unit. Validate thermal envelope and battery life under continuous inference load.
- Integrate the biometric wrist module as a separate companion device: select and validate a PPG + EDA + accelerometer module (e.g., based on MAX86150 or similar clinical-grade sensor IC). Commission custom wrist band enclosure.
- Integrate mattress pressure sensor pad for sleep staging (select from commercially available sleep mat options; validate sleep stage accuracy against PSG gold standard in a 20-subject sleep study).
- Validate that all Tier-1 biometric processing runs fully on-device with zero cloud dependency for emergency escalation.

**SENTINEL Prototype v2 (Months 12–18)**
- Integrate VALOR-CORE v0.5 connectivity
- Implement the seven SENTINEL capability modules in software: PTSD detection, TBI cognitive support, depression/suicide risk monitor, sleep environment management, substance craving intervention, grief/moral injury, MST support
- Field test with 10 veteran co-design participants: observed sessions, usability interviews, interaction design iteration
- Submit IRB protocol for the 500-unit pilot study

#### WS-2: HERALD Hardware (Months 7–14)

HERALD is the simplest hardware archetype — a docked display unit — which is intentional. Its value is software, not mobility.

- Select commercial touchscreen display unit as base (10–13" tablet in ruggedized kiosk enclosure, or custom build)
- Integrate document scanner module (USB or embedded, 300 DPI minimum, auto-crop)
- HERALD software implementation: VA benefits navigator, document vault, financial health manager, appointment coordinator, legal resource connector
- HERALD serves as the veteran's primary VALOR-CORE dashboard — implement the profile viewer, consent manager, and data audit interface here

#### WS-3: Clinical AI Models (Months 7–24)

This work stream runs in parallel with hardware and is the most technically risk-laden area. Key models to develop or adapt:

| Model | Approach | Validation requirement |
|---|---|---|
| PTSD/stress detection from HRV + EDA | Fine-tune on veteran biometric dataset; baseline from published HRV-stress literature | 80%+ sensitivity at <5% false positive rate in held-out veteran cohort |
| Mood/depression inference from voice NLP | Adapt existing speech affect models (e.g., based on openSMILE feature set + fine-tuned transformer) | Validated against PHQ-9 scores in pilot cohort |
| Sleep stage classification from mattress pressure | Train on pressure-PSG paired dataset; compare to commercial sleep mat accuracy benchmarks | AHI correlation r > 0.85 vs. PSG |
| Substance craving pre-signal detection | Most speculative model; begin with HRV + EDA + activity pattern features; expect to iterate | Pilot validation only in Phase 1; do not deploy as clinical decision support without Phase 2 validation |
| VA benefits eligibility classifier | Rules-based engine cross-referenced against VA VASRD and CFR Title 38; update quarterly | 99%+ accuracy on known-benefit test cases |

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

---

### Phase 2 Build Plan — Expansion (Months 31–54)

**Budget:** $280M  
**Primary deliverables:** NEXUS and ATLAS production, full fleet integration, 5,000-unit deployment, humanoid pilot, reimbursement pathway

#### NEXUS Development (Months 31–42)

NEXUS is the most mechanically complex archetype due to its articulated arms and medication dispensing requirements.

- Hardware: Select or commission a wheeled bedside platform with two 3 DOF soft-robotic arms. Evaluate commercial options (e.g., Hello Robot Stretch, or custom build on mobile base). Key requirements: safe force limits (ISO/TS 15066 for collaborative robotics), FDA 510(k) pathway consideration for the medication dispensing module.
- **FDA pathway:** The smart medication dispenser module likely requires FDA 510(k) clearance as a Class II medical device. Begin pre-submission meeting with FDA in Month 31; plan 18–24 months for clearance. Deploy Phase 2 NEXUS units with dispensing module in a non-dispensing monitoring-only mode until clearance is received.
- Integrate TENS therapy delivery arms, heat/cold pad dispensers, hearing support array, and AI vision system modules.
- Prosthetic interface coordinator: partner with two commercial prosthetic manufacturers (e.g., Ottobock, Össur) for Bluetooth SDK access and calibration API.
- Validate fall detection via floor pressure mat in a 30-unit home trial before broad deployment.

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

---

### Phase 3 Build Plan — Scale (Months 55–96)

**Budget:** $800M+  
**Primary deliverables:** 50,000-unit national deployment, PHALANX production, open API, transfer pool operations, cost reduction to $18,000–$24,000/unit

#### PHALANX Development (Months 55–66)

PHALANX is the most operationally challenging archetype due to outdoor autonomy requirements.

- Hardware: Ruggedized wheeled outdoor platform. Requirements: IP65 weather resistance, GPS + LiDAR + stereo cameras, 8-hour outdoor battery life, curb-climbing capability. Evaluate platforms: Clearpath Husky, Boston Dynamics Spot (for -H variant), or custom outdoor UGV.
- Outdoor autonomy stack: build on ROS 2 Nav2 as baseline; extend with veteran-specific trigger-environment routing (PTSD trigger map must be updatable by veteran at any time; route re-planning must complete in under 10 seconds).
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
| Cybersecurity breach of veteran Tier-1 data | Low | Critical | FedRAMP High; on-device only processing for Tier-1; penetration test every 6 months; breach response plan maintained and rehearsed |

---

### Team & Hiring Plan

| Phase | Headcount (cumulative) | Key hires |
|---|---|---|
| Pre-Phase 0 | 25–35 | CTO, CMO, CPO, 5 WS leads, 4 senior engineers per WS, 2 clinical researchers |
| Phase 1 | 80–120 | Clinical AI engineers (×6), VA integration engineers (×4), IRB/regulatory specialist, field operations lead, 25 field technicians for pilot |
| Phase 2 | 200–280 | Mechanical engineers for NEXUS arms (×4), ATLAS software engineers (×6), humanoid robotics specialists (×4), reimbursement/health economics analyst, 100 field technicians |
| Phase 3 | 500–700 | Manufacturing partnerships team, open API developer relations, 330 regional field technicians, NOC operators (×20), refurbishment center staff (×60) |

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
└── docs/                # System vision, architecture decision records, policy briefs
```

For architectural questions, design decisions, or policy collaboration, open an issue with the label `architecture`, `policy`, or the relevant archetype name.

---

> *VALOR System Vision — Version 3.0*  
> *Claude AI was used in producing this system overview, README file, and build roadmap.*  
> *This document is a conceptual vision for public interest discussion and policy development. All cost figures are estimates based on published research. All technical capabilities described are based on existing or near-term commercially available technologies.*  
> *These veterans gave everything. VALOR's mission is to give something back that matches the scale of what they carry — a system that is as persistent, as adaptive, and as committed as they are.*
