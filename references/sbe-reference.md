# SBE Reference

## 1. SBE Model

Use Situation-Behavior-Effect to ground every claim.

- Situation: Where and when the behavior occurred.
- Behavior: Observable action (or missing action), not inference.
- Effect: Impact on team, product, delivery, or ways of working.

### SBE Anti-Patterns

- Avoid mind-reading ("you did this because...").
- Avoid personality labels ("you are careless").
- Avoid unsupported absolutes ("always", "never").
- Avoid adding details the user did not provide.

## 2. Questionnaire Routing

1. Use the default template when the user confirms that format.
2. If format is unclear, ask for exact questionnaire text before final draft.
3. If user provides a different questionnaire, mirror it exactly.
4. Keep SBE and no-hallucination constraints in all formats.

## 3. Default Question Mapping

### Q1
Question:
"What are my main strengths? How have they positively impacted the team, product, or ways of working?"

Include:

- 1-3 strengths backed by observable examples.
- Explicit positive impact per strength.
- At least one SBE chain.

If missing, ask:

- "Which specific situation best shows this strength?"
- "What concrete impact did it have on team/product/ways of working?"

### Q2
Question:
"How do you experience working with me? What helps or hinders our collaboration, and how could I improve?"

Include:

- Concrete collaboration behaviors that help.
- Concrete behaviors that hinder (if applicable).
- One practical improvement suggestion.

If missing, ask:

- "What behavior helped collaboration most?"
- "Was there a behavior that made collaboration harder?"
- "What specific improvement would be most useful?"

### Q3
Question:
"What’s one area or skill where I could improve, or stretch myself further?"

Include:

- One development area only.
- Why it matters (effect).
- One realistic stretch action.

If missing, ask:

- "Which single skill area would create the biggest improvement?"
- "What impact would improving this area have?"

### Q4
Question:
"Is there anything else you think I should know or focus on?"

Include:

- Concise additional signal not repeated from Q1-Q3.
- Clear focus suggestion when appropriate.

If missing, ask:

- "Any additional context or priority you want included?"

## 4. Evidence Contract (No Hallucinations)

Apply these checks before final output:

1. Build fact list from user input only.
2. Map each answer sentence to one or more facts.
3. Remove or rewrite unsupported claims.
4. Label uncertainty explicitly.
5. Ask follow-up questions rather than filling gaps.

## 5. Quality Checklist

Confirm all items:

- Output follows the required questionnaire format exactly.
- Each answer is specific and evidence-backed.
- SBE reasoning is present in substance.
- Suggestions are practical and respectful.
- No fabricated details appear.
- The response is concise enough for HR text areas.

## 6. Example Trigger Prompts

- "Use the default template and draft my peer-review answers from these notes."
- "Turn this feedback into the four HR questions with SBE grounding."
- "I have a different questionnaire format; ask me for the questions first."
- "Rewrite these answers to be more factual and less opinion-based."

## 7. Example Output (Default Template)

Facts Used:

- In Q1 planning, the person flagged dependency risks early.
- Team reduced rework on two features.
- In two recent sprints, blockers were raised late.
- Late blocker visibility increased release-week pressure.
- Person gives clear async updates in Slack.

Final Draft:

1. What are my main strengths? How have they positively impacted the team, product, or ways of working?
You consistently raise dependency risks early in planning and provide clear async updates in Slack. In Q1 planning sessions, you flagged risks before implementation, which helped the team adjust scope early and avoid rework on two features.

2. How do you experience working with me? What helps or hinders our collaboration, and how could I improve?
Working with you is effective when updates are shared early and clearly, because it improves alignment and reduces back-and-forth. Collaboration is harder when blockers surface late in the sprint, since it compresses QA and increases release-week pressure. A useful improvement would be to raise blockers as soon as they appear and flag risk one day earlier in status updates.

3. What’s one area or skill where I could improve, or stretch myself further?
A strong growth area is earlier risk communication during execution, especially around blockers. Improving this would reduce late sprint pressure and help planning stay predictable. A practical stretch is to add a brief risk check in daily updates and escalate blockers within the same day.

4. Is there anything else you think I should know or focus on?
Continue pairing your strong proactive planning with earlier in-sprint escalation. That combination can improve both delivery confidence and team workload balance.

## 8. Example Output (Format Unclear)

Before drafting final feedback, ask:

- "Please share the exact questionnaire format you need me to fill."
- "If this is not the default template, paste each question in order."
- "Any length or tone constraints I should follow for each answer?"
