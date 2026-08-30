# Libre WebUI Runtipi App Store

Official [Runtipi](https://runtipi.io) app store for [Libre WebUI](https://librewebui.org) — a privacy-first, self-hosted AI platform: chat with local models via Ollama or cloud providers, plus agents, automations, and a knowledge base.

The main Runtipi app store no longer accepts new applications, so Libre WebUI ships through this dedicated store instead. Same format, and updates land here the moment a release ships.

## Install

1. In Runtipi, go to **Settings → App Stores** and add:

   ```
   https://github.com/libre-webui/runtipi-appstore
   ```

2. Find **Libre WebUI** in the store and install it.
3. Open the app and create the first account — it becomes the administrator.

Runs on `amd64` and `arm64`.

## Ollama (optional)

Libre WebUI works out of the box with cloud providers configured in-app. For local models, install one of Runtipi's Ollama apps (`ollama-cpu`, `ollama-amd`, `ollama-nvidia`) and set the Ollama URL field in this app's settings to that app's service URL, e.g. `http://ollama-cpu:11434`.

Note: the Work sandboxed task-container feature is disabled in this packaging because it requires Docker socket access this packaging does not grant. Everything else works normally.

## License

[Apache-2.0](https://github.com/libre-webui/libre-webui/blob/main/LICENSE), same as Libre WebUI itself.
