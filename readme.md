# LLM Testing with Promptfoo
This repository contains an example Promptfoo test framework for using the Ollama API to interact with and test the Meta Llama2 LLM. You can read the associated blog post on [The Quality Duck](https://www.thequalityduck.co.uk/how-to-automate-your-prompt-engineering-matrix-with-promptfoo/) website.

## Running the tests

You will need an instance of Ollama running Llama 2 running locally to run theses tests.

To get started, install promptfoo
```
npm install -g promptfoo
```

Then run:
```
promptfoo eval
```

Afterwards, you can view the results by running 

```
promptfoo view -y
```

## Example tests
There are 2 sets of example tests:

- promptfooconfig.yaml contains examples using the huggingface api to provide quality measures.
- promptfooconfig-maths.yaml contains examples using the LLM-rubric approach to assessing the answers

When running the tests as described above, promptfoo will run the promptfooconfig.yaml file.
To run the -maths examples, you must rename the file to promptfooconfig.yaml.
