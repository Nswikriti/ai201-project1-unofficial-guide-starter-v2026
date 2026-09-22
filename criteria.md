 # Acceptance criteria — The Unofficial Guide

These criteria describe my targets before evaluating the system’s answers.

## 1. Retrieved chunks contain the answer

For at least 4 of my 5 test questions, the retrieved chunks include one that contains the answer.

**Why this target:**

My campus documents are short and focus on specific topics, so I expect retrieval to find relevant information for most questions. I chose four rather than five because a question may use different wording from its source document, making a relevant match harder to find.

---

## 2. Every answer names a source

Every answer the system produces names at least one source document.

**Why this target:**

Students should be able to check where information about deadlines and campus policies came from. The retrieved chunks include source filenames, so I expect every document-based answer to include one rather than allowing answers that cannot be checked.

---

## 3. The relevance gate stops out-of-corpus questions

When I ask a question my documents clearly don't cover, the relevance gate stops it and the system returns "I don't have enough information about that" — in at least 4 of 5 tries.

**Why this target:**

My collection covers campus life, so the system should refuse questions about unrelated subjects. I chose four of five because an unrelated question could still share words with a campus document, but the gate should reject most clear mismatches. I have not measured the distance scores yet.

---

## 4. Chunks keep rules and their conditions together

In at least 4 of the 5 sample chunks in my README, any campus rule mentioned stays together with its conditions or exceptions from the original document. I will compare each chunk with its source to check this.

**Why this target:**

My documents are short, but separating related sentences could change their meaning. For example, the dining dollars policy needs both the rollover rule and the expiration information. Four of five allows one imperfect split while requiring most chunks to preserve this context.

---

## 5. Sources support the answer

For at least 4 of my 5 test questions, every factual claim in the answer is supported by the documents it cites. I will read those documents to verify the claims. A refusal counts as a failure for these answerable questions.

**Why this target:**

An incorrect deadline or requirement could mislead a student. This checks whether the cited documents actually support the answer, beyond simply including a filename. Four of five sets a strong initial target while allowing one answer that needs improvement.

---


<!-- ─────────────────────────────────────────────────────────────────────────
     UNIT 2 — read this before you change anything above.

     If a criterion turns out to be BROKEN rather than merely unmet, you can
     revise it, and that earns credit. But never delete or edit the original
     line. Add the revision underneath it, like this:

         ## 1. Retrieved chunks contain the answer

         For at least 4 of my 5 test questions, the retrieved chunks include
         one that contains the answer.

         **Why this target:** ...

         > **Revised in unit 2:** For at least 4 of 5 questions, the top three
         > results contain the answer.
         >
         > **Why revised:** I couldn't judge "the chunks include one that
         > contains the answer" the same way twice — I scored two questions
         > differently on Monday than on Wednesday. The new version is
         > something I can actually check.

     That's a revision because the criterion couldn't be MEASURED.

     Lowering a target because you missed it is not a revision, and it costs
     you the point:

         ✗ "I said 4 of 5 but got 2 of 5, so 2 of 5 is more realistic."

     A number you missed stays where it is, gets diagnosed, and gets a fix
     attempted. That's where the points are.

     The whole reason the originals stay visible is so someone can see what you
     said before you knew the answer.
     ───────────────────────────────────────────────────────────────────────── -->
