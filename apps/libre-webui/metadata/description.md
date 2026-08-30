# Libre WebUI

Libre WebUI is a private, self-hosted AI chat platform. Point it at a local Ollama server for fully offline models, or bring your own API keys for cloud providers, all from a single interface backed by your own data on your own server.

## Features

- **Chat with local or cloud models:** talk to models served by Ollama, or connect cloud providers with your own API keys.
- **Agents:** configure persona-style agents for different tasks.
- **Automations:** schedule recurring runs and webhooks.
- **Knowledge base:** upload documents and retrieve from them during chat.
- **Your data, your server:** conversations, uploads and keys live in the app's data volume, nothing leaves your instance unless you configure a cloud provider.

## Getting started

On first visit, create an account, it automatically becomes the administrator. Signups are disabled after that, so share access by creating additional accounts from the admin panel.

Ollama is optional. Libre WebUI runs fine without it if you only use cloud providers; to use local models, set the "Ollama Base URL" field to a reachable Ollama server, for example one of the Ollama apps from this store, using its internal service name and port 11434.

## Notes on this packaging

Libre WebUI also includes an optional Work feature for running sandboxed browser/task agents in their own containers. That feature needs direct access to the Docker socket, which this packaging does not grant, so Work sandboxes are disabled here. Everything else (chat, agents, automations, knowledge) works normally.

## Links

- Website: https://librewebui.org
- Documentation: https://docs.librewebui.org
- Source: https://github.com/libre-webui/libre-webui
