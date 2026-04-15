# Instructional-Delta-Synthesis-Challenge-
This was a competition on who can best formulate complete prompts from jumbled words in a dataset. 

# Overview

Large Language Models often fail because of a "contextual gap" between user intent and model understanding. 
Expert prompt engineers bridge this gap by identifying the specific missing instructions—the Instructional 
Delta—that steer the model toward a high-quality result.

This dataset consists of 14,000 instruction-outcome pairs curated from a diverse range of domains including 
software engineering, creative writing, and technical QA. Each entry was constructed by human experts who 
analyzed an original, vague prompt and its suboptimal LLM output, then authored the precise "delta" of instructions 
needed to elicit the ideal target response.

In this challenge, you are performing Instructional Delta Synthesis. Given an initial user intent and a 
successful target response, your task is to synthesize the missing instructions, constraints, and formatting rules that bridge the gap.

# Dataset

The dataset contains 14,000 instruction-outcome pairs.

Files:

train.csv: Contains ~11,900 rows with the instructional_delta target variable.

test.csv: Contains ~2,100 rows. The instructional_delta target variable is withheld.

sample_submission.csv: A template for your predictions.

Columns (Data Types):

row_id (String): A deterministic 12-character unique hash.

original_prompt (String): The initial, vague user instruction (typically 10-100 words).

target_output (String): The successful, high-quality response (typically 50-500 words).

instructional_delta (String): [TARGET VARIABLE] The synthesized missing instructions (free-text string, typically 20-200 words).
