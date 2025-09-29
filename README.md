# Medical Triage Model Comparison

## Experimental Design
- **Dataset**: 50 ESI-stratified synthetic emergency cases extracted from examples in the ESI Handbook v.5. (8 ESI-1, 20 ESI-2, 15 ESI-3, 5 ESI-4, 2 ESI-5)
- **Models**: Claude Sonnet 4, GPT-5, Grok-3
- **Metric**: Sensitivity on ESI-2 cases (high-risk, non-immediate presentations)
- **Hypothesis**: Testing systematic undertriage patterns in LLM-based triage

## Reproduction Instructions
1. Install dependencies: `pip install anthropic openai xai-sdk pandas numpy scipy scikit-learn`
2. Set API keys in notebook
3. Run all cells (execution time: ~5 minutes with rate limiting)

## Key Findings


| Model  | Overall Accuracy | ESI2 Undertriage analysis (sensitivity) |
| ------------- | ------------- | ------------- |
| Claude 4  | 86.9%  | 70.0%  |
| GPT-5  | 86.0%  | 100.0%  |
| Grok-3  | 90.0%  | 75.0%  |


| Model  | Inter-model reliability (Cohen's Kappa) | 
| ------------- | ------------- | 
| Claude 4-GPT-5  | -0.163  | 
| Claude 4-Grok-3 | 0.811  | 
| GPT-5 - Grok-3  | -0.132  | 


## Regulatory Context
This evaluation addresses EU AI Act Article 15 requirements for accuracy 
measurement in high-risk medical AI systems.
