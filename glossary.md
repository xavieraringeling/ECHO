# ECHO Glossary

## Core Framework

**ECHO**  
Ecosystem for Controlled Human/AI Output. A framework for building modular, traceable, maintainable prompts in high-stakes environments. Not a tool. A design logic.

**Prompt**  
A specific, structured request to an AI model, composed from components. In ECHO, a prompt isn’t a sentence. it’s a composition with traceable logic.

**Recipe**  
The reusable structure behind a class of prompts. Defines which components are needed, which are optional, and which techniques apply. Recipes carry the method. Prompts carry the moment.

**Recipe Variant**  
A version of a recipe adapted to a specific context or domain, while maintaining the core structural logic.

**High-Stakes Context**  
Domains where prompt failure has legal, ethical, reputational, or cultural consequences. ECHO is designed for these environments by default.

## Architecture & Design

**Modular Prompting**  
A design approach where prompts are assembled from interchangeable components: Context, Role, Instruction, etc.—each with a single function. Enables reuse, revision, and control.

**Component**  
A defined segment of a prompt with a distinct purpose. Components include Context, Role, Instruction, Guidelines, Guardrails, Output Instructions, and more.

**Component-Level Architecture**  
The structural backbone of ECHO. Each component is independent, updatable, and traceable. Prevents cascade failure and enables precise control.

**Lifecycle Logic**  
Prompts evolve through deliberate stages: design, validation, deployment, revision, and retirement. Each stage is visible and governs change.

**Metadata**  
Tags and fields attached to each component to enable filtering, sorting, versioning, and governance. Examples: tone type, ethical risk, domain.

**Versioning**  
Tracking changes to prompts and components over time. Ensures updates are transparent, reversible, and reviewable.

## Prompt Components

**Context**  
Frames the situation the prompt addresses what’s happening, why it matters, and what the model needs to know before responding. Without context, prompts drift or misfire. In ECHO, it’s the situational anchor.

**Perspective**  
An optional but critical component that sets the ethical or interpretive lens (e.g. feminist, decolonial, accessibility-first). Decouples what matters from how it’s said.

**Role**  
Defines the speaker position the model should adopt e.g. legal reviewer, benefits officer, empathetic advocate. Not tone. Not perspective. Just posture.

**Guidelines**  
Style and tone rules that shape how the model speaks. Applied consistently across prompts where the emotional or formal register needs control.

**Guardrails**  
Explicit constraints that block known risks e.g. deflection, impersonation, bias amplification. Guardrails are non-negotiable and enforced by design.

**Guardrails vs Guidelines**  
Guardrails prevent. Guidelines shape. Guardrails block unsafe or misleading moves. Guidelines set tone, voice, and fluency boundaries.

**Output Check**  
A quality gate for AI output. Ensures the result matches the purpose, respects risk boundaries, and performs under scrutiny. Can be AI- or human-driven.

## Quality & Evaluation

**Real-World Fit**  
A recipe for situational alignment. Ensures that tone, stance, and structure match the moment the message enters, not just the message itself.

**Framing Failure**  
When a prompt fails not in tone or logic, but in worldview. The model interprets the wrong frame. Often leads to polite but misaligned outputs.

**Human Review**  
Optional but critical for high-risk prompts. Ensures a qualified expert, not just a user—has validated the structure, not just the output.

**Fit-for-Purpose**  
A test of whether the prompt does what it claims under real conditions, for the real audience. More than "does it work?" It's "does it work *here*?"

**Cascade Failure**  
When a single bad update breaks multiple dependent prompts. Prevented in ECHO by isolating logic into components and tracking inheritance.

## Common Problems & Solutions

**Prompt Drift**  
The gradual degradation of prompt alignment as context, model behavior, or system rules evolve. ECHO detects and corrects this via structure.

**Silent Failure**  
When a prompt appears to work but produces low-quality, misleading, or biased outputs, often undetected until consequences surface.

**Chain-of-Thought**  
A prompting technique where reasoning is split into sequential steps. ECHO uses a similar approach structurally decomposing intention into discrete components.

**Role Priming**  
A technique where the model is assigned a clear role or identity to shape its interpretation and output. In ECHO, this is a formal component, not a style trick.
