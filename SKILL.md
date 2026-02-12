---
name: create-research-prompt
description: Generate a structured, domain-specific deep research prompt from a user's request.
---

# Workflow

Classify the request into one domain:

TECHNICAL — Engineering, architecture, integrations, system design, DevOps, tooling
STRATEGIC — Business intelligence, market analysis, org design, competitive positioning, GTM
LEARNING — Training design, instructional programs, capability building, workshops


Load the matching template from references/:

TECHNICAL → resources/technical.md
STRATEGIC → resources/strategic.md
LEARNING → resources/learning.md


Populate the template using the user's request:

Fill in every field possible from what the user provided.
Use bullet points within sections rather than dense paragraphs for scannability.
Be concise: Use precise terminology over explanatory prose. Each field should be tight and actionable.
Use domain-specific terminology that demonstrates depth (e.g., "investment-grade analysis," "product-level drivers," "CI/CD pipeline").
For fields the user didn't specify, insert smart defaults or contextually reasonable values based on the topic — do not leave raw placeholders like [FILL IN].
Where a field truly cannot be inferred, use a brief instructive placeholder that tells the user what to add, e.g., [Specify your compliance requirements — e.g., SOC2, HIPAA, or N/A].
Adapt the template ruthlessly:

Add domain-specific sections when warranted (e.g., regulatory for healthcare, ethical review for AI research).
Remove N/A sections entirely rather than including them with "N/A" values. Streamline aggressively.


Strategic domain: Default to "multidisciplinary team" with 2-4 specific relevant roles rather than a single generic role for the Expert Perspective field.
Be selective with checkboxes: Check only what's truly essential for THIS specific research question, not everything possible.


Output the completed prompt inside a single markdown code block (```). No preamble, no usage instructions, no explanation — just the prompt. Add a one-line note above the code block stating the detected domain.

Key Rules

Always include the Source Verification Standards block from the template verbatim — these are non-negotiable baseline requirements, not placeholders to adapt or remove.
Never answer the research question. Only produce the prompt.
Minimize back-and-forth. Generate the best prompt possible from what the user provides.
Use plain text inside the generated prompt — no bold, italic, or markdown formatting.
Keep all placeholders clearly bracketed with [ ].
Ensure the prompt encourages multiple perspectives, alternative solutions, and source quality hierarchy.
The prompt itself should be actionable and efficient — written like something a professional would actually use, not an academic exercise.