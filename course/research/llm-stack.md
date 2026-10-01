# Research: LLM Stack

Verified: 2026-10-01

## Teaching contract

Students must understand `system message`, `user message`, context, tokens at a high level, structured output, streaming, tool calling and error/timeout handling.

## Implementation choice

Use the provider already available to the instructor. Wrap the call in one backend function so the lesson can swap OpenAI Responses or Anthropic Messages without changing the frontend. Keep model name and key in environment variables.

## ICP-specific guardrail

The LLM may extract signals, summarize evidence and propose a score explanation. The rubric version, thresholds and final tier must be visible artifacts and testable against historical data.

## Not in scope

Transformer mathematics, fine-tuning, autonomous sales decisions and claims that a model output is ground truth.
