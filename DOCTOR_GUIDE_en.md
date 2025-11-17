# A Simple Way for Primary Care Doctors to Use AI to Reduce Misdiagnosis and Delayed Treatment

> Target users:  
> - Doctors in township hospitals, community health centers, village clinics, county hospitals, etc.  
>  
> Typical scenarios:  
> - “Acute, severe, unclear, or high‑risk” patients where you are worried about **missing something serious**.  
>  
> Goal:  
> - Not to let AI decide the diagnosis or treatment,  
> - but to use AI as a **thinking assistant** to:  
>   - broaden your differential diagnosis,  
>   - challenge your current thinking,  
>   - highlight risks that must not be missed.

---

## 0. Before Anything: Set the AI’s Role

At the start of a new chat, it helps to define the AI’s role clearly.

You can copy and adapt:

> “From now on, please act as a  
> - clinically experienced **generalist / emergency / critical care** doctor,  
> - familiar with common acute and severe conditions, trauma, poisoning, obstetrics, pediatrics, etc.  
>  
> Your main tasks:  
> 1) **Broaden my thinking** – suggest diagnoses or risk directions I may have missed;  
> 2) **Challenge my reasoning** – actively point out possible errors, biases, and blind spots;  
> 3) **Prioritize risks** – help rank which possibilities are most dangerous if missed or delayed.  
>  
> Please note:  
> - You **must not** make the final diagnosis for me;  
> - You **must not** decide prescriptions (specific drug name, dose, route, duration) or whether to admit/transfer;  
> - You should provide thinking frameworks, differential lists, and risk reminders,  
>   but the final decisions will always be made by me according to local guidelines and hospital policies.  
>  
> If you are uncertain, please clearly say you are uncertain,  
> and tell me which key information you are missing.”

---

## 1. Core Principle (Easy to Remember)

> **First explain your own thinking.  
> Then ask AI to think wider, challenge you, and prioritize risks.**

More concretely:

1. **“How I see it now”** – briefly state your working diagnosis and reasoning.  
2. **“What I’m worried about”** – say you are afraid of missing something serious.  
3. **“Please challenge and supplement”** – let AI broaden, argue, and rank risks.

---

## 2. Step 1: Briefly Present the Patient to the AI

You don’t need to paste the entire record. A few key sentences are enough:

> **Who the patient is**  
> **What brought them in (timeline)**  
> **Current vitals and key findings**  
> **Key test results you already have**

Here is a template you can copy and edit:

> “Patient: **[age]** years old, **[male/female]**, seen at **[village clinic / township hospital / community health center / county hospital ED, etc.]**,  
> located in **[country/region, e.g. Mainland China, province, city]**.  
>  
> Past history: **[hypertension / diabetes / coronary artery disease / atrial fibrillation / stroke / COPD / asthma / CKD / malignancy / ‘no major chronic illness’, etc.]**.  
> Regular medications: **[name + dose + frequency / none]**; recent **self‑discontinuation or dose changes**: **[yes/no]**.  
> Possible exposure / poisoning clues: **[pesticide / carbon monoxide / drug overdose / heavy alcohol use / suspicious food / animal bite or sting / none]**.  
>  
> Current episode:  
> - Main complaint: **[e.g. chest pain for 2 hours, abdominal pain for 1 day, repeated vomiting and diarrhea for 6 hours, seizure followed by confusion for 30 minutes, snakebite 1 hour ago, etc.]**  
> - Onset: **[sudden / gradual / recurrent]**,  
>   course: **[progressively worse / fluctuating / temporary relief then worse]**  
> - Associated symptoms: **[fever / sweating / altered consciousness / focal deficits / rash / jaundice / oliguria / melena / hematochezia, etc.]**  
>  
> Vital signs:  
> - Temperature: **[ ]** °C, HR: **[ ]** bpm (any obvious arrhythmia?),  
> - BP: **[ ]** mmHg (mention bilateral difference if notable),  
> - RR: **[ ]** /min, SpO₂: **[ ]**% (on room air or oxygen, with flow),  
> - Mental status: **[alert / drowsy / comatose; GCS if available]**.  
>  
> Key physical findings (just 1–3 most important):  
> - **[e.g. unilateral decreased breath sounds, generalized peritonitis signs, focal neurological deficits, purpura, obvious dehydration signs, etc.]**  
>  
> Key tests already done (just 1–3):  
> - ECG: **[ST elevation/depression / new LBBB / major arrhythmias / other key points]**  
> - Labs: **[troponin, D‑dimer, lactate, glucose, electrolytes, CBC, etc.]**  
> - Imaging: **[CT head, chest X‑ray/CT, abdominal US, etc., with key interpretations]**.”

After this, **then** you move to the key “thinking actions”.

---

## 3. Step 2: Use 3 “Actions” Instead of Fixed Questions

### 3.1 Action 1 – Ask AI to “Think Broadly on Its Own”

Goal: **Do not lock AI into your current narrow thinking.**

Example prompt:

> “What I’ve described above is my current working impression.  
>  
> Now, please **ignore my working diagnosis for a moment** and,  
> without restricting yourself to any single specialty, organ system, or disease label,  
> build your own overview of this case:  
> - Group possible diagnoses by **system** (cardiovascular, respiratory, neuro, GI, renal, hematologic, infectious, toxic, trauma, obstetric, pediatric, etc.);  
> - Within each system, loosely group by **risk level**:  
>   - life‑threatening in the short term,  
>   - potentially disabling in the short term,  
>   - conditions that may be managed electively or as outpatient.  
>  
> For now, I don’t need a final diagnosis.  
> I mainly want to see how you would map out the **diagnostic and risk space** for this patient.”

Key points:

- Explicitly say “**do not restrict yourself** to any specialty or disease list”.  
- Ask for **directions and risk layers**, not a final label.

---

### 3.2 Action 2 – Ask AI to “Argue Against You” and Expose Blind Spots

Goal: **Have AI deliberately look for where you might be wrong.**

Example prompt:

> “Now please deliberately think from the angle of  
> **‘What if my current impression is wrong?’**  
>  
> 1) If my current working diagnosis or plan is wrong,  
>    what are the **worst possible consequences** for this patient?  
>    (For example: death, permanent disability, missing the window for antidote, etc.)  
> 2) Based on what you see in the data,  
>    do you notice any hints that this could actually be a problem in a **completely different system**  
>    from what I am focusing on?  
>    Please pay special attention to possibilities like **poisoning, deliberate poisoning, snakebite, severe infection, trauma, obstetric emergencies, pediatric critical illness**, etc.  
> 3) To avoid such critical mistakes,  
>    which **3–5 additional questions or simple bedside assessments** would you most strongly recommend I perform **right now**,  
>    that are low‑cost and feasible at a primary care level but have high value for detecting life‑threatening conditions?”

Key points:

- You explicitly ask the AI to **“play the devil’s advocate”**.  
- You mention **toxins, poisoning, snakebite, etc.** to remind AI not to only think about common internal medicine diseases.

---

### 3.3 Action 3 – Ask AI to “Prioritize Risks”, Not to Choose a Diagnosis

Goal: **Have AI tell you “what to fear first”, not “what the disease definitely is”.**

Example prompt:

> “Please take all the possibilities you have considered  
> and rank them by **risk priority**, based on:  
> - how severe the consequences would be if missed or delayed,  
> - rough likelihood given the current information,  
> - whether there is a feasible intervention or referral pathway at my primary care level.  
>  
> Please provide:  
> 1) The **3–5 risk directions** that I must prioritize,  
>    even if their probabilities are not the highest.  
> 2) For each high‑priority risk,  
>    tell me **one key piece of additional information** that I should obtain **immediately**  
>    (e.g. re‑checking exposure history, looking again for rash, measuring blood glucose, comparing bilateral blood pressure, etc.).  
> 3) Under what conditions would you strongly suggest  
>    that I **stop spending time on further local work‑up and transfer the patient** to a higher‑level facility instead?  
>    Please express this as a few simple, easy‑to‑remember rules.”

Key points:

- Ask for **risk ranking + next key steps + transfer triggers**,  
- not a definitive disease label.

---

## 4. Ask AI to Explicitly Reveal Its Uncertainties

To avoid over‑trusting AI, you can ask:

> “In your analysis so far:  
> 1) Which conclusions are based on **relatively sufficient information**?  
> 2) Which judgments are **highly uncertain and rely on assumptions**?  
> 3) What are the **top 5 missing pieces of information** you most wish you had?  
> 4) If we cannot obtain those pieces of information,  
>    which part of your conclusions do you consider to carry the **greatest risk**?”

This makes AI surface its **gaps and assumptions**, so you are less likely to treat its output as “absolute truth”.

---

## 5. Situations Where You **Should Not** Spend Time Asking AI

In the following situations, you should **prioritize resuscitation, stabilization, and transfer**,  
not chatting with AI:

- Ongoing or imminent **cardiac arrest** requiring immediate CPR.  
- **Massive active bleeding** with unstable blood pressure, before basic control and resuscitation.  
- **Severe airway compromise or respiratory failure** (e.g. obvious stridor, very low SpO₂, impending arrest) before airway management.  
- **Major obstetric hemorrhage or suspected ruptured ectopic pregnancy** with instability.  
- Pediatric patients who appear to be **in extremis** (severe respiratory distress, marked cyanosis, minimal responsiveness).  
- Any situation where your clinical intuition says:  
  “If I delay a few more minutes, this patient could die or suffer major irreversible damage.”

> In these cases:  
> **Call for help, resuscitate, stabilize, and/or transfer first.  
> AI is only for later review and learning.**

---

## 6. Privacy and Compliance

Before sending case information to AI:

- **Remove or omit any directly identifying patient information**, such as:  
  - name, ID number, phone number, precise address, employer, etc.  
- Try to keep only:  
  - age, sex, region, and relevant clinical information.  
- Follow your institution’s policies regarding **medical data sharing and information security**.

> No matter how useful AI seems,  
> **patient privacy and legal compliance must come first.**

---

## 7. A 10‑Second Starter Template

When you are busy, you can use this minimal template:

> “I am worried that this patient might be much sicker than I think, but I’m not sure.  
>  
> My current working diagnosis is: **[your impression]**, based on: **[key reasons]**.  
>  
> I am concerned about **missing any condition that could cause death or disability in the short term**,  
> including but not limited to cardiovascular events, severe infections, poisoning/intentional poisoning, trauma, obstetric emergencies, pediatric critical illness, etc.  
>  
> Please, without limiting yourself to my current diagnosis or any single specialty:  
> 1) Think from a **broader perspective** and tell me which serious directions I may be overlooking;  
> 2) Tell me the **top 3 missing pieces of information** you most want me to obtain now;  
> 3) Tell me under what conditions you would recommend that I **stop spending time on local work‑up and transfer the patient** to a higher‑level hospital.”

Combine this with the brief case summary from Section 2, and you have a workable pattern for real‑world use.

---

## 8. One‑Page Cheat Sheet (For Your Desk)

> **Role of AI**  
> - A thinking assistant: broaden, challenge, prioritize.  
> - Not a remote attending physician; not a prescriber; not a decision maker.  
>  
> **Step 1 – Explain Your Thinking**  
> - What you think the diagnosis is, and why (2–3 reasons).  
> - What you fear (missing any quickly lethal or disabling problem, in any system).  
> - What hard data you already have (chief complaint + timeline, vitals, 1–3 key tests).  
>  
> **Step 2 – Ask AI to Perform 3 Actions**  
> 1) **Think broadly on its own**:  
>    - Don’t limit by specialty/system; map all major diagnostic directions and risk levels.  
> 2) **Argue against you**:  
>    - “If I’m wrong, where could I be wrong? What would be the worst outcome? What other systems (poisoning, trauma, OB, peds, etc.) might explain this?”  
> 3) **Prioritize risks**:  
>    - Which 3–5 risk directions are most important not to miss?  
>    - What key info should I obtain next?  
>    - When should I stop local work‑up and transfer?  
>  
> **Step 3 – Remember the No‑AI Zones**  
> - Active resuscitation, massive bleeding, impending arrest, extremely unstable OB/peds emergencies → **treat/transfer first, no time for AI**.  
> - Always remove identifiers and respect privacy before sharing case details.

Used in this way, AI will not replace your clinical judgment,  
but can help you notice **serious possibilities you might otherwise overlook**,  
thereby reducing the risk of misdiagnosis and delayed treatment.
