[![npm version](https://badge.fury.io/js/%40aiswarm%2Fconductor.svg)](https://badge.fury.io/js/%40aiswarm%2Fconductor)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Downloads](https://img.shields.io/npm/dm/%40aiswarm%2Fconductor.svg)](https://npmjs.com/package/%40aiswarm%2Fconductor)
[![Issues](https://img.shields.io/github/issues-raw/aiswarm/conductor)](https://github.com/aiswarm/conductor/issues)
[![Known Vulnerabilities](https://snyk.io/test/github/aiswarm/conductor/badge.svg)](https://snyk.io/test/github/aiswarm/conductor)
# AI Swarm - Conductor

This is the main application that runs the AI Swarm. It is responsible for managing the agents, skills, and orchestrating the communication between them.

This is the easiest way to get your own agent swarm up and running.

## Getting Started

### Prerequisites

* [Node.js](https://nodejs.org/en/) - JavaScript runtime
* Git - Version control system
* Access to a supported LLM. Right now only [OpenAI](https://openai.com/) is supported, but plans to include AWS Bedrock and other services are underway.

### Installing & Running

You can install the conductor as a binary using npm:

```bash
npm install -g @aiswarm/conductor
conductor run  --help
```

Or you can install it in a folder and run it from there:

```bash
npx @aiswarm/conductor run --help // this will install it automatically and run it
```

To run the conductor, you need to provide a config file. For more information on how to create your config, plus some sample configurations take a look at the  [configs](https://github.com/aiswarm/configs) repository.

## Recommended Setup for development with other plugins

You will need to link the plugin to the other plugins you want to use. So that you can make changes and see them immediately without having to publish the plugin to npm.

For this I recommend you create a new folder for the AI Swarm and clone all the plugins you want to use into it. Then link them together.

Each plugin has `link` script defined in the `package.json` file if there are dependencies on other packages.
You can run it with `npm run link` to link your code directly when you make changes.