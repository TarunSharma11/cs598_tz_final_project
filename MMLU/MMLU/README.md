This is adapted from original simple-eval implementation to evaluate our ablations.


Environment:
Use the original simple-eval to create the environment: https://github.com/openai/simple-evals.

Change this import manually in simple_evals.py for different ablations
from .mmlu_eval import MMLUEval

For shuffled dataset change to: from .mmlu_eval_shuffled import MMLUEval

For none ablation dataset change to: from .mmlu_eval_none_ablation import MMLUEval


Run to evaluate mmlu:

python -m mmlu.simple_evals --model gpt-4o-mini