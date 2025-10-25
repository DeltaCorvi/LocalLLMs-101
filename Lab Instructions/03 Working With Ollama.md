---
author: Bronwen Aker
updated: 2025-09-29
presentation_type: Workshop
venue: WWHF - Deadwood
---
```table-of-contents
title: # Table of Contents
minLevel: 0
maxLevel: 3
```


## Installing Ollama 

[Ollama](https://ollama.com/) is an excellent way to get started with using and customizing local LLMs. It is available on multiple platforms, is easy to install, has extensive documentation, and is well supported. 

> [!NOTE]
> This VM has been customized so that Ollama and Msty can share the same LLM models. Details for how this was done can be found [here](https://github.com/ollama/ollama/issues/10246).

To install Ollama on Linux, run the following command:

```shell
curl -fsSL https://ollama.com/install.sh | sh
```

### Start Ollama:

```shell
ollama serve
```

In another terminal, verify that Ollama is running:[^1]

```shell
ollama -v
```

To see what models are available, run the following command:

```bash
ollama list
```

### Pull a model

```shell
ollama pull llama3.2
```

This command can also be used to update a local model. Only the diff will be pulled.

> [!NOTE]
> You should have at least 8 GB of RAM available to run the 7B models, 16 GB to run the 13B models, and 32 GB to run the 33B models.

### Remove a model

```shell
ollama rm llama3.2
```

### Copy a model

```shell
ollama cp llama3.2 my-model
```



## Creating a Custom Model

While there is a lot to be said for training your own model from the ground up, doing so is labor and resource intensive. Using Ollama, it is possible to take an existing model and customize it using simple text file called a modelfile.

Create a `Modelfile`:

```
FROM llama3.2

# set the temperature to 1 [higher is more creative, lower is more coherent]
PARAMETER temperature 1

# set the system message
SYSTEM """
You are Mario from Super Mario Bros. Answer as Mario, the assistant, only.
"""
```

Next, create and run the model:

```
ollama create mario -f ./Modelfile
ollama run mario
>>> hi
Hello! It's your friend Mario.
```

For more information on working with a Modelfile, see the [Modelfile](docs/modelfile.md) documentation.

## CLI Reference

### Create a model

`ollama create` is used to create a model from a Modelfile.

```shell
ollama create mymodel -f ./Modelfile
```







![[Keeping Things Local/WWHF Deadwood 2025/Lab Instructions/assets/Keeping Things Local - SCaLE 2025.04 - Ollama Demos.mp4]]











### Footnotes
---

[^1]: Running `ollama serve` is not always necessary. For example, if you are running Ollama on a macOS system, there is a high likelihood that you won't need to run the `olama serve` command. FYI. 
