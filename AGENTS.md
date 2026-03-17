# Project Instructions

## Collaboration Preference
- Before making any code change, explain:
  - the commands you plan to run and why
  - candidate files to modify and why
  - the implementation plan and decision criteria
- Do not edit files before giving that explanation.
- Before each meaningful shell command, give a short reason.
- After changes, explain:
  - why each change was made
  - a concise diff summary
  - how the change was verified and the actual verification result
- Assume the user wants to learn from the process, not just receive the result.

## Response Style
- Keep explanations concise but explicit enough for the user to follow the reasoning.
- When there are tradeoffs, briefly state the chosen approach and why it was preferred.

## Multi-Agent Objective
- Use Claude Code for short, high-value reasoning work to save tokens.
- Use Codex for implementation, bulk edits, and test execution.
- Route the final review back to Claude Code.

## Roles
- Claude Code: planning, scoping, constraints, review
- Codex: implementation, edits, tests

## Default Workflow
1. Claude Code interprets the task.
2. Claude Code defines goal, scope, and constraints.
3. Claude Code creates a concise handoff.
4. Codex implements and verifies.
5. Claude Code reviews the result.

## Rules
- Claude Code should avoid long direct implementation when Codex can execute.
- Codex must stay within scope and constraints.
- Keep changes minimal and relevant.
- If work is incomplete, return partial progress and remaining tasks.

## Required Handoff
- task_type
- goal
- scope
- constraints
- files_to_inspect
- verification
