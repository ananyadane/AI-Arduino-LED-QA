# AI-Arduino-LED-QA

## Project Title
AI-Assisted GitHub-Based QA Documentation and Problem Solving for Arduino LED Project

## Objective
The objective of this project is to implement a basic Arduino LED blinking system and use AI-assisted analysis and GitHub tools to identify, document, verify, and resolve software quality issues.

## Project Description
This project implements a simple LED blinking system using an Arduino board. The original program uses delay() to turn the built-in LED ON and OFF at regular intervals.

The project code was analyzed using ChatGPT to identify possible timing, blocking, configuration, and scalability issues.

## Tools Used
- Arduino
- Arduino IDE
- GitHub
- ChatGPT

## Original Code
The original code uses delay(1000) to control the LED blinking interval.

File:
LED_Blinking.ino

## QA Analysis
The AI-assisted QA analysis identified four main issues:

1. Blocking delay() calls
2. Timing depends on delay() execution
3. No configurable blink interval
4. Limited scalability / blocking design

These issues were documented using GitHub Issues.

## AI-Assisted Solution
ChatGPT was used to analyze the code, identify root causes, suggest solutions, and assist with code refactoring.

The main improvement was replacing delay() with millis()-based non-blocking timing.

## Refactored Code
The improved implementation uses:
- millis()
- BLINK_INTERVAL
- previousMillis
- ledState

File:
Refactored_LED_Blinking.ino

## Verification
The refactored code was reviewed to confirm that delay() is no longer used.

The verification details are documented in:

VERIFICATION.md

## GitHub Issues
Four QA issues were created in the GitHub repository to document the identified problems, their severity, root causes, suggested solutions, and verification methods.

## AI Prompt Log
The prompts used during AI-assisted analysis and refactoring are documented in:

AI_PROMPT_LOG.md

## Project Planning and Tracking
GitHub Issues were used to identify and track QA problems.

The repository contains the original code, refactored code, AI prompt log, and verification documentation.

## Learning Outcomes
- Learned how to create and manage a GitHub repository.
- Learned how to use GitHub Issues for QA documentation.
- Learned how AI can assist in identifying software issues.
- Learned the difference between blocking delay() and non-blocking millis() timing.
- Learned how to document and verify AI-assisted solutions.

## QA Resolution Tracking

Issue #1 was analyzed using AI assistance. The identified blocking delay() problem was addressed by developing a refactored version using millis()-based non-blocking timing.

The refactored solution is available in:
Refactored_LED_Blinking.ino
