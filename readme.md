
## AI home
https://github.com/judahpaul16/gpt-home/tree/main

## Setup sound 

```
jharvey@raspberrypi:~/gpt-home $ cat /etc/asound.conf
pcm.!default { type hw card vc4hdmi0 device 0 }
ctl.!default { type hw card vc4hdmi0 }
```

## Clade
  - Need API key from CLAUDE.
  - **DONT PASTE IN WEB API - ADD TO  .env**

```
# LiteLLM API Key (required for LLM and embeddings)
# Supports: OpenAI, Anthropic, Google, Cohere, Azure, and 100+ more
# Can be edited via web UI Settings page
LITELLM_API_KEY='sk-ant-api03-bD2Ch0rrrKvrRLPr-XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'

# Model to use - LiteLLM format
# Examples: gpt-4o-mini, gpt-4, claude-3-5-sonnet-20241022, gemini/gemini-pro
MODEL='anthropic/claude-sonnet-4-5-20250929'
```

## start
```
cd gpt-home
COMPOSE_PROFILES=dev docker-compose up
```

## connect
http://raspberrypi
