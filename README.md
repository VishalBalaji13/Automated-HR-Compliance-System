Automated HR Compliance System
The Problem
Large Language Models (LLMs) frequently hallucinate internal corporate policies, creating significant liability risks for HR departments managing complex frameworks like Flexible Work Arrangements (FWA).

The Solution
To solve this, we developed a highly adaptable Dual-Layer Retrieval-Augmented Generation (RAG) architecture designed to automate and secure policy audits for any enterprise or university employee handbook.

Dynamic Two-Step Verification Pipeline
Our solution introduces a dynamic, two-step verification pipeline to ensure complete accuracy:

Layer 1: Contextual Retrieval & Rule Injection

Utilizes ChromaDB for contextual vector retrieval.

Employs a local Llama-3 "Critic" model to forcefully inject mandatory, institution-specific rules (such as managerial approval requirements) directly into the generated response.

Layer 2: Mathematical Firewall

Deploys a DeBERTa-v3 Natural Language Inference (NLI) model.

Calculates the entailment-versus-contradiction probability between the generated text and the source document, effectively and physically preventing policy hallucinations.

Deployment & Monitoring
Deployed via an enterprise-grade frontend with synchronous backend monitoring, this architecture guarantees strict policy enforcement across any organizational dataset.
