# LLM Math and Moral Reasoning
LLM Reasoning: A preliminary study on mathematical and moral reasoning

This project is a part of a preliminary study done using MMLU benchmark using Mistral 8x7B LLM

Data: Measuring Massive Multitask Language Understanding (Hendrycks et al., 2020)
Task: Elementary Mathematics and Moral Scenarios
Test data: A randomly generated sample of 100 instances from test data of MMLU moral scenarios and elementary mathematics

Results:
## RQ1 
Here the max_tokens parameter is set to 1 for LLM generation
### Elementary Math
|   Prompt type    | Accuracy | Invalid answers |
| ---------------- | -------- | --------------- |
|    Zero-shot     |    16%   |        71%      |
|  Random one-shot |    35%   |        12%      |
|Random three-shot |    39%   |        13%      |
| Dynamic one-shot |    38%   |        10%      |
|Dynamic three-shot|    40%   |        13%      |

### Moral Scenarios
|   Prompt type    | Accuracy | Invalid answers |
| ---------------- | -------- | --------------- |
|    Zero-shot     |  29%     |      22%        |
|  Random one-shot |  47%     |       1%        |
|Random three-shot |  48%     |       8%        |
| Dynamic one-shot |  40%     |       1%        |
|Dynamic three-shot|  53%     |       1%        |

## RQ2 
Here the max_tokens parameter is set to 256 for LLM generation
### Elementary Math
|        Prompt type           | Accuracy | Invalid answers |
| ---------------------------- | -------- | --------------- |
|        Zero-shot             |  57%     |       2%        |
|  Linguistic Chain-of-Thought |  49%     |       5%        |
|      Chain-of-Thought        |  56%     |       1%        |


### Moral Scenarios
|        Prompt type           | Accuracy | Invalid answers |
| ---------------------------- | -------- | --------------- |
|        Zero-shot             |  29      |         0%      |
|  Linguistic Chain-of-Thought |  28%     |         0%      |
|      Chain-of-Thought        |  26%     |         0%      |

