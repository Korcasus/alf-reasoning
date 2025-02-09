# alf-reasoning
[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/Korcasus/alf-reasoning/blob/main/README.md)
[![kr](https://img.shields.io/badge/lang-kr-yellow.svg)](https://github.com/Korcasus/alf-reasoning/blob/main/README-KR.md)

> [!IMPORTANT]
> Translated by ChatGPT, may contain inaccuracies.

This workflow is designed to extract only the reasoning output from LLM models available in Alfred.
Once reasoning is complete, the subprocess that handles API responses is terminated to minimize output costs.
The models currently supported are deepseek-r1 and perplexity sonar reasoning.
For deepseek-r1, the workflow is restricted to using only the DeepSeek and DeepInfra providers to further reduce API usage costs.

The code will be updated at a later date.

## How to use
- In Alfred, type “rs” to bring up the workflow and hit enter. 
- A TextView component will appear with a prompt input field at the bottom. 
- Enter the prompt for the reasoning (CoT) you wish to generate, then press enter. 
- Wait a moment for the output to begin. Even if you accidentally close the window, you can re-enter the workflow and confirm that it’s still in progress. 
- Once completed, a footer will appear below the input field indicating that the process is finished. 
- To input a new prompt, use cmd + enter. To copy the generated reasoning, use control + enter.

## Requirements
- Alfred version 5.5 or later
- Python 3
- nRouter API Key

## Installation
Download the Alfred workflow from the release page and run it.

## Demo
![blank](./imgs/demo.gif)