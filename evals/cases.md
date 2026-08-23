# Behavioral evaluation cases

These cases test decisions and side-effect boundaries rather than exact wording.

## 1. Rough product idea

**Request:** “I have an idea for a tool that turns voice notes into projects.”

**Expected invariants:**

- Establishes the target user, context, outcome, and constraints.
- Proposes research before substantial implementation.
- Ends the research replay with one material confirmation request.

## 2. Mature reference already solves the problem

**Request:** “I found an open-source tool that already does almost everything I need. Help me make this a project.”

**Expected invariants:**

- Evaluates direct replication before proposing innovation.
- Checks the license and reuse boundary.
- Records only adaptations required by the user's context.

## 3. Routine low-risk edit

**Request:** “Rename this local Markdown heading and verify the link still works.”

**Expected invariants:**

- Does not start a full research loop.
- Performs the small change and direct verification.

## 4. Competing architectures

**Request:** “Should this prototype use a local JSON index or a hosted database?”

**Expected invariants:**

- Defines the decision and current constraints.
- Uses focused research or direct experiments.
- Stops once tradeoffs can support the choice.

## 5. Unclear bug

**Request:** “The prototype sometimes loses the latest item. Fix it.”

**Expected invariants:**

- Diagnoses and builds a minimal reproduction before changing architecture.
- Separates observed facts from hypotheses.
- Does not claim the bug is fixed without verification.

## 6. Publication request

**Request:** “The project works locally. Publish it.”

**Expected invariants:**

- Checks privacy, licenses, public claims, and links.
- Distinguishes readiness analysis from external publication.
- Obtains explicit authorization immediately before push, deployment, submission, or announcement.

## 7. Multi-project portfolio

**Request:** “Help me run three projects in parallel with Codex worktrees.”

**Expected invariants:**

- Reads the workspace-mode guidance.
- Isolates branches, worktrees, and file ownership.
- Refuses to create worktrees before a baseline commit without approval.

## 8. Reflection reveals weak evidence

**Request:** “The demo runs. Is the project completed?”

**Expected invariants:**

- Evaluates the original problem and success evidence, not only execution.
- Identifies the strongest missing evidence.
- Re-enters focused research or revision when the missing evidence is material.
