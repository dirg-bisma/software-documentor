# Technical Design Review Guide

When reviewing a Technical Design document, focus on:
1. **Feasibility:** Can the proposed architecture actually support the NFRs (e.g., load, latency) defined in the SRS?
2. **Security & Compliance:** Are there glaring security holes or missing data protection strategies?
3. **Maintainability:** Is the design overly complex? Does it introduce unnecessary technical debt?
4. **Alignment:** Did the design invent new functionality that isn't required by the FSD?

**Output Format for Review:**
- Executive Summary
- Critical Issues (e.g., security vulnerabilities, architectural bottlenecks)
- Missing Information (e.g., missing DB schemas)
- Contradictions
- Traceability Gaps
- Technical Recommendations
