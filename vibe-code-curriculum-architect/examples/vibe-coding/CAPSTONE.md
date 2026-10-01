# Capstone: Personal Knowledge AI Chat

## Goal

Build an application that accepts a question, retrieves relevant information from a small private document set, sends grounded context to an LLM, and displays the answer.

## Architecture

```text
User -> Frontend -> Backend -> Retrieval -> LLM -> Backend -> Frontend
                         ^
                         |
Documents -> Ingestion -> Store
```

## Required Evidence

- Working question-and-answer flow.
- At least one stored conversation.
- A document ingestion run with visible records.
- A response grounded in retrieved content.
- A learner explanation of every block and boundary.
- A debugging log for one failure.

## Success Criteria

The system works on the agreed sample data, failures are communicated clearly, and the learner can explain the complete request and data flow without relying on tool-specific vocabulary.
