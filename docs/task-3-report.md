# Rules File Experimentation (Task 2 & 3)  

## 1. Overview

This document records my work for the agent rules configuration challenge.  
The goal: to benchmark and improve my agent's rules file using research from Boris Cherny's workflow (Claude Code) and broader community best practices.  
**Rules file under review:** `.github/copilot-instructions.md` (for VS Code)

---

## 2. What I Did

**Research:**
- Reviewed Boris Cherny's thread on agent setup and prompt strategies for Claude Code
- Surveyed recent Github discussions and blogs about controlling/optimizing coding agents (Copilot, Claude, Cursor, etc)
- Compared rule files/templates shared by other advanced users

**Configuration iterations:**
- [ ] Strengthened file/folder naming rules
- [ ] Clarified preferred code style and formatting expectations
- [ ] Added explicit instructions on security and privacy (e.g., never output credentials)
- [ ] Tuned agent creativity level and response completeness

---

## 3. What Worked

- Strong, explicit “Do Not” sections made the agent more predictable (e.g., “Never edit files in /deploy unless explicitly told”)
- Including examples/templates in the rules led to higher quality automated code completions
- Instructions that specify "**always ask before making big changes**" reduced undesired mass refactoring

---

## 4. What Didn’t Work

- Overly long or ambiguous rules often got ignored or confused the agent
- Generic wording (e.g., "Be smart about...") yielded inconsistent results
- Adjusting creativity settings too high/low sometimes led to loss of useful suggestions or overly verbose output

**Troubleshooting:**  
- Shortened and simplified unclear sections  
- Added concrete examples rather than vague principles

---

## 5. Insights Gained

- _Rules-based configuration is powerful_—the more explicit and context-aware the rules, the more reliably the agent follows user intent.
- _Examples are essential_—showing specific input/output demos helps align the agent's pattern-matching.
- _Iterative testing_ after each edit shows tangible changes; sometimes small tweaks have outsized effects.
- _Different models/agents (Copilot vs Claude) respond differently_—it's important to tailor the language and instructions accordingly.

---

## 6. Next Steps

- Continue to refine rules as new tasks arise and as agent models evolve
- Consider open-sourcing my rules file/template for others to benefit

---

## Appendices

### A. Example Diff — Key Rule Change

```diff
- Please follow the coding style in this repository.
+ Always ensure new code matches the indentation, variable naming, and module organization seen in /src.
```

### B. Reference Material
- [Boris Cherny Claude Code Workflow Thread](https://x.com/bcherny/status/2007179832300581177)  
- [vscode docs](https://code.visualstudio.com/docs/copilot/customization/custom-instructions)
