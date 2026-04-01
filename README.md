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
15. [Financial Case & ROI](#financial-case--roi)
16. [Policy Framework](#policy-framework)
17. [Contributing](#contributing)

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
| Housing stability system | Monitors lease dates, utility bills, benefit payment schedules; auto-files for emergency housing assistance; maintains encrypted document vault for housing applications |
| Veteran peer network connector | Matches veteran with peer support specialists sharing similar MOS, diagnosis, or life situation; facilitates encrypted group discussions |

**Key integration:** ATLAS receives social engagement trend data from SENTINEL (isolation early warning) and shares housing stability signals with HERALD (emergency benefits filing trigger).

---

### HERALD — Benefits, Administration & Financial Guardian

**Nickname:** "The Advocate"  
**Domain:** Full-stack VA navigation, financial management, and bureaucratic representation  
**Form factor:** Compact desktop unit with 12-inch display, high-resolution document scanner, speaker-microphone for secure video calls with VA representatives and attorneys; optional mobile rolling base

**Capability modules:**

| Module | Description |
|---|---|
| VA benefits navigator | Knows all 130+ VA benefit programs; auto-fills forms (VA 21-526EZ, 10-10EZ, etc.); tracks claim status via VA API in real time; flags unclaimed eligible benefits |
| Claims appeal automation | When a claim is denied, auto-generates appeal documents, requests C&P exam scheduling, and alerts VSO/attorney partner |
| Financial stability coach | Tracks VA benefit deposits, disability pay, and pension; flags fraudulent charges; auto-pays bills in priority order; models debt repayment plans |
| Document vault | Encrypted storage of DD-214, discharge papers, medical records, financial documents, and housing leases; auto-syncs from smart mail scanner |
| Appointment manager | Schedules and sends reminders for all VA appointments across medical, mental health, vocational rehab, and specialty care; integrates with VA scheduling API |
| Insurance interoperability | Coordinates VA, Medicare, Medicaid, and private insurance claims to minimize veteran out-of-pocket costs |
| Legal referral system | Identifies cases warranting VA-accredited attorney representation; connects to nonprofit legal aid partners and Volunteers of America advisors |

**Key integration:** HERALD is a pure enabler hub — it receives trigger signals from all other robots (missed medication → pharmacy refill; depression threshold → appointment scheduling; housing alert → benefits filing) and takes administrative action automatically.

---

### PHALANX — External Environment & Safety Scout

**Nickname:** "The Scout"  
**Domain:** Outdoor navigation support, environmental monitoring, and emergency response  
**Form factor:** Ruggedized outdoor wheeled unit; weatherproof; LiDAR array + stereo cameras; 4G/5G connected; pedestrian-pace movement; low-profile chassis; 8-hour active escort battery life  
**Humanoid option:** See [Humanoid Robot Options](#humanoid-robot-options) — PHALANX-H variant provides visible deterrence in public environments and more natural side-by-side walking cadence for veterans with mobility or anxiety needs

**Capability modules:**

| Module | Description |
|---|---|
| Outdoor mobility escort | Accompanies veteran on walks; monitors physiological stress in public environments; real-time obstacle and crowd detection |
| Driving assistance integration | Syncs with veteran's vehicle for pre-trip stress assessment; if PTSD or TBI symptoms are elevated, suggests alternative transport |
| Emergency response coordinator | If veteran falls or is in crisis outdoors, contacts emergency services, shares GPS location, and provides first-responder briefing on veteran's medical history |
| Environmental trigger detection | Identifies documented PTSD triggers (loud noises, crowds, specific sensory stimuli) and provides advance warning or alternate route suggestion |
| Field medication reminder | Delivers reminders and motivational check-ins during outdoor activities based on veteran's schedule |
| Community resource mapping | Real-time overlay of nearby VA clinics, pharmacies, peer support centers, and veteran-friendly businesses during navigation |

**Key integration:** PHALANX shares real-world stress exposure data with SENTINEL (outdoor trigger logging) and mobility data with NEXUS (joint planning for veterans with physical limitations).

---

## Humanoid Robot Options

Each VALOR archetype is available in a **humanoid variant** (suffixed `-H`) for veterans who prefer or benefit from interaction with a robot that has a recognizable human form. This is an elective configuration choice made during onboarding and adjustable at any time.

> **Design philosophy:** Humanoid form is not the default because many veterans find non-humanoid robots less anxiety-inducing and less socially complex. However, for veterans whose primary needs involve physical interaction, social presence, or reduced loneliness, the embodied human form significantly improves engagement and perceived connection.

### Humanoid Variant Specifications

| Archetype | Humanoid Variant | Form Factor | Primary Advantage |
|---|---|---|---|
| SENTINEL | SENTINEL-H | Seated or standing companion (~1.4–1.7m); expressive face with limited affect display; soft outer shell | Reduces emotional distance during crisis intervention; more natural for grounding exercises and guided breathing |
| NEXUS | NEXUS-H | Standing clinical assistant (~1.6m); articulated arms rated for 10 kg assist; stability rails integrated | Physical therapy guidance through natural mirroring; more intuitive for veterans performing exercises or transfers |
| ATLAS | ATLAS-H | Social companion form (~1.5m); designed for side-by-side sitting and shared activity | Significantly reduces reported loneliness; more engaging for extended conversation; natural at shared meals or recreational activities |
| PHALANX | PHALANX-H | Walking escort form (~1.6m); weather-hardened; pedestrian-cadence gait | Side-by-side walking is more natural than wheeled escort; provides visible safety presence in public; veterans with anxiety report reduced stress |
| HERALD | HERALD-H | Desktop-anchored with humanoid upper body; not ambulatory | More engaging for extended administrative sessions; voice and gesture improve document interaction |

### Humanoid Variant Selection Guidance

Veterans and their VA care teams can use the following criteria when choosing between standard and humanoid variants:

- **Recommend standard form factor when:** veteran has hypervigilance or startle responses likely to be triggered by human-like movement; veteran's primary needs are clinical or administrative; veteran explicitly prefers minimal social interaction with the robot
- **Recommend humanoid variant when:** veteran's primary challenge is social isolation or loneliness; veteran is elderly and has prior experience with human caregivers; veteran's physical rehabilitation involves demonstration and mirroring; veteran indicates preference during intake

> **Note on uncanny valley:** All VALOR-H humanoid variants are designed to be clearly robotic in surface finish — they do not attempt to pass as human. This is intentional. Research on robot-human interaction consistently shows veterans prefer honest, clearly-robotic humanoid forms over high-fidelity simulations of human appearance. VALOR-H variants use matte surfaces, visible panel joints, and abstracted facial features to remain recognizably robotic while still conveying warmth and intentionality.

---

## Inter-Robot Communication

All five robots communicate via an **encrypted local mesh network** when within range (~100 meters), falling back to cloud relay via VALOR-CORE when separated.

**Message types:**

| Type | Description |
|---|---|
| `STATE_BROADCAST` | Continuous low-bandwidth updates of each robot's sensor readings to all fleet members |
| `ALERT_ESCALATION` | High-priority events requiring coordinated fleet response (e.g., SENTINEL detects crisis-level depression → all robots shift to supportive mode) |
| `RESOURCE_HANDOFF` | When a capability required by one situation spans two robots (e.g., SENTINEL identifies medication-related mood issue → hands off to NEXUS for dispensing review) |
| `CONTEXT_UPDATE` | Any new information about the veteran (new diagnosis, new prescription, new life event) is immediately propagated to all fleet members via VALOR-CORE |

**Network topology:**
```
SENTINEL ─── VALOR-CORE (cloud) ─── HERALD
   │                │                  │
NEXUS ──────────────┼────────────── ATLAS
   │                │
PHALANX ────────────┘

Local mesh (100m range) + cloud relay fallback
Encryption: AES-256 at rest, TLS 1.3 in transit
```

---

## Cascade Prevention — How the Fleet Works Together

The most powerful VALOR capability is coordinated cascade prevention — detecting a problem in one domain before it triggers failures in downstream domains.

### Scenario 1: PTSD → Sleep → Depression cascade

**Without VALOR:** Nightmare at 2:00 AM → chronic sleep loss → depression deepens → veteran stops answering calls → misses VA appointment → prescription lapses → crisis.

**With VALOR:**
1. **Night 1** — NEXUS detects sleep disruption; SENTINEL detects elevated cortisol proxy and delivers calming soundscape + breathing prompt
2. **Morning** — SENTINEL notes elevated baseline stress; HERALD confirms upcoming VA appointment and sends 48-hour reminder
3. **Day 3** — SENTINEL's mood model detects early depression indicators; ATLAS schedules peer support video call
4. **Day 5** — NEXUS notes medication adherence slipping; HERALD auto-contacts VA pharmacy for early refill
5. **Week 2** — Veteran reports feeling better; cascade interrupted at step one

### Scenario 2: Addiction → Financial → Homelessness cascade

**Without VALOR:** Relapse → missed work → job loss → VA benefits lapse → savings depleted → eviction → street homelessness.

**With VALOR:**
1. **Relapse event** — SENTINEL detects physiological craving signal; connects veteran to peer sponsor immediately
2. **HERALD** — detects VA disability recertification due in 30 days; auto-prepares form
3. **ATLAS** — detects reduced social engagement (relapse indicator); schedules peer check-in
4. **HERALD** — monitors bank account; flags low funds 12 days before rent; auto-submits emergency housing assistance application; books financial counselor
5. **Outcome** — veteran retains housing, benefits maintained, recovery continues

---

## Robot Transfer & Reassignment Protocol

VALOR robots are assigned to individual veterans, but life circumstances sometimes require physical units to be moved to a different veteran. The Transfer & Reassignment Protocol governs this process to protect both the outgoing and incoming veteran's privacy, preserve the incoming veteran's onboarding experience, and ensure no capability gap occurs during the transition.

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
| 15 | Medication management | NEXUS | Physical |
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

> *VALOR System Vision — Version 2.0 Draft*  
> *Claude AI was used in producing this system overview and README file*  
> *This document is a conceptual vision for public interest discussion and policy development. All cost figures are estimates based on published research. All technical capabilities described are based on existing or near-term commercially available technologies.*  
> *These veterans gave everything. VALOR's mission is to give something back that matches the scale of what they carry — a system that is as persistent, as adaptive, and as committed as they are.*
