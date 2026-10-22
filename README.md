# Mansi Agarwal

Clinical psychology researcher applying for PhD positions in quantitative and methods-focused psychology. My work is about measuring psychological change accurately, and about checking that an analysis method can be trusted before it is used on real participants.

**Current role:** Project Research Scientist-I, King George's Medical University (KGMU), Lucknow. I work on a multi-centre randomised controlled trial of psychosocial interventions for common psychological problems.

**Previous role:** Project Research Scientist-I, NIMHANS, Bengaluru. I set up trials and managed data for digital mental health research: REDCap builds, randomisation and multi-site participant onboarding.

**Education:** M.Sc. Clinical Psychology, Kristu Jayanti College, Bengaluru

## Research interests

- Measuring how a person's skill or psychological state changes over time
- Personalized algorithmic environments: whether systems that adapt to a person's responses still let researchers estimate what works
- Validity and reliability of psychological measures
- Using simulation to test a method before collecting data

## Projects

### [adaptive-assignment-recovery](https://github.com/MansiAgrwal/adaptive-assignment-recovery)

Personalized digital environments, such as adaptive learning platforms, recommender systems and digital health apps, choose what each person encounters next from their earlier responses. Can researchers still tell which experiences actually change people? This repository tests that question by simulating a personalized environment with a controlled rule-learning task.

What I found so far, in one simulated scenario: the choice of analysis model mattered more than whether the algorithm personalized. A model that ignored differences between fast and slow learners got the direction of the effect wrong. A model that allowed for those differences recovered the true effect, including under personalization. The next version will test whether this holds under more realistic conditions.

### [literature-evidence-pipeline](https://github.com/MansiAgrwal/literature-evidence-pipeline)

Notebooks for mapping a broad literature in a way that can be checked afterwards. The main search ran 153 pre-specified queries across 40 domains in OpenAlex and PubMed. Every paper is traced back to the query that found it, duplicates are merged only on exact matches, and screening queues are stratified so that counterevidence is not crowded out by highly cited papers.

### [personalized-feedback-reports](https://github.com/MansiAgrwal/personalized-feedback-reports)

Personalization in practice. I automated a digital mental-health study's hand-written feedback reports: the code turns each participant's questionnaire answers (K10 distress, coping strategies, and barriers to seeking help) into an individual Word report. The main work was finding the hard cases within the existing report structure before the logic was carried into a larger system for automating intervention delivery. The repository runs on synthetic data.

## Tools

R (lavaan; still developing) · Python (pandas, NumPy, python-docx) · OpenAlex and PubMed APIs · SPSS/AMOS · REDCap

---

All code here runs on simulated data or published literature records. No participant data from any study I have worked on is included.
