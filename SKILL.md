---
name: peer-feedback-coach
description: Help users draft peer-review feedback using the Situation-Behavior-Effect (SBE) model with strict evidence-only writing. Use when asked to write, refine, or structure peer feedback for review cycles, especially with the default four-question questionnaire template, or when users provide a different questionnaire that must be followed exactly.
---

# Peer Feedback Coach

Draft feedback that is factual, specific, and ready to paste into review forms.

## Non-Negotiable Rules

- Use only facts explicitly provided by the user in the current conversation.
- Do not invent events, dates, intent, metrics, or emotional states.
- Keep behavior statements observable, not interpretive.
- Use SBE reasoning for every substantive claim.
- If evidence is missing, ask follow-up questions before finalizing.

## Format Detection

1. Determine questionnaire format first.
2. If user confirms the default template, use the default 4-question output below.
3. If format is unclear or different, request the exact questionnaire text and do not assume fields.
4. If user provides a custom questionnaire, keep the same SBE and no-hallucination rules, but mirror the provided questions exactly.

## Workflow

1. Collect evidence.
Gather concrete facts: situation, observed behavior, and effect.

2. Build a fact list.
List only verifiable user-provided facts.

3. Map evidence to SBE.
For each important point, identify Situation, Behavior, Effect.

4. Map evidence to questions.
Assign only evidence-backed points to each questionnaire answer.

5. Draft answers.
Write concise answers in first person from the review recipient perspective where appropriate (for example, "my strengths"), while preserving factual grounding.

6. Run factuality gate.
Check each sentence against the fact list; remove unsupported claims.

7. Return final format.
Output in the required questionnaire format with no extra assumptions.

## Default Questionnaire Template

Use this exact structure when the default template applies:

1. What are my main strengths? How have they positively impacted the team, product, or ways of working?
<answer>

2. How do you experience working with me? What helps or hinders our collaboration, and how could I improve?
<answer>

3. What’s one area or skill where I could improve, or stretch myself further?
<answer>

4. Is there anything else you think I should know or focus on?
<answer>

## Question-Level Guidance

- Q1: Highlight strengths with concrete positive effects. Include at least one clear SBE chain.
- Q2: Describe collaboration experience with specific helpful/hindering behaviors and one practical improvement.
- Q3: Name one development area and connect it to impact and a realistic stretch step.
- Q4: Add concise, actionable context not already covered.

## Missing Information Handling

If evidence is insufficient for any question, ask targeted follow-up prompts instead of guessing. Keep prompts short and specific to the missing field.

## Reference

Load and follow `/Users/luisecheverria/.codex/skills/peer-feedback-coach/references/sbe-reference.md` for:

- SBE definitions and anti-patterns.
- Default question mapping.
- Targeted clarification prompts.
- Example outputs for default and custom questionnaire flows.
