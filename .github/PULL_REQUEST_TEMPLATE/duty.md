<!-- All proposal justification and deliberation goes here in the PR description.
     The duty file in your branch must follow the duty template exactly and contain
     no deliberation content. See CONTRIBUTING.md for the full lifecycle. -->

## Proposal

### Harm Statement
What concrete harm does this duty prevent? Who gets hurt, how, and under what conditions?

### Relationship Specification
Who is the fiduciary, who is the beneficiary, and what power asymmetry justifies this obligation?

### Classification
Is this duty **Grounded** (extends established fiduciary law -- cite precedent) or **Novel** (no direct legal analogue -- argue why the fiduciary framework is the right home)?

### Boundary Definition
Where does this duty end? What is explicitly outside its scope?

### Distinguishment
Why isn't this covered by an existing duty? If it overlaps, why is a separate duty necessary?

### Compliance Criteria
How would an independent auditor determine whether this duty is being met?

### Enforcement Mechanism
How is breach detected, adjudicated, and remedied?

### Proportionality
Is the burden on the fiduciary proportionate to the harm prevented?

### Tension Analysis
Where does this duty conflict with other duties or legitimate interests? What is the proposed resolution or priority hierarchy?

### Mandatory or Aspirational
Is non-compliance a violation or a departure from best practice? Justify.

---

## Duty File Checklist

Your branch must include a single new file at `duties/<category>/<duty-name>.md` matching the template below exactly. This file contains only the duty itself -- no proposal arguments or discussion.

- [ ] File follows the duty template
- [ ] File contains no deliberation content
- [ ] Category directory is correct
- [ ] Related duties are linked

### Duty Template

```markdown
# Duty Name

- **Category:** (Foundational | System Design | Digital Twin | Interaction | Lifecycle | Societal)
- **Classification:** (Grounded | Novel)
- **Binding:** (Mandatory | Aspirational)
- **Fiduciary:** (who owes the duty)
- **Beneficiary:** (who is protected)
- **Related Duties:** [Duty Name](../category/duty-file.md), ...

## Description

Concise statement of what the duty requires.

## Scope

What this duty covers and where it ends.

## Compliance

How adherence is observed or measured.

## Enforcement

How breach is detected, adjudicated, and remedied.
```
