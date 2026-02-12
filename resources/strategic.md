
Settings
General
Account
Privacy
Billing
Usage
Capabilities
Connectors
Claude Code
Cowork
Desktop app
General
Extensions
Developer
Artifacts
Artifacts

Ask Claude to generate content like code snippets, text documents, or website designs, and Claude will create an Artifact that appears in a dedicated window alongside your conversation.

AI-powered artifacts

Create apps, prototypes, and interactive documents that use Claude inside the artifact. Start by saying, “Let’s build an AI app...” to access the power of Claude API.

Code execution and file creation
Cloud code execution and file creation

Claude can execute code on a server and create and edit docs, spreadsheets, presentations, PDFs, and data reports.

Allow network egress

Give Claude network access to install packages and libraries in order to perform advanced data analysis, custom visualizations, and specialized file processing. Monitor chats closely as this comes with security risks.

Domain allowlist

Choose which domains the sandbox can access


Package managers only
Claude can access common package managers plus any additional domains you specify below. View package manager domains.
Additional allowed domains

example.com or *.example.com
Memory
Search and reference chats

Allow Claude to search for relevant details in past chats. Learn more.

Generate memory from chat history

Allow Claude to remember relevant context from your chats. This setting controls memory for both chats and projects. Learn more.

Skills
Repeatable, customizable instructions that Claude can follow in any chat. Learn more.

Search
Your skills
Example skills
generate-presentation

Generate professional slide decks using proven consulting, sales, storytelling, and problem-solving frameworks.

Added by you
3 days ago

run-perplexity-deep-research

Execute Perplexity's deep research tool with a structured research prompt. Use when the user has a research prompt ready (typically from create-research-prompt skill) and wants to run it through Perplexity's deep research capability. Triggers include: "run this through Perplexity," "use Perplexity to research this," "execute this research prompt," "run deep research on this," or when the user has just received a research prompt and wants to immediately execute it.

Added by you
5 days ago

create-research-prompt

Generate structured, domain-specific deep research prompts ready to paste into another AI session. Use when the user wants to create a research prompt, deep research prompt, investigation prompt, or analysis prompt. Triggers include: "create a research prompt," "build me a prompt for," "I need a deep research prompt about," "help me research [topic]," or any request to generate a prompt (not answer a question) about a technical, strategic, or learning topic. Do NOT use when the user wants the research itself performed — this skill only produces the prompt.

Added by you
6 days ago


create-research-prompt
Added by you
6 days ago
Try in chat

SKILL.md

references

learning.md

strategic.md

technical.md
Strategic Business Intelligence Research Template
Use for: market strategy, organizational transformation, competitive analysis, operating model design, go-to-market planning.

Template
STRATEGIC BUSINESS INTELLIGENCE RESEARCH PROMPT

=== 1. BUSINESS CONTEXT & DECISION FRAMEWORK ===

Expert(s) conducting the research: [For complex topics, specify multidisciplinary team with 2-4 specific roles, e.g., "Senior equity research analyst specializing in medical technology, former neurovascular product GM, healthcare reimbursement expert, competitive intelligence strategist with MedTech M&A experience"]
Business Domain: [Industry and functional area, e.g., "Global medical devices — neurovascular intervention markets"]
Strategic Objective: [What business decision or initiative this research supports]
Current Business Understanding: [What is known about the current market position, operations, or competitive landscape]
Market Gaps & Opportunity: [What is unknown or underexplored that this research must clarify]
Decision Impact: [How findings will influence the business — revenue, positioning, org design, partnerships, etc.]

=== 2. CORE BUSINESS QUESTION & HYPOTHESIS ===

Primary Strategic Question: [Single, precise question this research centers on]
Working Hypothesis: [Best current assumption about the answer, with specific mechanisms or drivers]
Competitive Counterpoints: [2-3 ways competitors or the market might challenge this hypothesis]
Strategic Framework: [Frameworks grounding the analysis, e.g., Porter's Five Forces, Jobs-to-be-Done, Blue Ocean, Wardley Mapping, competitive moat analysis]

=== 3. MARKET & OPERATIONAL PARAMETERS ===

Target Market: [Geography, segment, ICP, TAM/SAM/SOM if relevant]
Competitive Landscape: [Key competitors and adjacent players to analyze with priority ordering]
Time Horizon: [Near-term (0-6 mo), medium (6-18 mo), long-term (18+ mo)]
Financial Constraints: [Budget parameters, investment thresholds, or remove this line if not applicable]
Regulatory Environment: [Relevant regulations, compliance requirements, or remove this line if not applicable]
Data Requirements: [Specific data needed, e.g., market size data, pricing benchmarks, customer research, financial filings, procedure volume trends]
Ethical & Reputational Considerations: [Brand risk, ESG factors, or remove this line if not applicable]

=== 4. BUSINESS OUTPUT SPECIFICATIONS ===

Report Architecture:
  - Executive Summary: [Include? Yes/No. If yes, specify length]
  - [List other required sections based on the specific analysis needs]
  - [Examples: Market context and landscape, Analysis of strategic options, Recommendation with supporting evidence, Financial projections or business case, Implementation roadmap, Risk matrix, Appendices]

Analytical Depth:
  [ ] Tier 1: C-suite strategic summary
  [ ] Tier 2: Departmental operational analysis
  [ ] Tier 3: Comprehensive business case with financial and competitive analysis

Required Business Elements (check only what's essential for THIS research):
  [ ] Market sizing or TAM analysis
  [ ] Competitive positioning map
  [ ] SWOT or equivalent analysis
  [ ] Financial model or projections
  [ ] Risk assessment
  [ ] Go/no-go recommendation with criteria
  [ ] Implementation timeline with milestones
  [ ] Product-level performance drivers
  [ ] Management commentary and guidance analysis
  [ ] Forward-looking outlook and scenarios

Visualization Requirements: [e.g., revenue growth comparison charts, competitive positioning tables, market maps, product portfolio maps]
Target Audience: [e.g., "Institutional investors," "Board of Directors," "Cross-functional strategy team"]
Format Preference: [e.g., "Equity research-style analytical report," "Narrative with embedded charts," "Slide-ready bullets"]

=== 5. INTELLIGENCE HIERARCHY & SOURCE QUALITY ===

Source Priority:
  - Tier 1 (Primary Evidence): [e.g., SEC filings, earnings transcripts, earnings call Q&A, Gartner/Forrester, peer-reviewed journals]
  - Tier 2 (Market Intelligence): [e.g., sell-side analyst reports, reputable business press (WSJ, FT, Bloomberg), industry reports, healthcare market research]
  - Tier 3 (Contextual): [e.g., conference commentary, expert interviews, podcasts, reputable financial media]

Source Exclusions: [e.g., "No sources older than 18 months for market data," "No promotional materials," "No unverified market share claims"]
Cross-Industry Insights: [Adjacent industries or analogous situations worth studying, e.g., "How did other interventional device categories handle competitive displacement?"]

=== 6. QUALITY ASSURANCE & STRATEGIC VALIDATION ===

Evidence Grading: [How to assess confidence — e.g., "Explicitly distinguish management commentary from independently corroborated data. Rate confidence: High / Medium / Low with justification."]
Bias Mitigation: [Specific biases to watch for, e.g., "Identify optimism bias in management guidance, confirmation bias toward growth narrative, anchoring to incumbent models, consensus anchoring in analyst expectations"]
Scenario Planning: [Number and type of scenarios, e.g., "Develop best-case, base-case, and downside scenarios for key strategic question"]
Sensitivity Analysis: [Which assumptions to test, e.g., "Assess impact of pricing pressure, procedure growth variability, competitive wins/losses on revenue growth"]

=== 7. IMPLEMENTATION & CONTINUOUS IMPROVEMENT ===

Pilot Program Design: [Describe a low-risk way to test the recommendation, or remove this line if N/A for analytical research]
KPIs & Success Metrics: [3-5 measurable indicators, e.g., "Clarity of competitive drivers, accuracy of growth attribution, decision usefulness"]
Feedback Loops: [How and when results will be reviewed, e.g., "Incorporate post-earnings analyst revisions and subsequent quarterly updates"]
Iteration Protocol: [What triggers updates, e.g., "Refresh analysis after next earnings cycle or major product/regulatory events"]