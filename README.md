# Intro to Gaia Workshop Walkthrough

Last updated: May 21st

For today workshop, we will give a tutorial on how to install and setup a gaia node on a system.

I will be using Hyperbolic GPU rental service to run my node. However, you guys are welcome to use your own computer devices or other remote server to host your own node.

You can learn more about Hyperbolic GPU rental service here: https://app.hyperbolic.xyz/

They give $15 free credits for a new user account creation

I will be not be going over how to set up and connect to your own remote server for today's workshop for the sake of time.

# Install and set up your own Gaia node

Official documentation for reference here: https://docs.gaianet.ai/getting-started/quick-start

## Requirements:

| System                                 | Minimum Requirements        |
| -------------------------------------- | --------------------------- |
| OSX with Apple Silicon (M1-M4 chip)    | 16GB RAM (32GB recommended) |
| Ubuntu Linux 20.04 with Nvidia CUDA 12 | 8GB VRAM on GPU             |
| Azure/AWS                              | Nvidia T4 GPU Instance      |

You will also need to have the following system applications installed:

- `curl`
- `lsof`

# To Connect Your Node to a Knowledge Base

Official Documentation: https://docs.gaianet.ai/knowledge-bases/how-to/markdown

We will be using our club data and provide club information to the LLM to assist with answer questions about the club, using vectorized data :^)

## Prerequisites

Install the WasmEdge Runtime, the cross-platform LLM runtime.
```
curl -sSf https://raw.githubusercontent.com/WasmEdge/WasmEdge/master/utils/install_v2.sh | bash -s
```

Download an embedding model.

```
curl -LO https://huggingface.co/gaianet/Nomic-embed-text-v1.5-Embedding-GGUF/resolve/main/nomic-embed-text-v1.5.f16.gguf
```


