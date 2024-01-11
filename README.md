# AI Swarm - Conductor

This is the main application that runs the AI Swarm. It is responsible for managing the agents, skills, and orchestrating the communication between them.

This is the easiest way to get your own agent swarm up and running.

## Getting Started

### Prerequisites

* [Node.js](https://nodejs.org/en/) - JavaScript runtime
* Git - Version control system
* Access to a supported LLM. Right now only [OpenAI](https://openai.com/) is supported, but plans to include AWS Bedrock and other services are underway.

### Installing

You can install the conductor as a binary using npm:

```bash
npm install -g @aiswarm/conductor
conductor run  --help
```

Or you can install it in a folder and run it from there:

```bash
npx @aiswarm/conductor run --help // this will install it automatically and run it
```

## Running

To run the conductor, you need to provide a config file. You can use the example config file as a starting point. More configs can be found in the [configs](https://github.com/aiswarm/configs) repository.

```bash