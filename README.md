# LLM-DPO-FineTuning
# TinyLlama DPO Training
Fine-tuning the TinyLlama-1.1B-Chat model using **Direct Preference Optimization (DPO)** on the Intel/Orca dataset to improve chat-style responses.

## Usage
1. Load the dataset and select a subset for training and evaluation.
2. Load model and tokenizer.
3. Train with DPO using provided configuration.
4. Evaluate the model on sample prompts.

## Sample Results

### Before DPO
| Sample | Output Analysis |
|--------|----------------|
| 0      | Correct but no summarization. |
| 5      | Complete answer to NFL question. |
| 10     | Correct, identified how Dillon accesses bread. |
| 20     | Incorrect, confused Alka-Seltzer ingredients with brand ownership. |
| 25     | Incorrect Desktop Publishing choice. |
| 30     | Complete answer about Clause. |

### After DPO
| Sample | Output Analysis |
|--------|----------------|
| 0      | Improved, summarization suggested. |
| 5      | More concise and accurate NFL response. |
| 10     | Dillon response more precise. |
| 20     | Alka-Seltzer response formal and complete. |
| 25     | Desktop Publishing response correct. |
| 30     | Clause response unchanged, already accurate. |
