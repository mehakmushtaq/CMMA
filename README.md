# CMMA: Causal Mental-Model Alignment for Concept-Based Explanations

This repository contains the implementation of a concept-based explanation pipeline that aligns a model-derived causal graph with a human/clinical causal graph. The goal is to generate explanations that are both faithful to the trained predictive model and cognitively aligned with clinical reasoning.

## Overview

The method builds and compares three main causal graphs:

Model Causal Graph (MCG):A graph derived from the behavior of a trained machine learning model using concept-level interventions.

Human Causal Graph (HCG):A graph derived from LLM-generated clinician-style causal reasoning over a fixed set of predefined concepts.

Cognitively Aligned Causal Graph (CACG):A graph that combines the model-derived MCG and the human-derived HCG to produce explanations that are both model-faithful and clinically interpretable.

The final explanations are generated at the patient/instance level using the CACG graph.
