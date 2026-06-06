# Prompt — Generate ADR from Meeting Notes

> Use these prompts with the ADR Generator Gem right after a meeting or decision session.
> Choose the variant that matches how you're providing the input.

---

## Variant 1 — Attached transcript file

Use when you have a transcript file (`.md`, `.txt`, `.docx`, `.pdf`) to upload directly to the Gem.

```
Generate the ADR for [brief summary of the decision] based on the attached refinement transcript.
```

**How to use:**
1. Open the ADR Generator Gem
2. Attach the transcript file
3. Paste the prompt above, replacing `[brief summary of the decision]` with a one-line description
4. Send

---

## Variant 2 — Pasted text

Use when you have raw notes, a meeting summary, or a transcript copied to the clipboard.

```
Generate the ADR for [brief summary of the decision] based on the refinement transcript below:

[Paste the transcript or decision summary here]
```

**How to use:**
1. Open the ADR Generator Gem
2. Paste the prompt above, replacing:
   - `[brief summary of the decision]` with a one-line description
   - `[Paste the transcript or decision summary here]` with your raw notes or transcript
3. Send

---

## Tips

- The brief summary in both prompts helps the Gem name and code the ADR correctly — keep it specific (e.g., "adoption of Kafka for async order processing" rather than "messaging decision")
- Always review the **Consequences** and **Trade-offs** sections — the Gem may miss organizational or political constraints not explicit in the transcript
- If the decision is still open, set `Status: Proposed` and let the team validate before merging the ADR
