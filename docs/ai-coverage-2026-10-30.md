# AI domain coverage audit — 2026-10-30

This update adds selected AI service, API, authentication and dedicated resource domains, including services absent from the traffic export. The source documents identify service ownership or required endpoints; choosing the AI policy is a local routing decision, not a vendor requirement.

Shared cloud/CDN domains use exact hosts. No wholesale additions for googleapis.com, githubusercontent.com, amazonaws.com, cloudfront.net, workos.com or generic telemetry platforms. Domestic AI direct rules and the main configuration order are retained.

## Added AI rules and official evidence

| Service | Rule | Official source |
|---|---|---|
| Midjourney AI 服务 | `DOMAIN-SUFFIX,midjourney.com` | [Source](https://www.midjourney.com/) |
| AI Agent 搜索服务 | `DOMAIN-SUFFIX,tavily.com` | [Source](https://www.tavily.com/) |
| Manus AI 服务 | `DOMAIN-SUFFIX,manus.im` | [Source](https://manus.im/) |
| OpenAI / ChatGPT | `DOMAIN-SUFFIX,oaistatsig.com` | [Source](https://help.openai.com/en/articles/9247338-network-recommendations-for-chatgpt-errors-on-web-and-apps) |
| OpenAI / ChatGPT | `DOMAIN,cdn.workos.com` | [Source](https://help.openai.com/en/articles/9247338-network-recommendations-for-chatgpt-errors-on-web-and-apps) |
| OpenAI / ChatGPT | `DOMAIN,forwarder.workos.com` | [Source](https://help.openai.com/en/articles/9247338-network-recommendations-for-chatgpt-errors-on-web-and-apps) |
| OpenAI / ChatGPT | `DOMAIN,frontend-apps-multi-region.workos.com` | [Source](https://help.openai.com/en/articles/9247338-network-recommendations-for-chatgpt-errors-on-web-and-apps) |
| OpenAI / ChatGPT | `DOMAIN,setup.workos.com` | [Source](https://help.openai.com/en/articles/9247338-network-recommendations-for-chatgpt-errors-on-web-and-apps) |
| OpenAI / ChatGPT | `DOMAIN,images.workoscdn.com` | [Source](https://help.openai.com/en/articles/9247338-network-recommendations-for-chatgpt-errors-on-web-and-apps) |
| OpenAI / ChatGPT | `DOMAIN,workos.imgix.net` | [Source](https://help.openai.com/en/articles/9247338-network-recommendations-for-chatgpt-errors-on-web-and-apps) |
| ChatGPT 别名 | `DOMAIN-SUFFIX,chat.com` | [Source](https://chat.com/) |
| Cursor API、资源和云端运行 | `DOMAIN-SUFFIX,cursorapi.com` | [Source](https://prod.cursor.com/docs/enterprise/network-configuration) |
| Cursor API、资源和云端运行 | `DOMAIN-SUFFIX,cursor-cdn.com` | [Source](https://prod.cursor.com/docs/enterprise/network-configuration) |
| Cursor API、资源和云端运行 | `DOMAIN-SUFFIX,cursorvm.com` | [Source](https://prod.cursor.com/docs/enterprise/network-configuration) |
| Cursor / Grok 认证和资源 | `DOMAIN-SUFFIX,grokusercontent.com` | [Source](https://cursor.com/help/troubleshooting/sign-in-domains) |
| Cursor / Grok 认证和资源 | `DOMAIN-SUFFIX,grokipedia.com` | [Source](https://cursor.com/help/troubleshooting/sign-in-domains) |
| Cursor / Grok 认证和资源 | `DOMAIN,accounts.spacex.ai` | [Source](https://cursor.com/help/troubleshooting/sign-in-domains) |
| Windsurf / Codeium / Devin | `DOMAIN-SUFFIX,windsurf.com` | [Source](https://docs.devin.ai/desktop/troubleshooting/windsurf-common-issues) |
| Windsurf / Codeium / Devin | `DOMAIN-SUFFIX,codeium.com` | [Source](https://docs.devin.ai/desktop/troubleshooting/windsurf-common-issues) |
| Windsurf / Codeium / Devin | `DOMAIN-SUFFIX,codeiumdata.com` | [Source](https://docs.devin.ai/desktop/troubleshooting/windsurf-common-issues) |
| Windsurf / Codeium / Devin | `DOMAIN-SUFFIX,devin.ai` | [Source](https://docs.devin.ai/desktop/troubleshooting/windsurf-common-issues) |
| Windsurf / Codeium / Devin | `DOMAIN-SUFFIX,devinenterprise.com` | [Source](https://docs.devin.ai/desktop/troubleshooting/windsurf-common-issues) |
| Google Gemini Code Assist 专用接口 | `DOMAIN,cloudaicompanion.googleapis.com` | [Source](https://docs.cloud.google.com/gemini/docs/codeassist/set-up-gemini) |
| Google Gemini Code Assist 专用接口 | `DOMAIN,cloudcode-pa.googleapis.com` | [Source](https://docs.cloud.google.com/gemini/docs/codeassist/set-up-gemini) |
| Google Antigravity | `DOMAIN-SUFFIX,antigravity.google` | [Source](https://docs.cloud.google.com/docs/security/compliance/deploy-antigravity-us-public-sector) |
| Google Antigravity | `DOMAIN-SUFFIX,antigravity.google.com` | [Source](https://docs.cloud.google.com/docs/security/compliance/deploy-antigravity-us-public-sector) |
| Google Antigravity | `DOMAIN-SUFFIX,antigravity-unleash.goog` | [Source](https://docs.cloud.google.com/docs/security/compliance/deploy-antigravity-us-public-sector) |
| Google Antigravity | `DOMAIN,daily-cloudcode-pa.googleapis.com` | [Source](https://docs.cloud.google.com/docs/security/compliance/deploy-antigravity-us-public-sector) |
| Google Antigravity | `DOMAIN,aicode.googleapis.com` | [Source](https://docs.cloud.google.com/docs/security/compliance/deploy-antigravity-us-public-sector) |
| Google Jules | `DOMAIN-SUFFIX,jules.google` | [Source](https://jules.google/) |
| Google Jules | `DOMAIN-SUFFIX,jules.google.com` | [Source](https://jules.google/) |
| Gemini 别名 | `DOMAIN-SUFFIX,gemini.google` | [Source](https://gemini.google/) |
| NotebookLM / Gemini Notebook 别名 | `DOMAIN-SUFFIX,notebooklm.google` | [Source](https://notebooklm.google/) |
| NotebookLM / Gemini Notebook 别名 | `DOMAIN-SUFFIX,notebook.google` | [Source](https://notebooklm.google/) |
| Perplexity 别名 | `DOMAIN-SUFFIX,pplx.ai` | [Source](https://pplx.ai/) |
| Perplexity 别名 | `DOMAIN-SUFFIX,perplexity.com` | [Source](https://perplexity.com/) |
| Hugging Face 别名 | `DOMAIN-SUFFIX,hf.co` | [Source](https://hf.co/) |
| Hugging Face Spaces | `DOMAIN-SUFFIX,hf.space` | [Source](https://huggingface.co/docs/hub/spaces-embed) |
| Manus 专用文件资源（官网 HTML 使用 files.manuscdn.com） | `DOMAIN-SUFFIX,manuscdn.com` | [Source](https://manus.im/) |
| ElevenLabs 语音和 API | `DOMAIN-SUFFIX,elevenlabs.io` | [Source](https://elevenlabs.io/docs/api-reference/authentication) |
| ElevenLabs 别名 | `DOMAIN-SUFFIX,elevenlabs.com` | [Source](https://elevenlabs.com/) |
| Cerebras 推理服务 | `DOMAIN-SUFFIX,cerebras.ai` | [Source](https://www.cerebras.ai/) |
| LM Studio | `DOMAIN-SUFFIX,lmstudio.ai` | [Source](https://lmstudio.ai/) |
| DeepWiki | `DOMAIN-SUFFIX,deepwiki.com` | [Source](https://deepwiki.com/) |
| Lovable | `DOMAIN-SUFFIX,lovable.dev` | [Source](https://docs.lovable.dev/introduction/welcome) |
| v0 | `DOMAIN-SUFFIX,v0.app` | [Source](https://v0.app/docs) |
| v0 旧域名 | `DOMAIN-SUFFIX,v0.dev` | [Source](https://v0.dev/) |
| Bolt | `DOMAIN-SUFFIX,bolt.new` | [Source](https://bolt.new/) |
| Runway 网站及 API | `DOMAIN-SUFFIX,runwayml.com` | [Source](https://runwayml.com/) |
| Runway 网站及 API | `DOMAIN-SUFFIX,runway.com` | [Source](https://runwayml.com/) |
| Suno 音乐及专用资源 | `DOMAIN-SUFFIX,suno.com` | [Source](https://suno.com/) |
| Suno 音乐及专用资源 | `DOMAIN-SUFFIX,suno.ai` | [Source](https://suno.com/) |
| Udio | `DOMAIN-SUFFIX,udio.com` | [Source](https://www.udio.com/) |
| Ideogram | `DOMAIN-SUFFIX,ideogram.ai` | [Source](https://ideogram.ai/) |
| Krea | `DOMAIN-SUFFIX,krea.ai` | [Source](https://www.krea.ai/) |
| fal 生成媒体平台 | `DOMAIN-SUFFIX,fal.ai` | [Source](https://fal.ai/) |
| fal 推理和结果资源 | `DOMAIN-SUFFIX,fal.run` | [Source](https://fal.ai/docs/documentation/model-apis/inference/queue) |
| fal 推理和结果资源 | `DOMAIN-SUFFIX,fal.media` | [Source](https://fal.ai/docs/documentation/model-apis/inference/queue) |
| Stability AI 及其官网链接的 Stable Audio | `DOMAIN-SUFFIX,stability.ai` | [Source](https://stability.ai/) |
| Stability AI 及其官网链接的 Stable Audio | `DOMAIN-SUFFIX,stableaudio.com` | [Source](https://stability.ai/) |

## Precedence and cleanup

- The existing `DOMAIN,search.lmstudio.ai` is replaced by `DOMAIN-SUFFIX,lmstudio.ai`; the search host stays in the same AI group.
- The old AI rule for `static.cloudflareinsights.com` is removed because the approved `app-clean.list` suffix rule now owns this family and is loaded first.
- Broad legacy Sentry, Crashlytics, ASN and other shared dependency classifications are not expanded or restructured in this update.
- Microsoft remains before AI in the consumer configurations. Existing Copilot overlaps are not resolved by adding redundant late rules.
- The game list selects the game policy group; its actual DIRECT/proxy choice is made by the client.

## Reviewed sources and excluded candidates

The current V2Fly and MetaCubeX AI categories were used to discover candidates; selected additions were then checked against official documentation, official sites, redirects, or resources embedded by the official site. They were not imported wholesale.

- [V2Fly category](https://github.com/v2fly/domain-list-community/blob/master/data/category-ai-!cn)
- [MetaCubeX category](https://github.com/MetaCubeX/meta-rules-dat/blob/meta/geo/geosite/category-ai-!cn.list)

Community-only entries such as `windsurf.build` and unverified Claude alias domains were not added. Google API names without direct official endpoint evidence were left out. Foreign-facing variants of domestic AI services (for example Kimi/Moonshot/MiniMax/Trae) were not swept into AI without a separate regional routing review. Existing explicit domestic AI direct rules remain unchanged.

## Validation scope

Validate new exact and suffix rules against first-match DOMAIN / DOMAIN-SUFFIX / DOMAIN-KEYWORD order in both local consumer configurations, compare the full observed Host set to the pre-change snapshot, and check remote raw lists after push. This is static routing validation, not a real-device connectivity, speed, login, download or WebSocket test.
