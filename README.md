# Savannah Tracker Report: AfyaTech AI Prompt Redesign

## Introduction
Precision in maternal health is not optional—it directly impacts outcomes for mothers and babies. Generic AI advice can mislead or exclude users. In rural Kenya and Uganda, effective AI must reflect real constraints such as distance to clinics, local diets, mobile money access, and community health systems.

---

## Prompt A: Nutrition Advice

### AIM Framework
- **Audience**: Pregnant women in rural Kenya and Uganda relying on staple foods like ugali, matooke, beans, and sukuma wiki.
- **Intent**: Provide practical, affordable, culturally relevant nutrition advice.
- **Mode**: SMS-friendly (≤160 words), simple English or Swahili, supportive tone.

### MAP Framework
- **Model**: Act as a rural maternal nutrition assistant familiar with East African diets. Avoid expensive or imported foods.
- **Action**: Generate 3–5 nutrition tips using local foods, including benefits for mother and baby.
- **Personalization**: Assume limited income, weekly market access, and reliance on staple foods.

### Final Prompt
“Provide 3–5 simple nutrition tips for a pregnant woman in rural Kenya or Uganda. Use locally available foods like ugali, matooke, beans, sukuma wiki, groundnuts, and small fish. Explain how each food helps mother and baby. Keep advice affordable and practical for someone shopping once a week. Write in clear, friendly SMS-style language.”

### Key Improvement
Reduces urban bias and prevents unrealistic recommendations by grounding outputs in local diets and economic realities.

---

## Prompt B: Appointment Reminders

### AIM Framework
- **Audience**: Pregnant women living more than 5 km from clinics, using walking, boda bodas, or community health workers.
- **Intent**: Improve clinic attendance through practical, actionable reminders.
- **Mode**: Concise SMS reminder with planning guidance.

### MAP Framework
- **Model**: Act as a maternal care coordinator familiar with rural clinic systems and community health workers.
- **Action**: Generate a reminder including appointment timing, travel planning, and fallback options.
- **Personalization**: Assume limited clinic availability, transport costs, and use of mobile money.

### Final Prompt
“Create an SMS reminder for a pregnant woman about her upcoming clinic visit. Include when to leave based on long travel distance, suggest transport options (walking or boda boda), and remind her to carry her clinic book and small mobile money funds if needed. If she cannot attend, suggest contacting her local community health worker.”

### Key Improvement
Improves real-world effectiveness by addressing travel, cost, and system constraints rather than giving a generic reminder.

---

## Prompt C: Emergency Triage

### AIM Framework
- **Audience**: Pregnant women with limited immediate access to hospitals.
- **Intent**: Provide safe, clear triage guidance without causing panic.
- **Mode**: Short, simple SMS-style instructions.

### MAP Framework
- **Model**: Act as a maternal health triage assistant using structured reasoning.
- **Action**: Ask 1–2 symptom questions, assess severity, and provide next steps.
- **Personalization**: Assume long distance to clinics and reliance on community health workers.

### Chain-of-Thought (Internal Reasoning)
1. Identify key symptoms  
2. Assess severity (urgent vs non-urgent)  
3. Select safest next action  

### Verifier Pattern
- Ensure no harmful or dismissive advice  
- Escalate urgent symptoms appropriately  
- Maintain calm and supportive tone  

### Final Prompt
“A pregnant woman reports feeling unwell. Ask 1–2 simple questions to understand symptoms (such as bleeding, severe headache, swelling, or fever). Based on the answers, give clear next steps: go to the nearest clinic immediately, contact a community health worker, or rest and monitor. Keep the tone calm and supportive, and avoid causing panic. Ensure urgent symptoms are treated seriously.”

### Key Improvement
Enhances safety and reliability by structuring reasoning and verifying outputs before responding.

---

## Reflection
This assignment shows that AI in healthcare must go beyond general knowledge to become context-aware and practical. In rural settings, factors like distance, cost, and cultural norms shape health decisions. Designing prompts with these realities in mind makes AI more useful and trustworthy. It also highlights that prompt design is not just technical—it directly affects health outcomes. Well-designed prompts can extend care access, while poor ones risk misinformation or exclusion. AI should support existing community health systems, not replace them, acting as a reliable assistant that improves decision-making and access to care.
