
2023 CSV of LLMs [here](./LLMs.csv).

## Coding & Open Weights

We maintain a guide on how to deploy an open-source code LLMs [here](https://github.com/continuedev/deploy-os-code-llm).

### Open Source

This is a list of the **open-source** LLMs that developers are using while coding, roughly ordered from most popular to least popular, as of October 2023.

#### 1. Code Llama

[Code Llama](https://about.fb.com/news/2023/08/code-llama-ai-for-coding/) is an LLM trained by Meta for generating and discussing code. It is built on top of Llama 2. Even though it is below WizardCoder and Phind-CodeLlama on the [Big Code Models Leaderboard](https://huggingface.co/spaces/bigcode/bigcode-models-leaderboard), it is the base model for both of them. It also comes in a variety of sizes: 7B, 13B, and 34B, which makes it popular to use on local machines as well as with hosted providers. At this point, it is the most well-known open-source base model for coding and is leading the open-source effort to create coding capable LLMs.

<details>
    <summary>Details</summary>

    Creator: Meta
    Date released: August 24th, 2023
    License: Llama 2 Community
    Base model: Llama 2
    Parameters: 7B, 13B, 34B

</details>

#### 2. WizardCoder

[WizardCoder](https://github.com/nlpxucan/WizardLM/tree/main/WizardCoder) is an LLM built on top of Code Llama by the WizardLM team. The [Evol-Instruct method](https://x.com/WizardLM_AI/status/1705551243421090207?s=20) is adapted for coding tasks to create a training dataset, which is used to fine-tune Code Llama. It comes in the same sizes as Code Llama: 7B, 13B, and 34B. As a result, it is the most popular open-source instruction-tuned LLM so far.

<details>
    <summary>Details</summary>
    
    Creator: WizardLM
    Date released: August 26th, 2023
    License: Llama 2 Community
    Base model: Code Llama
    Parameters: 7B, 13B, 34B
    
</details>

#### 3. Phind-CodeLlama

[Phind-CodeLlama](https://www.phind.com/blog/code-llama-beats-gpt4) is an LLM built on top of Code Llama by Phind. A proprietary dataset of ~80k high-quality programming problems and solutions was used to fine-tune Code Llama. That fine-tuned model was then further fine-tuned on 1.5B additional tokens. It currently leads on the [Big Code Models Leaderboard](https://huggingface.co/spaces/bigcode/bigcode-models-leaderboard). However, it is only available as a 34B parameter model, so it requires more available memory to be used.

<details>
    <summary>Details</summary>
    
    Creator: Phind
    Date released: August 28th, 2023
    License: Llama 2 Community
    Base model: Code Llama
    Parameters: 34B

</details>

#### 4. Mistral

[Mistral](https://mistral.ai/news/announcing-mistral-7b) is a 7B parameter LLM trained by Mistal AI. It is the most recently released model on this list, having dropped at the end of September. Mistal AI says that it “approaches CodeLlama 7B performance on code, while remaining good at English tasks”. Despite only being available in the one small size, people are quite excited about it in the first couple weeks after release. The first fine-tuned LLMs that use it as their base are now beginning to emerge, and we are likely to see more going forward.

<details>
    <summary>Details</summary>
    
    Creator: Mistral AI
    Date released: September 27th, 2023
    License: Apache 2.0
    Base model: Mistral
    Parameters: 7B
    
</details>

#### 5. StarCoder

[StarCoder](https://huggingface.co/blog/starcoder) is a 15B parameter LLM trained by BigCode, which was ahead of its time when it was released in May. It was trained on 80+ programming languages from The Stack (v1.2) with opt-out requests excluded. It is not an instruction model and commands like "Write a function that computes the square root" do not work well. However, by using the [Tech Assistant prompt](https://huggingface.co/datasets/bigcode/ta-prompt) you can make it more helpful.

<details>
    <summary>Details</summary>
    
    Creator: BigCode
    Date released: May 4th, 2023
    License: OpenRAIL-M
    Base model: StarCoder
    Parameters: 15B
    
</details>

#### 6. DeepSeek Coder

[DeepSeek Coder](https://deepseekcoder.github.io) is an LLM trained by DeepSeek AI on 2 trillion tokens. With a dataset made up of over more than 80 programming languages, it's the newest model on this list and has been reported to score quite high on various coding-related benchmarks.

<details>
    <summary>Details</summary>
    
    Creator: DeepSeek AI
    Date released: November 3rd, 2023
    License: DeepSeek License Agreement
    Base model: DeepSeek Coder
    Parameters: 1.3B, 6.7B, 33B
    
</details>

#### 7. Llama2

[Llama 2](https://ai.meta.com/llama/#inside-the-model) is an LLM trained by Meta on 2 trillion tokens. It is the most popular open source LLM overall, so some developers use it, despite it not being as good as many of the models above at making code edits. It is also important because Code Llama, the most popular LLM for coding, is built on top of it, which in turn is the foundation for WizardCoder and Phind-CodeLlama.

<details>
    <summary>Details</summary>
    
    Creator: Meta
    Date released: July 18th, 2023
    License: Llama 2 Community
    Base model: Llama 2
    Parameters: 7B, 13B, 70B
    
</details>

