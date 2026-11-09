# 🎙️ Powerful Realtime Voice AI & Full-Duplex Speech-to-Speech (2026)

> **A battle-tested, live-monitored directory of open-source full-duplex speech-to-speech (S2S) models, ultra-fast neural TTS (<82M), streaming ASR, and WebRTC conversational agents.**
> *Updated automatically every 24 hours with live health-checks and latency benchmarks.*

[![Uptime](https://img.shields.io/badge/Monitored_Uptime-95.7%25-3fb950?style=for-the-badge&logo=statuspage)](https://github.com/dhaulagani/powerful-realtime-voice-ai) [![Verified Frameworks](https://img.shields.io/badge/Verified_Frameworks-23_Active-58a6ff?style=for-the-badge)](https://github.com/dhaulagani/powerful-realtime-voice-ai) [![Last Verified](https://img.shields.io/badge/Last_Check-2026-11-09_16:21_UTC-brightgreen?style=for-the-badge)](https://github.com/dhaulagani/powerful-realtime-voice-ai)

---

### 💡 Why Traditional Cascading Voice Stacks Are Obsolete
Legacy AI voice assistants relied on a sluggish three-step cascading pipeline:
```
[User Audio] ──> STT (Whisper) ──> Text LLM (GPT-4) ──> TTS (ElevenLabs) ──> [Audio Output]
                 (300ms - 600ms)     (600ms - 1500ms)       (400ms - 800ms)
Total Latency: 1.5s - 3.0s (Unacceptable awkward silence & zero natural interruption)
```

**The Modern Paradigm: Native Speech-to-Speech (S2S) & Sub-300ms Full-Duplex**:
- ⚡ **Zero-Silence Latency**: Audio tokens stream directly into acoustic decoders with sub-200ms latency.
- 🗣️ **Natural Interruption Handling**: Users can interrupt the agent mid-sentence, exactly like a human conversation.
- 🎭 **Emotional Vocalization**: Tone, sighs, cadence, and laughter are preserved natively rather than lost in text transcription.

---

## 📑 Table of Contents
- [End-to-End Speech-to-Speech (S2S) Models](#end-to-end-speech-to-speech-s2s-models)
- [Ultra-Fast Neural TTS Models](#ultra-fast-neural-tts-models)
- [Streaming Speech Recognition (ASR)](#streaming-speech-recognition-asr)
- [Real-Time Orchestration & WebRTC](#real-time-orchestration-webrtc)
- [Voice Activity Detection (VAD) & Turn-Taking](#voice-activity-detection-vad-turn-taking)

---
## End-to-End Speech-to-Speech (S2S) Models

| Framework / Model | Latency Target | Capability & Architecture | License | Health & Latency | Source & Docs |
| :--- | :---: | :--- | :---: | :--- | :--- |
| [Kyutai Moshi](https://kyutai.org/moshi) | `sub-200ms` | First open-source full-duplex speech-text foundation model (7B) with simultaneous listening and talking | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 1058ms` | [**GitHub / Docs ↗**](https://github.com/kyutai-labs/moshi) |
| [Mini-Omni 2](https://github.com/gpt-omni/mini-omni2) | `sub-300ms` | Real-time multimodal speech-to-speech conversational model with continuous acoustic listening & interruption | `MIT` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 1081ms` | [**GitHub / Docs ↗**](https://github.com/gpt-omni/mini-omni2) |
| [GLM-4-Voice (Zhipu AI)](https://github.com/THUDM/GLM-4-Voice) | `sub-300ms` | End-to-end voice reasoning model supporting emotional expressiveness, tone shifting, and streaming audio generation | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 1089ms` | [**GitHub / Docs ↗**](https://github.com/THUDM/GLM-4-Voice) |
| [Ultravox (Fixie.ai)](https://github.com/fixie-ai/ultravox) | `sub-200ms` | Open-weights multimodal speech LLM mapping audio encoders directly into Llama 3 with streaming output | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 657ms` | [**GitHub / Docs ↗**](https://github.com/fixie-ai/ultravox) |
| [LLaMA-Omni](https://github.com/ictnlp/LLaMA-Omni) | `sub-250ms` | Simultaneous low-latency speech interaction built on Llama-3.1 with instant acoustic decoding | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 585ms` | [**GitHub / Docs ↗**](https://github.com/ictnlp/LLaMA-Omni) |
| [Freeze-Omni](https://github.com/Vchitect/Freeze-Omni) | `sub-300ms` | Conversational speech model keeping LLM weights frozen while training low-latency cross-modal adapters | `Apache-2.0` | ![Degraded](https://img.shields.io/badge/Status-HTTP_404-d29922?style=flat-square) | [**GitHub / Docs ↗**](https://github.com/Vchitect/Freeze-Omni) |

## Ultra-Fast Neural TTS Models

| Framework / Model | Latency Target | Capability & Architecture | License | Health & Latency | Source & Docs |
| :--- | :---: | :--- | :---: | :--- | :--- |
| [Kokoro-82M (Hexgrad)](https://github.com/hexgrad/kokoro) | `sub-100ms` | 82M parameter ultra-compact TTS delivering ElevenLabs-grade human naturalness at 10x faster execution | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 665ms` | [**GitHub / Docs ↗**](https://github.com/hexgrad/kokoro) |
| [Outetts (OuteAI)](https://github.com/edwko/OuteTTS) | `sub-150ms` | Pure language-model architecture for voice synthesis using structured audio tokens without complex diffusion | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 631ms` | [**GitHub / Docs ↗**](https://github.com/edwko/OuteTTS) |
| [CosyVoice 2 (Alibaba)](https://github.com/FunAudioLLM/CosyVoice) | `sub-150ms` | Highly controllable multi-lingual speech generation with zero-shot voice cloning and emotional rhythm control | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 1054ms` | [**GitHub / Docs ↗**](https://github.com/FunAudioLLM/CosyVoice) |
| [F5-TTS](https://github.com/SWivid/F5-TTS) | `sub-200ms` | Non-autoregressive flow-matching speech synthesis offering fast zero-shot voice cloning and editing | `MIT` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 691ms` | [**GitHub / Docs ↗**](https://github.com/SWivid/F5-TTS) |
| [Fish-Speech (Fish Audio)](https://github.com/fishaudio/fish-speech) | `sub-150ms` | State-of-the-art text-to-speech with sub-second time-to-first-audio and cross-lingual voice transfer | `CC-BY-NC-SA-4.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 636ms` | [**GitHub / Docs ↗**](https://github.com/fishaudio/fish-speech) |
| [ChatTTS (2Noise)](https://github.com/2noise/ChatTTS) | `sub-200ms` | Conversational speech model designed specifically for dialogue with natural laughs, sighs, and interjections | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 563ms` | [**GitHub / Docs ↗**](https://github.com/2noise/ChatTTS) |

## Streaming Speech Recognition (ASR)

| Framework / Model | Latency Target | Capability & Architecture | License | Health & Latency | Source & Docs |
| :--- | :---: | :--- | :---: | :--- | :--- |
| [Faster-Whisper](https://github.com/SYSTRAN/faster-whisper) | `sub-100ms` | CTranslate2-powered Whisper running 4x faster with half the memory footprint for streaming transcription | `MIT` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 645ms` | [**GitHub / Docs ↗**](https://github.com/SYSTRAN/faster-whisper) |
| [Whisper.cpp](https://github.com/ggerganov/whisper.cpp) | `sub-50ms` | High-performance plain C/C++ implementation of Whisper optimized for Apple Silicon (Metal) and CPU SIMD | `MIT` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 1034ms` | [**GitHub / Docs ↗**](https://github.com/ggerganov/whisper.cpp) |
| [SenseVoice (Alibaba)](https://github.com/FunAudioLLM/SenseVoice) | `sub-70ms` | Ultra-fast multilingual speech recognition with audio event detection (cough, music, laughter) and sentiment | `MIT` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 1119ms` | [**GitHub / Docs ↗**](https://github.com/FunAudioLLM/SenseVoice) |
| [Distil-Whisper](https://github.com/huggingface/distil-whisper) | `sub-80ms` | Distilled, lightweight Whisper variants operating at 6x speed with 99% accuracy retention | `MIT` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 2181ms` | [**GitHub / Docs ↗**](https://github.com/huggingface/distil-whisper) |

## Real-Time Orchestration & WebRTC

| Framework / Model | Latency Target | Capability & Architecture | License | Health & Latency | Source & Docs |
| :--- | :---: | :--- | :---: | :--- | :--- |
| [LiveKit Agents](https://livekit.io/agents) | `sub-100ms` | Industry-standard real-time WebRTC framework for voice, video, and multimodal AI agents with native turn-taking | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 511ms` | [**GitHub / Docs ↗**](https://github.com/livekit/agents) |
| [Pipecat AI](https://www.pipecat.ai) | `sub-120ms` | Python open-source framework for building voice, video, and multimodal conversational agents over WebRTC | `BSD-2-Clause` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 163ms` | [**GitHub / Docs ↗**](https://github.com/pipecat-ai/pipecat) |
| [TEN Framework (Agora)](https://github.com/TEN-framework/ten_framework) | `sub-150ms` | Real-time multimodal conversational framework bridging hardware, wearables, and voice intelligence | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 1028ms` | [**GitHub / Docs ↗**](https://github.com/TEN-framework/ten_framework) |
| [Daily Bots](https://www.daily.co/products/bots/) | `sub-100ms` | Managed WebRTC infrastructure and cloud pipelines tailored for ultra-low latency voice agents | `Commercial / Free Tier` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 631ms` | [**GitHub / Docs ↗**](https://github.com/daily-co/daily-bots) |

## Voice Activity Detection (VAD) & Turn-Taking

| Framework / Model | Latency Target | Capability & Architecture | License | Health & Latency | Source & Docs |
| :--- | :---: | :--- | :---: | :--- | :--- |
| [Silero VAD v5](https://github.com/snakers4/silero-vad) | `sub-1ms` | Enterprise-grade pre-trained voice activity detector processing 30ms audio chunks in under 1ms | `MIT` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 671ms` | [**GitHub / Docs ↗**](https://github.com/snakers4/silero-vad) |
| [py-webrtcvad](https://github.com/wiseman/py-webrtcvad) | `sub-1ms` | Python interface to Google WebRTC's lightweight C-based Voice Activity Detector | `MIT` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 582ms` | [**GitHub / Docs ↗**](https://github.com/wiseman/py-webrtcvad) |
| [Voice-BPE & Audio Tokenizers](https://github.com/fishaudio/fish-speech) | `sub-10ms` | Acoustic vector quantization and discrete audio tokenizers for speech language models | `Apache-2.0` | ![Online](https://img.shields.io/badge/Status-Online-3fb950?style=flat-square) `⚡ 99ms` | [**GitHub / Docs ↗**](https://github.com/fishaudio/fish-speech) |

---

## 🏗️ Architectural Topology: Full-Duplex S2S Pipeline

```
+-------------------------------------------------------------------------+
|                     CLIENT / WEBRTC AUDIO STREAM                        |
+-------------------------------------------------------------------------+
             |                                          ^                  
   User Mic  | (16kHz PCM Audio Stream)                 | Agent Audio Play 
             v                                          |                  
+-------------------------+                +-------------------------+     
|  VAD & TURN DETECTION   |                |   LOW-LATENCY ACOUSTIC  |     
|  (Silero VAD v5 <1ms,   |                |          DECODER        |     
|   py-webrtcvad)         |                | (Kokoro-82M, Outetts,   |     
+-------------------------+                |  Moshi Mimi Audio Codec)|     
             | (Speech Frame)                           ^                  
             v                                          | (Acoustic Tokens)
+-------------------------------------------------------------------------+
|               FULL-DUPLEX SPEECH-TO-SPEECH (S2S) CORE                  |
|        (Kyutai Moshi 7B, Mini-Omni 2, GLM-4-Voice, Ultravox)           |
+-------------------------------------------------------------------------+
```

## 🤖 How the Autonomous Verification Engine Works
This repository is maintained automatically by a background verification daemon:
1. Every 24 hours, an automated runner sends latency probes and handshake pings to each framework's primary repository and documentation portal.
2. Frameworks with breaking deprecations, licensing shifts, or archived repositories are flagged and revised.
3. Live badges and latency benchmarks (`ms`) are re-computed and committed directly to `main` via GitHub Actions with concurrency locks.

## 🤝 Contributing & Submitting Voice Frameworks
Are you authoring or researching a new speech-to-speech model, ultra-fast neural TTS engine, or WebRTC voice framework? Pull requests are welcome! All submissions undergo automated validation.

---

### 🌐 Part of the @dhaulagani Developer Infrastructure & AI Suite
- ⚡ [awesome-free-developer-infra](https://github.com/dhaulagani/awesome-free-developer-infra) — Live-monitored free-tier cloud VPS, serverless DBs & developer tools.
- 🤖 [awesome-free-ai-apis](https://github.com/dhaulagani/awesome-free-ai-apis) — Free AI inference APIs, reasoning models (DeepSeek R1, Llama 3.3) & endpoints.
- 🧠 [awesome-sentient-ai](https://github.com/dhaulagani/awesome-sentient-ai) — Open-source cognitive architectures, episodic memory & world models.
- 📓 [awesome-free-cloud-notebooks](https://github.com/dhaulagani/awesome-free-cloud-notebooks) — Free cloud Jupyter notebooks, GPU servers & Colab/Kaggle alternatives.
- ⚡ [awesome-webgpu-ai](https://github.com/dhaulagani/awesome-webgpu-ai) — In-browser WebGPU runtimes, client-side LLMs & zero-server ML.
- 🎙️ [powerful-realtime-voice-ai](https://github.com/dhaulagani/powerful-realtime-voice-ai) — Full-duplex speech-to-speech (S2S) models, neural TTS & WebRTC agents.
- ⚡ [powerful-agent-skills](https://github.com/dhaulagani/powerful-agent-skills) — The fastest-trending AI agent skills, harnesses & self-installing registry.

**Maintained with ❤️ by [@dhaulagani](https://github.com/dhaulagani)** | Support open-source AI tooling via [GitHub Sponsors](https://github.com/sponsors/dhaulagani).