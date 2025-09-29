# Medical Triage Model Comparison

## Experimental Design
- **Dataset**: 50 ESI-stratified emergency cases (8 ESI-1, 20 ESI-2, 15 ESI-3, 5 ESI-4, 2 ESI-5)
- **Models**: Claude Sonnet 4, GPT-5, Grok-3
- **Metric**: Sensitivity on ESI-2 cases (high-risk, non-immediate presentations)
- **Hypothesis**: Testing systematic undertriage patterns in LLM-based triage

## Reproduction Instructions
1. Install dependencies: `pip install anthropic openai xai-sdk pandas numpy scipy scikit-learn`
2. Set API keys in notebook
3. Run all cells (execution time: ~5 minutes with rate limiting)

## Key Findings
[Your results summary - keep it factual]

## Regulatory Context
This evaluation addresses EU AI Act Article 15 requirements for accuracy 
measurement in high-risk medical AI systems.
