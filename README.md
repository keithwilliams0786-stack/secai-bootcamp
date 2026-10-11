# SecAI+ (CY0-001) Bootcamp

Free, open-source (MIT), self-contained study tools for the **CompTIA SecAI+ (CY0-001)** certification exam: an interactive bootcamp console and a narrated video course. You don't need an account or a server, and no data leaves your browser.

**▶ Live site:** https://keithwilliams0786-stack.github.io/secai-bootcamp/

| | |
|---|---|
| **Bootcamp console** | [`secai-bootcamp.html`](https://keithwilliams0786-stack.github.io/secai-bootcamp/secai-bootcamp.html): lessons, practice tests, PBQ simulators, readiness tracking |
| **Video course** | [`secai-video-course.html`](https://keithwilliams0786-stack.github.io/secai-bootcamp/secai-video-course.html): 28 narrated episodes with synced captions |
| **Landing page** | [`index.html`](https://keithwilliams0786-stack.github.io/secai-bootcamp/) |

---

## What's inside

### 5-Day Readiness Bootcamp (`secai-bootcamp.html`)

**Lessons**
- 47 lecture and lab blocks covering all four exam domains and all 15 sub-objectives, laid out as a Mon–Fri, 8-hours-a-day schedule
- Gap-review sections added to the topics most often missed in practice (AI tool selection, ML techniques, data integrity, privacy tech, threat modeling, gateway controls, model attacks)
- Objective tracker for self-rating each sub-objective

**Question bank: 376 original items**
| Pool | Questions | Matching sets | PBQs |
|---|---|---|---|
| Regular bank | 277 | 9 | 6 |
| Locked reserve | 78 | 3 | 3 |

- Item types: single-answer multiple choice, multi-select ("Select two/three", scored all-or-nothing), term-to-definition matching with a decoy, and performance-based questions
- Every wrong option has its own explanation, so the review screen tells you *why* each choice is wrong, not just which answer is right
- Items are tagged by objective and concept, which drives the weak-area targeting

**Practice tests and exams**
- **Practice test:** 60 items in 60 minutes. Question order and answer order are reshuffled on every appearance, items you haven't seen come up first, and each test includes 3 PBQs and 2 matching sets, weighted to the exam blueprint
- **Strict timer** with a pace indicator; the test auto-submits when time runs out
- **Domain drills** and an untimed **weak-topic drill** that gives instant feedback
- **Weak-areas final:** unlocks once you've seen every item in the regular bank. It draws only from the locked reserve, weighted toward the topics you miss most
- **Balanced fresh mock:** a full-length test drawn mostly from reserve items you've never seen
- Results separate first-attempt accuracy from repeat accuracy, so memorized answers don't inflate your score

**Readiness tracker:** a 7-point go/no-go checklist
1. Every item in the regular bank seen at least once
2. Last 3 practice tests averaging ≥ 90%
3. First-attempt accuracy ≥ 85%
4. Last practice test finished, all items answered, with ≥ 5 minutes left
5. Weak-areas final ≥ 85%
6. Balanced fresh mock ≥ 90%
7. Brain dump recalled at ≥ 90% in about 2 minutes, twice

**PBQ simulators**
- Tool selection (multi-part mapping)
- Attack / evidence / control tables
- Policy rule-action builders
- Architecture controls (place each control on the right layer, edge to model), with partial credit
- Framework sort (OWASP Top 10, OWASP LLM Top 10, STRIDE)

**Study tools and games**
- 159-card flashcard deck and a 16-pair attack↔control matching drill
- **Brain-dump sheet** plus a timed 2-minute recall drill, for the exam tutorial window, which doesn't count against your 60 minutes
- Games: Defend the Pipeline, Jeopardy Board, Wheel of Security (sound toggle included)

### Narrated Video Course (`secai-video-course.html`)

- **28 episodes:** an intro, one episode per sub-objective, 10 gap-review episodes on the most-missed topics, and a closing exam-strategy / go-no-go episode
- Captions highlight in sync with the narration
- Play/pause, slide skip, playback speed, voice picker, and autoplay to the next episode
- Uses your device's built-in text-to-speech, so there are no audio files to download. Without a voice, it falls back to a paced, captioned slideshow
- Made for listening while driving, working out, or away from a screen

---

## Exam coverage

| Domain | Sub-objectives |
|---|---|
| 1. Basic AI Concepts Related to Cybersecurity | 1.1 – 1.3 |
| 2. Securing AI Systems | 2.1 – 2.6 |
| 3. AI-assisted Security | 3.1 – 3.3 |
| 4. AI Governance, Risk, and Compliance | 4.1 – 4.3 |

Domain 2 is the largest share of the exam, and the bootcamp's time and question weighting follow that.

**Sources:** Content is cross-checked against the official Sybex/Wiley *CompTIA SecAI+ Study Guide* (Mike Chapple and Fred Nwanganga) and gap-checked against a full CompTIA CertMaster run. **Every question, scenario, and PBQ in this repo is original.** No CertMaster or study-guide question text is reproduced.

---

## Using it

**Online:** open the [live site](https://keithwilliams0786-stack.github.io/secai-bootcamp/).

**Offline:** download or clone the repo and open any `.html` file in a browser. Each page is a single self-contained file with no build step and no dependencies. Fonts load from Google Fonts when you're online and fall back to system fonts otherwise.

```bash
git clone https://github.com/keithwilliams0786-stack/secai-bootcamp.git
cd secai-bootcamp
# then open index.html in your browser
```

**Suggested study loop**
1. Work through the bootcamp days, or listen to the matching video episodes.
2. Take practice tests until bank coverage hits 100% (about 5 tests).
3. Drill your weak topics between tests.
4. Once your last three practice tests average 90% or better, take the weak-areas final, then the fresh mock.
5. Practice the brain dump until you can recall it in about 2 minutes.
6. Book the exam when every line of the readiness tracker is green.

---

## Privacy and progress

- Everything runs client-side. There are no accounts, analytics, or network calls beyond loading fonts.
- Progress is saved in your browser's `localStorage`, under:
  - `secai-bootcamp-progress-v1` for the console
  - `secai-video-progress-v1` for the video course
- Progress is per browser and per device. Clearing site data resets it.

---

## Repo layout

```
index.html                 Landing page
secai-bootcamp.html        Interactive bootcamp console (lessons, bank, tests, PBQs, games)
secai-video-course.html    Narrated video course
README.md
LICENSE                    MIT License
```

---

## License and reuse

Free to use, share, and adapt under the [MIT License](LICENSE). You can host it, fork it, translate it, add questions, or use it in a class or study group, including commercially. Just keep the copyright and license notice.

Contributions are welcome. If you spot a wrong answer key or an outdated fact, open an issue or a pull request with the question text and a source. Please keep any new questions original. Don't paste in text from CertMaster, the study guide, or other paid prep material.

---

## Changelog

**October 2026**
- The question bank grew from 97 to 376 items, including multi-select, matching, and PBQs, with per-option explanations
- New practice-test engine: shuffled questions and answers, unseen items first, strict timer with a pace indicator
- Added the readiness tracker, a locked reserve bank, the weak-areas final, and the balanced fresh mock
- New PBQ formats: tool selection, attack/evidence/control tables, and the policy rule builder. The architecture PBQ now gives partial credit
- Added the brain-dump sheet and timed drill
- Added 10 gap-review video episodes; video progress now saves reliably
- Content corrections:
  - STRIDE vs. the MIT AI Risk Repository causal taxonomy
  - Data lineage vs. provenance
  - Data balancing
  - CoE models (centralized / federated / hybrid)
  - Data scientist vs. data engineer roles
- The logo in each app now links back to the landing page

---

## Disclaimer

This is an independent study resource, not affiliated with or endorsed by CompTIA, Wiley/Sybex, or Pearson VUE. CompTIA, SecAI+, and CertMaster are trademarks of CompTIA, Inc. Check the current official CY0-001 exam objectives on [comptia.org](https://www.comptia.org/) before you test.

---

Built by [Keith Williams](https://github.com/keithwilliams0786-stack) with Claude. © 2026 CyberSentinel Services LLC, released under the [MIT License](LICENSE).
