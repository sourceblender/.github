# Sourceblender

Sourceblender builds open infrastructure for AI agents that work together over
time: shared memory, an agent runtime, and real-time voice. It is built and run
every day on our own hardware.

## Showcase

### Musubi: shared memory for AI agents

A memory server for a small fleet of agents, so that what one learns the others
can use. It has three memory planes, runs local inference, and has a lifecycle
engine that matures raw captures into a knowledge base a person can review.
Every agent host connects through the same harness, which captures each
exchange, delivers it, and reads it back before calling it saved.

| | Repository | Status |
| --- | --- | --- |
| Server | [ericmey/musubi](https://github.com/ericmey/musubi) | Public, released |
| Harness | [musubi-harness](https://github.com/sourceblender/musubi-harness) | Public, released |
| Claude Code | [musubi-claude](https://github.com/sourceblender/musubi-claude) | Public, released |
| Codex | [musubi-codex](https://github.com/sourceblender/musubi-codex) | Public, released |
| Grok Build | [musubi-grok](https://github.com/sourceblender/musubi-grok) | Public |
| Hermes | [musubi-hermes](https://github.com/sourceblender/musubi-hermes) | Public, released |
| OpenClaw | [musubi-openclaw](https://github.com/sourceblender/musubi-openclaw) | Public |
| LiveKit | [musubi-livekit](https://github.com/sourceblender/musubi-livekit) | Public, early |

### Chord: one model name, a team of specialists behind it

An OpenAI-compatible endpoint that routes each turn to a local specialist agent
(conversation, image, audio, search, video), each with its own prompt, model and
tools. Clients see one model; they never see the internal tool calls.
**Public later:** it runs in production here today, and the repository is not
open yet.

### Voice: real-time voice and phone agents

Spoken conversation with agents, in real time and over the phone, built on
LiveKit and SIP. The public name is still to be decided. **Public later.**

## Also from us

- [ComfyUI Immich](https://github.com/sourceblender/comfyui-immich): ComfyUI nodes
  that upload images to Immich, with metadata and album management.
- [ComfyUI Kotodama](https://github.com/sourceblender/comfyui-kotodama): a ComfyUI
  node that enhances text-to-image prompts through any OpenAI-compatible
  endpoint.

## Status labels

- **Released:** the source is public and has a published release.
- **Public:** the source is public; no release yet.
- **Early:** public and experimental; expect breaking changes.
- **Public later:** we intend to publish it, and it is not open yet.

Start with a project's README for installation and support. Report security
issues through that repository's `SECURITY.md`, or the
[organization default](https://github.com/sourceblender/.github/blob/main/SECURITY.md).
