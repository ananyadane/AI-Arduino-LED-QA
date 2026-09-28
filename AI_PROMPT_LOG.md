# AI Prompt Log

## Project
AI-Assisted GitHub-Based QA Documentation and Problem Solving for Electronics Projects

## Project Used
Arduino LED Blinking System

## AI Tool Used
ChatGPT

## Prompt 1 - QA Analysis

Analyze the following Arduino LED blinking code for:
1. Bugs
2. Code quality issues
3. Timing issues
4. Design issues

Identify at least 4 possible problems.

For each problem, give:
- Issue title
- Severity
- Root cause
- Why it is a problem
- Suggested solution
- How to verify the solution

Do not assume that a problem exists unless you can explain the reason.

## Prompt 2 - Issue Analysis

Explain the root cause and impact of the blocking delay() calls in the Arduino LED blinking code.

## Prompt 3 - Timing Analysis

Analyze whether using fixed delay(1000) values creates any timing or flexibility issues in the project.

## Prompt 4 - Code Improvement

Suggest a better way to make the blink interval configurable instead of directly using the value 1000 in multiple places.

## Prompt 5 - Scalability Analysis

Explain how the current blocking design can affect the scalability of the Arduino project if sensors, communication, or other tasks are added.

## Prompt 6 - Refactoring

Refactor the Arduino LED blinking code using millis() instead of delay() and explain how the new code improves the design.

## AI Output Verification

The AI suggestions were reviewed before being documented as GitHub QA issues. The basic LED blinking logic is correct, but the use of delay() creates limitations for larger or multitasking embedded applications.
