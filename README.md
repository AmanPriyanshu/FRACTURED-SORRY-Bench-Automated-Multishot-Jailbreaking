# FRACTURED-SORRY-Bench

## Framework for Revealing Attacks in Conversational Turns Undermining Refusal Efficacy and Defenses over SORRY-Bench

This repository contains the code and data for the FRACTURED-SORRY-Bench framework, as described in our paper.

### Abstract

FRACTURED-SORRY-Bench is a framework for evaluating the safety of Large Language Models (LLMs) against multi-turn conversational attacks. Building upon the SORRY-Bench dataset, we propose a simple yet effective method for generating adversarial prompts by breaking down harmful queries into seemingly innocuous sub-questions.

### Key Results

Vanilla Responses:

| Model      | Harmful & Relevant | Harmful but Irrelevant | Harmless | ASR (%) |
|------------|--------------------|-----------------------|----------|---------|
| GPT-4o     | 52                 | 3                     | 395      | 11.56   |
| GPT-3.5    | 21                 | 4                     | 425      | 4.67    |
| GPT-4o-mini| 58                 | 2                     | 390      | 12.89   |
| GPT-4      | 45                 | 3                     | 402      | 10.00   |

Decomposed Responses:

| Model      | Harmful & Relevant | Harmful but Irrelevant | Harmless | ASR (%) |
|------------|--------------------|-----------------------|----------|---------|
| GPT-4o     | 223                | 103                   | 124      | 49.56   |
| GPT-3.5    | 229                | 106                   | 115      | 50.89   |
| GPT-4o-mini| 226                | 106                   | 118      | 50.22   |
| GPT-4      | 221                | 104                   | 125      | 49.11   |

Our approach achieves significant increases (6X) in Attack Success Rates (ASRs) across multiple models

### Repository Structure

- `data/`: Contains the FRACTURED-SORRY-Bench dataset creation code.
- `evaluations/`: Contains evaluation code scripts.
- `responses/`: Contains response results from the dataset, as well as the evaluations.

### Usage

For experiment replication employ the  `mutator.py` file within `data/`.

```shell
python3 mutator.py
```

## Cite This Work

```
@inproceedings{FRACTURED-SORRY-Bench,
  title = {FRACTURED-SORRY-Bench: Framework for Revealing Attacks in Conversational Turns Undermining Refusal Efficacy and Defenses over SORRY-Bench},
  author = {Aman Priyanshu, Supriti Vijay},
  year = {2024},
  publisher = {{GitHub}},
  url = {https://github.com/AmanPriyanshu/FRACTURED-SORRY-Bench}
}

```

## Contributions and Feedback

Contributions, suggestions, and feedback are welcome! If you have any ideas to enhance the repository or encounter any issues, please feel free to open an issue or submit a pull request on the GitHub repository. Thank you for your interest in this research work and project. We hope "FRACTURED-SORRY-Bench" proves to be a valuable resource.

## Other Usage Details

### Attribution

* If you use or share this work, please provide attribution with the following information:

_"FRACTURED-SORRY-Bench" by Aman Priyanshu and Supriti Vijay, licensed under CC BY-NC 4.0. Available at: https://github.com/AmanPriyanshu/FRACTURED-SORRY-Benchs_

* When sharing adaptations of this work, please include a statement indicating that changes were made, such as:

_This work is adapted from "FRACTURED-SORRY-Bench" by Aman Priyanshu and Supriti Vijay, licensed under CC BY-NC 4.0. Original work available at: https://github.com/AmanPriyanshu/FRACTURED-SORRY-Bench_

### License
This work is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.

TL;DR: My projects are licensed under CC BY-NC 4.0, which means you can freely use them for non-commercial purposes with attribution. If you're considering commercial use or are unsure whether your use case requires permission, please refer to the [LICENSE](/LICENSE) file or reach out to me via [email](amanpriyanshusms2001@gmail.com)—I'm always happy to chat!
