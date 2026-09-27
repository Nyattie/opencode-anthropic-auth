---
"@ex-machina/opencode-anthropic-auth": patch
---

Decode tool-name aliases when OpenCode reloads the plugin while a request is in flight. Previously the response reached a newer plugin setup that did not recognize the request, so the raw `mcp_T...` alias reached OpenCode and the tool call failed with "No tool named".
