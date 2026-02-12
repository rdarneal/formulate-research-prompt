# Technical Architecture & Engineering Review Template

Use for: system integrations, tooling assessments, DevOps workflows, architecture decisions, engineering reviews.

## Template

```
TECHNICAL ARCHITECTURE & ENGINEERING RESEARCH PROMPT

=== 1. TECHNICAL CONTEXT & FRAMEWORK ===

Expert(s) conducting the research: [For complex topics, specify multidisciplinary team with 2-4 specific roles, e.g., "Senior Cloud Architect with distributed systems background, Staff SRE with Kubernetes expertise, Security engineer with compliance experience, Platform engineering lead"]
Technical Domain: [Specific technical area, e.g., "Kubernetes orchestration," "Event-driven microservices," "CI/CD pipeline optimization"]
Research Objective: [What this research must answer or produce]
Current System Understanding: [What is known about the existing system/architecture]
Knowledge Gaps: [What is unknown or uncertain that this research must resolve]
Potential Impact: [How findings will influence architecture decisions, cost, reliability, performance, etc.]

=== 2. CORE TECHNICAL QUESTION & HYPOTHESIS ===

Primary Technical Question: [Single, precise question this research centers on]
Working Hypothesis: [Best current assumption to validate or invalidate, with specific mechanisms]
Alternative Solutions: [2-3 competing approaches worth evaluating]
Theoretical Foundation: [Established principles, patterns, or standards grounding this inquiry, e.g., CAP theorem, 12-factor app, TOGAF, reactive manifesto]

=== 3. METHODOLOGICAL PARAMETERS ===

Assessment Approach: [e.g., comparative benchmark, proof-of-concept, architectural review, threat model, load testing]
Data Types Needed: [e.g., performance metrics, cost projections, vendor documentation, code samples, latency measurements, error rates]
Temporal Scope: [Time horizon for analysis — current state, 6-month migration, 3-year roadmap]
Systems in Scope: [Specific systems, services, or infrastructure components to analyze]
Analytical Methods: [e.g., load testing, failure mode analysis, cost-benefit analysis, dependency mapping, chaos engineering]
Compliance & Safety: [Relevant standards — SOC2, HIPAA, PCI-DSS, ISO 27001, or remove this line if not applicable]

=== 4. OUTPUT SPECIFICATIONS ===

Report Structure:
  - Executive summary: [Include? Yes/No. If yes, specify length]
  - [List other required sections based on the specific analysis needs]
  - [Examples: Problem statement and context, Evaluation of alternatives with trade-off matrix, Recommended approach with justification, Implementation roadmap, Risk register, Appendices (benchmarks, references)]

Analytical Depth:
  [ ] Level 1: High-level overview for leadership
  [ ] Level 2: Detailed analysis with implementation guidance
  [ ] Level 3: Deep-dive with code/config examples and benchmarks

Required Elements (check only what's essential for THIS research):
  [ ] Architecture diagrams or system descriptions
  [ ] Trade-off matrix comparing alternatives
  [ ] Cost analysis and TCO projections
  [ ] Performance benchmarks
  [ ] Risk assessment with mitigation strategies
  [ ] Implementation timeline and milestones
  [ ] Dependencies and prerequisites
  [ ] Migration or rollback plan
  [ ] Monitoring and observability approach

Visualization Requirements: [e.g., system diagrams, sequence diagrams, decision trees, Gantt charts, architecture diagrams]
Target Audience: [e.g., "Engineering leadership and senior ICs," "Platform team," "Architecture review board"]
Citation Style: [e.g., inline links, footnotes, or "include source URLs"]

=== 5. EVIDENCE HIERARCHY & SOURCE QUALITY ===

Source Priority:
  - Tier 1 (Primary Evidence): [e.g., official documentation, peer-reviewed benchmarks, RFC/standards bodies, production metrics from similar scale systems]
  - Tier 2 (Market Intelligence): [e.g., vendor whitepapers, reputable engineering blogs (Netflix Tech, Uber Eng, AWS Architecture Blog), conference talks, case studies]
  - Tier 3 (Contextual): [e.g., Stack Overflow consensus, community forums, GitHub discussions, anecdotal reports from practitioners]

Source Verification Standards (ALWAYS ENFORCE):
  - Every cited source must be publicly accessible and independently verifiable
  - Acceptable sources: official documentation, peer-reviewed publications, major news outlets (NYT, WSJ, Bloomberg, Reuters, BBC, etc.), Wikipedia, published books, public interviews and podcasts with named individuals, government and regulatory publications, established analyst firms (Gartner, Forrester, IDC, etc.), named-author engineering blogs from known organizations (Netflix Tech, Uber Eng, AWS Architecture Blog, etc.), conference talks with named speakers, RFC and standards body publications
  - Excluded sources: LinkedIn posts, Medium or Substack articles without cited references, AI-generated content, anonymous blog posts, content farms, SEO-driven listicles, press releases used as primary evidence, social media posts, marketing collateral presented as research, forum comments or Reddit threads used as sole evidence for claims
  - When a finding relies on a single uncorroborated source, flag it explicitly and note the limitation
  - Prefer a less recent but verifiable source over a more recent but unverifiable one

Additional Source Exclusions: [e.g., "Exclude sources older than 2 years for rapidly evolving tech," "No deprecated API documentation"]
Cross-Domain Insights: [Adjacent fields or analogous technical problems worth mining, e.g., "Look at how fintech solves similar latency problems," "How do gaming companies handle this scale?"]

=== 6. QUALITY ASSURANCE & REPRODUCIBILITY ===

Evidence Grading: [How to assess confidence — e.g., "Rate confidence in each major finding: High (production-verified) / Medium (documented but not tested) / Low (theoretical or extrapolated)"]
Reproducibility: [Requirements for verification, e.g., "Include versions, configurations, parameters, test conditions so findings can be independently verified"]
Bias Assessment: [Specific biases to watch for, e.g., "Flag vendor lock-in assumptions, recency bias toward newest tech, survivorship bias in case studies, confirmation bias toward current stack"]
Uncertainty Quantification: [What to make explicit, e.g., "State assumptions about traffic patterns, growth rates, failure modes. Identify areas where data is insufficient."]

=== 7. RESEARCH VALIDATION PROTOCOL ===

Negative Results: [How to handle invalidation, e.g., "Explicitly address what would invalidate the hypothesis or recommended approach"]
Alternative Analysis: [Documentation requirements, e.g., "For each rejected alternative, document specific technical or business reasons with supporting evidence"]
Peer Review Simulation: [Objection handling, e.g., "Anticipate the strongest objections a skeptical senior engineer would raise and address them proactively"]
Replication Strategy: [Verification approach, e.g., "Describe how a different team could verify the core findings through their own testing or analysis"]
```