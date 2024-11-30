# Perplexity-Permutation-Puzzle-Kaggle2024

Help Rudolph descramble holiday-related words to make the LLMs happy!

## To-Do List/Agenda

### **Day 1: Understand the Competition**

1. Read the competition overview and evaluation metric.
2. Explore the dataset:
   - Review `sample_submission.csv` to understand the input format.
3. Set up the environment:
   - Install required libraries: `torch`, `transformers`, `numpy`, `pandas`.
   - Test GPU/TPU availability.

### **Day 2: Build a Baseline**

1. Write a script to:
   - Load `sample_submission.csv`.
   - Shuffle the words in each row randomly.
2. Validate the output:
   - Ensure the format matches submission requirements.
   - Check that all outputs are valid permutations of the input.
3. Make a baseline submission to the leaderboard.

### **Day 3: Set Up Local Validation**

1. Save the official evaluation metric code in your workspace.
2. Test the metric:
   - Run it on a small sample dataset.
   - Debug any issues with formatting or invalid permutations.
3. Create a reusable validation pipeline:
   - Compare generated outputs against the evaluation metric.
   - Automate validation checks for future use.
