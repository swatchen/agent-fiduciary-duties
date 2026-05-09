# Contributing

## Duty Lifecycle

Each duty progresses through a defined lifecycle. The `/duties/` folder contains only accepted duties. All deliberation happens on pull requests.

### Proposing a Duty

Create a branch, add a new Markdown file to `/duties/<category>/`, and open a PR using the [duty PR template](.github/PULL_REQUEST_TEMPLATE/duty.md). The PR title should be the duty name. One duty per PR.

The PR contains two distinct parts. The **duty file** in the branch must follow the duty template exactly -- it is the clean, canonical description of the duty and contains no deliberation content. All proposal justification, analysis, and discussion belong in the **PR description** and review comments, not in the duty file. When the PR is merged the duty file enters the taxonomy as-is; the deliberation record lives in the PR history.

The PR description must address all of the following before the proposal is eligible for review:

- **Harm statement.** What concrete harm does this duty prevent? Who gets hurt, how, and under what conditions?
- **Relationship specification.** Who is the fiduciary, who is the beneficiary, and what power asymmetry justifies imposing this obligation?
- **Classification.** Is this duty Grounded or Novel? Grounded duties extend an established fiduciary concept (care, loyalty, impartiality) into the digital twin context and must cite legal precedent. Novel duties propose obligations without direct legal analogue and must argue why the fiduciary framework -- rather than regulation, ethics guidelines, or technical standards -- is the right home for the obligation.
- **Boundary definition.** Where does this duty end? What is explicitly outside its scope?
- **Distinguishment.** Why isn't this covered by an existing duty? If it overlaps, why is a separate duty necessary rather than amending the existing one?
- **Compliance criteria.** How would an independent auditor determine whether this duty is being met? If adherence can't be observed or measured, it is an aspiration, not a duty.
- **Enforcement mechanism.** How is breach detected, adjudicated, and remedied?
- **Proportionality.** Is the burden on the fiduciary proportionate to the harm prevented?
- **Tension analysis.** Where does this duty conflict with other duties or legitimate interests? What is the proposed resolution or priority hierarchy?
- **Mandatory or aspirational.** Is non-compliance a violation or a departure from best practice? This classification carries the highest stakes and receives the most scrutiny during review.

Proposals that omit required sections will not advance to review.

### Under Review

A proposal moves to Under Review once all required sections are complete and at least one reviewer is engaged. Review requires:

- **Adversarial review.** At least one reviewer must actively attempt to find edge cases where the duty causes harm, is unenforceable, creates perverse incentives, or is meaningless in practice.
- **Consistency check.** The duty must be non-contradictory with all existing accepted duties. Where tension exists, explicit priority ordering must be established.
- **Implementation test.** It must be demonstrable that a system could actually comply with this duty in practice, not just in principle.
- **Grounded duties** additionally require verification against established fiduciary law to ensure no contradiction with existing legal obligations.

### Accepted

A duty is accepted when:

- All review requirements are satisfied.
- No unresolved formal objections remain. A formal objection is a substantive claim that the duty as written would cause harm, is unenforceable, or is inconsistent. It is not a stylistic preference.
- Consensus among reviewers is reached. Consensus means no sustained opposition from any domain-qualified reviewer, not a majority vote.
- All related duties are updated with cross-references and priority ordering where tensions exist.
- The mandatory or aspirational classification is confirmed.

Merging the PR places the duty file into `/duties/` as part of the canonical taxonomy.

### Deferred

A duty is deferred by closing the PR without merging. Deferral requires:

- A specific blocking condition, not "needs more discussion."
- A named prerequisite: what must change before reconsideration.
- The full discussion history is preserved. Deferred PRs should be labeled `deferred` and can be reopened when conditions are met.

## Directory Structure

```
duties/
  01-foundational/
  02-system-design/
  03-digital-twin/
  04-interaction/
  05-lifecycle/
  06-societal/
```

## General Guidelines

- One duty per PR.
- Keep duty descriptions precise.
- Use ToIP terminology where established conventions exist.
- Cross-reference related duties by relative link.
