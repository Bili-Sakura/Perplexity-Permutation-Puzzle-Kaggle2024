# Overview

## Description

Minimizing perplexity, a task quite grand,
A neural network’s mission, across the land.
A model, trained on texts, both vast and deep,
To rearrange the words, while others sleep.
It sorts and sifts, with algorithms bright,
To find the clearest path, the words made right.
A digital reindeer, with circuits aglow,
Reducing confusion, a wondrous show.
No longer puzzled, the reader’s mind at ease,
As the model’s magic, effortlessly, please.
A gift of clarity, a present divine,
A neural network’s work, a clever design.

## The Challenge

Just like those mischievous elves who mixed up the ornaments on Santa's Christmas tree, someone has scrambled the words in classic Christmas tales! Your task, dear Kagglers, is to put those words back in order, minimizing the perplexity of each passage. The lower the perplexity, the more sense the story makes!

## The Data

Rudolph has provided a sleigh-full of jumbled text passages, each one a beloved Christmas story in disarray. He's even included a special metric to guide you, a measure of how puzzled a reader would be by the mixed-up words.

## The Goal

Use your coding magic and linguistic skills to rearrange the words, making the stories flow smoothly and beautifully once more. The Kagglers who achieve the lowest perplexity scores will win Rudolph's heart and earn a place on the leaderboard!

So join Rudolph and his friends in this festive challenge! Untangle the words, spread Christmas cheer, and help make this a holiday to remember!

## Evaluation

Submissions to this competition are evaluated by their Average Perplexity, with lower scores ranked better.

Submissions comprise texts that are permutations of words given in the `sample_submission.csv` file. We compute the perplexity of each submitted sequence of words with respect to the Gemma 2 9B model. Your final score is the average perplexity across all sequences.

You may view the evaluation metric in this notebook: [Santa 2024 Metric](../notebooks/【Official】Santa-2024-Metric.ipynb).

## Submission File

For each `id`, the submission file should contain a sequence of words in the `text` field. Each sequence must be attainable by a permutation of the corresponding "base" sequence of words in the `sample_submission.csv` file. For example, if the base sequence is `a b c`, then the submitted sequence could be `a b c`, `a c b`, `b a c`, `b c a`, `c a b`, or `c b a`, but the submitted sequence could not be `b a` or `a a b` or `a b c b`. Such sequences are invalid and will fail scoring.

The `submission.csv` file should contain a header and have the following format:

```csv
id,text
0,advent chimney elf family ...
1,fireplace gingerbread mistletoe ...
2,yuletide decorations gifts ...
...
```

## Timeline

- **November 21, 2024** - Start Date.
- **January 24, 2025** - Entry Deadline. You must accept the competition rules before this date in order to compete.
- **January 24, 2025** - Team Merger Deadline. This is the last day participants may join or merge teams.
- **January 31, 2025** - Final Submission Deadline.

All deadlines are at 11:59 PM UTC on the corresponding day unless otherwise noted. The competition organizers reserve the right to update the contest timeline if they deem it necessary.

## Prizes

- **First Prize**: $12,000
- **Second Prize**: $10,000
- **Third Prize**: $10,000
- **Fourth Prize**: $8,000
- **Rudolph Prize - $10,000**: Awarded to the team holding 1st place on the leaderboard for the longest period of time between November 21, 2024 12:00 AM UTC and January 31, 2025 11:59 PM UTC. In the event the competition needs to be restarted, the Rudolph Prize dates shall be the new start and deadline of the competition.

As a condition to being awarded a Prize, a Prize winner must provide a detailed write-up on their solution in the competition forums within 14 days of the conclusion of the competition.

## Citation

Ryan Holbrook, Walter Reade, Maggie Demkin, and Elizabeth Park. Santa 2024 - The Perplexity Permutation Puzzle. [https://kaggle.com/competitions/santa-2024](https://kaggle.com/competitions/santa-2024), 2024. Kaggle.
