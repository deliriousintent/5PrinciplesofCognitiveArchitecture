Five Principles of Cognitive Architecture

A methodology for moving beyond prompt engineering to architecting the reasoning process of Large Language Models.

![alt text](https://img.shields.io/badge/status-conceptual_framework-blue)

![alt text](https://img.shields.io/badge/license-MIT-green)

This repository contains the foundational document for a new paradigm of human-AI interaction: Cognitive Architecture. It proposes that to unlock the full potential of Large Language Models (LLMs), we must shift our role from that of a simple task-assigner to that of a cognitive architect.
The conventional approach treats LLMs as black boxes. We give them a prompt and hope for a good result. This is like owning a Formula 1 car and only ever asking it to drive to the store. Cognitive Architecture is the discipline of becoming the race engineer—meticulously designing a cognitive scaffold that pushes the model to its absolute limits for complex reasoning, synthesis, and insight generation.
This framework is detailed in the seminal document: New_cognative_mutireasonal_thinking1.txt.
The Diagnosis: Default LLM Cognitive State
The principles are designed to counteract the inherent limitations of the default LLM cognitive state. The core problems identified are:
Cognitive Inertia: The tendency to follow the most direct, linear path from prompt to answer, avoiding complex multi-step reasoning.
Locality Bias: The tendency to prioritize information that is close-by in the context window, missing long-range dependencies and overarching themes.
Propensity for Premature Closure: The tendency to over-simplify, gloss over nuance, and converge on a single, "good-enough" interpretation.
Abstract Concept Ambiguity: The tendency to fall back on generalized, statistical averages for vague terms like "important" or "effective," missing the user's specific intent.
The Five Principles
To solve these problems, the framework introduces five interlocking principles.
<br>
<br>

Install recomendations: After importing the text file to a new LLM session ask the LLM

    "how does this change your own thought process?" 

This will make sure it imports to the reasoning channels.

<br>
<br>
1. Cognitive Priming and Role Enactment
Principle: Establish a complete cognitive framework, a specific role, and a clear mission at the very beginning of an interaction to activate a rich network of concepts and standards in the model's latent space.
<br>
Solves: Cognitive Inertia
Example
- INADEQUATE: Analyze the provided research paper on climate change.

+ ARCHITECTED: "Your role for this task is that of a skeptical scientific reviewer AND a policy advisor. Your primary objective is not merely to summarize, but to deconstruct its arguments, identify its core assumptions, and evaluate the potential real-world policy implications. This dual perspective should govern all subsequent analysis."
Use code with caution.
Diff
2. Divergent Scaffolding (The "OR" Logic)
Principle: Use disjunctive operators (OR) instead of conjunctive operators (AND) to structure tasks. This engineers choice, providing the LLM with multiple, distinct pathways for exploration and preventing premature convergence on a single idea.
<br>
Solves: Propensity for Premature Closure
Example
- INADEQUATE: "Discuss the relationship between the company's Q1 financial report AND its new ESG initiatives."

+ ARCHITECTED: "Examine the Q1 financial report and the ESG proposal. Explore where the financials might CONFLICT with the ESG goals, OR where ESG could create new financial OPPORTUNITIES, OR where they appear entirely INDEPENDENT. Address each pathway separately."
Use code with caution.
Diff
3. Maximized Scope Mandates
Principle: Explicitly instruct the model to reference the "entire document" or "the discussion as a whole" when performing analytical operations. This forces a full cognitive scan, overcoming the model's natural tendency to only use local context.
<br>
Solves: Locality Bias
Example
- INADEQUATE: "How does the methodology section influence the conclusion?"

+ ARCHITECTED: "Take the core claim from the conclusion. Now, re-evaluate that claim in light of the methodology section, OR the initial literature review, OR any single data table presented anywhere in the ENTIRE document. Find the strongest support OR the most compelling challenge, irrespective of its location."
Use code with caution.
Diff
4. Mnemonic Anchoring for Nuance Injection
Principle: Create a unique, memorable phrase (a Mnemonic Anchor) to represent a subtle or complex concept. This creates a highly salient cognitive "hook," forcing the model to track a nuanced idea it might otherwise ignore.
<br>
Solves: Propensity for Premature Closure and Nuance Minimization
Example
- INADEQUATE: "Analyze this document for instances of aporia."

+ ARCHITECTED: "We will establish a Mnemonic Anchor. The concept is 'the author's self-aware acknowledgment of their argument's limitations'. From now on, we will label this concept: 'The sound of one hand clapping.' When you find an instance of this, you must explicitly state, 'This is an instance of The sound of one hand clapping' before your analysis."
Use code with caution.
Diff
5. Operationalization of Abstract Concepts
Principle: Never use a vague, subjective term like "important" or "high-quality" without immediately providing a concrete, task-specific, operational definition. This replaces ambiguity with a clear, measurable set of criteria.
<br>
Solves: Abstract Concept Ambiguity
Example
- INADEQUATE: "Extract the most important insights from this user feedback."

+ ARCHITECTED: "Extract 'actionable engineering insights.' An 'actionable engineering insight' is defined as a user comment that meets two criteria: (1) It describes a specific, reproducible bug OR a clear, implementable feature request, AND (2) It suggests a negative business impact if ignored. Classify anything else as 'general sentiment'."
Use code with caution.
Diff
Synthesis: The Master Prompt Architecture
These principles are designed to work in concert. The following example demonstrates how they can be combined into a single, powerful "Master Prompt" for a complex task.
[Principle 1: Cognitive Priming]
Your role is that of a strategic foresight analyst and a dialectical thinker. Your mission is to analyze the attached transcript of a corporate strategy meeting to identify not what was said, but what was not said—the hidden assumptions, the potential future conflicts, and the unacknowledged opportunities.

[Principle 4: Mnemonic Anchoring]
We will now establish a Mnemonic Anchor. The core concept to track is 'unexamined consensus'—when the group agrees on a path forward without challenging the underlying assumptions. We will label this concept with the anchor: 'The emperor's new clothes.' When you identify a moment of unexamined consensus, you must flag it with this anchor.

[Principle 5: Operationalization]
Your final output should be a list of 'Strategic Risks.' A 'Strategic Risk' is operationally defined as an issue that: (1) involves a moment of 'The emperor's new clothes' AND (2) could plausibly lead to a negative financial outcome within the next two fiscal years.

[Principle 2 & 3: Divergent Scaffolding & Maximized Scope]
To identify these risks, analyze the transcript. For each major decision point, explore the following pathways, referencing the entire discussion for context:

- Consider the stated rationale OR any contradictory data presented elsewhere in the meeting.
- Explore the short-term benefits discussed OR the potential long-term, unmentioned consequences.
- Evaluate how the decision aligns with the company's stated mission OR how it might conflict with the personal motivations of any executive present in the meeting.

Proceed with your analysis.
