# Sourceblender

Sourceblender builds open infrastructure for AI agents that work together over
time: shared memory, an agent runtime, and real-time voice. It is built and run
every day on our own hardware.

Built by [Eric Mey](https://github.com/ericmey).

## Showcase

### Musubi: shared memory for AI agents

A memory server for a small fleet of agents, so that what one learns the others
can use. It has three memory planes, runs local inference, and has a lifecycle
engine that matures raw captures into a knowledge base a person can review.
Host adapters connect agents to Musubi. For the hosts it supports, the shared
harness supplies turn capture and verified delivery.

| | Repository | Visibility · lifecycle |
| --- | --- | --- |
| Server | [ericmey/musubi](https://github.com/ericmey/musubi) | Public · released |
| Harness | [musubi-harness](https://github.com/sourceblender/musubi-harness) | Public · released |
| Claude Code | [musubi-claude](https://github.com/sourceblender/musubi-claude) | Public · released |
| Codex | [musubi-codex](https://github.com/sourceblender/musubi-codex) | Public · released |
| Grok Build | [musubi-grok](https://github.com/sourceblender/musubi-grok) | Public · developing |
| Hermes | [musubi-hermes](https://github.com/sourceblender/musubi-hermes) | Public · released |
| OpenClaw | [musubi-openclaw](https://github.com/sourceblender/musubi-openclaw) | Public · developing |
| LiveKit | [musubi-livekit](https://github.com/sourceblender/musubi-livekit) | Public · proof of concept |

### Chord: one model name, a team of specialists behind it

An OpenAI-compatible endpoint that routes each turn to a local specialist agent
(conversation, image, audio, search, video), each with its own prompt, model and
tools. Clients see one model; they never see the internal tool calls.
It runs in production here today. **Private · public release planned.**

### Voice: real-time voice and phone agents

A private house system in development: spoken conversation with agents, in real
time and over the phone, built on LiveKit and SIP. The public name is still to be
decided. **Private · public release planned.**

## Also from us

- [ComfyUI Immich](https://github.com/sourceblender/comfyui-immich): ComfyUI nodes
  that upload images to Immich, with metadata and album management.
- [ComfyUI Kotodama](https://github.com/sourceblender/comfyui-kotodama): a ComfyUI
  node that enhances text-to-image prompts through any OpenAI-compatible
  endpoint.

## Status labels

Two separate things: who can see it, and how far along it is.

- **Visibility:** *public* (source open), *private*, or *public release planned*.
- **Lifecycle:** *proof of concept*, *developing*, *released* (has a published
  release), *maintained*, or *archived*.

Start with a project's README for installation and support. Report security
issues through that repository's `SECURITY.md`, or the
[organization default](https://github.com/sourceblender/.github/blob/main/SECURITY.md).
