# Reinforcement Learning: Gold Reward-Based Text Generation

## Project Overview
This project explores a gold reward function for evaluating generated weather reports using Python.

## Objectives
- Create a small corpus of weather reports.
- Generate sentences using a corpus-based reference model.
- Calculate reward scores for generated sentences.
- Analyze how sentence length and numeric information affect rewards.

## Reward Function
Reward = Temperature Bonus - 0.1 × Number of Words

The temperature bonus is 1 if a sentence contains a numeric word and 0 otherwise. The special token `<eos>` is excluded from the word count.

## Technologies Used
- Python
- Google Colab
- GitHub

## How to Run
1. Open the notebook in Google Colab.
2. Run the code cells in order.
3. Observe the generated sentences and reward scores.

## Limitation
The reference model samples word transitions from the corpus. The basic implementation calculates reward scores but does not train a reinforcement learning policy.

## Conclusion
This experiment demonstrates how a reward function can evaluate short weather reports according to specified criteria.
