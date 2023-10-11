# Assessing the Effectiveness of AI Writing Detectors
### Table of Contents

    Project Overview
    Methods Summary
    Usage
    Installation
    Credits

### Project Overview

This Python project aims to automate the evaluation and generation of essays using various AI models and online essay checkers. It provides methods to assess the authenticity of essays and generate new ones. The project is designed to be user-friendly, allowing users to evaluate essays, generate content, and visualize the results.

### Methods Summary

This project includes the following main methods:

    writer_checker(text)
        Scores an essay as AI-generated or human-generated using Writer.com checker.

    crossplag_checker(text_list)
        Scores a list of essays as AI-generated or human-generated using CrossPlag.com checker.

    sapling_checker(text_list)
        Scores a list of essays as AI-generated or human-generated using Sapling.ai checker.

    zerogpt_checker(text_list)
        Scores a list of essays as AI-generated or human-generated using ZeroGPT.com checker.

    generate_gpt(title, tone)
        Generates an essay with the GPT-3.5 model given a title and tone.

    generate_essays(prompt_list, tone_list)
        Generates essays with the Davinci model and returns a DataFrame of the essays along with their AI checker scores.

    human_essay_checker()
        Checks AI detection scores for human-generated essays.

    graph_results(generation, cat, analysis)
        Generates various graphs based on specific criteria such as method of essay generation, category, and analysis type.

    graph_results_by_checker(generation, analysis)
        Generates graphs comparing the performance of different checkers for AI or human-generated content.

    graph_score_distribution(generation)
        Generates a graph displaying the score distribution of each checker for AI or human content.

    graph_comparison()
        Generates a comparison graph of checker performance for AI vs. human content.

    graph_all(generation, analysis)
        Simultaneously generates four graphs, displaying all four categories of analysis.

    confusion_matrix(checker)
        Generates a confusion matrix for a specific checker.

    graph()
        User interface method to generate any desired graphs.

### Usage

The project provides methods to evaluate essays, generate content, and visualize results. To get started, you can call the relevant methods with appropriate arguments based on your specific use case.

### Installation

To use this project, ensure you have the necessary Python libraries installed. You can install these libraries using pip:

pip install openai pandas selenium requests matplotlib seaborn

Additionally, you will need to set up your OpenAI API key by replacing the placeholder in the code with your actual API key. You must do the same for Writer checker API.

### Credits
Created with Ryan Demolina and Ian DeLano

