# AI Architecture

## Platform
Amazon Bedrock.

## Model strategy
- Claude Sonnet: complex reasoning and high-value analysis.
- Amazon Nova: suitable high-volume/low-latency tasks.
- Titan Embeddings: semantic retrieval where appropriate.

## Agents
### Staffing Agent
Parse job requirements, retrieve candidates, analyze documents, recommend and explain shortlists. Human review remains required for consequential decisions.

### Learning Agent
Analyze performance, identify gaps, recommend next activities and adapt practice.

### Marketing Agent
Draft campaigns, audience segments, content variations and performance summaries.

### Management Assistant
Answer authorized business questions and summarize KPIs.

AI credentials remain server-side behind an AI gateway. Enforce authorization before retrieval and log appropriate AI actions.
