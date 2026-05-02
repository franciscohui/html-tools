---
description: Explore all available models on GroqCloud.
title: Supported Models - GroqDocs
image: https://console.groq.com/og_cloudv5.jpg
---

# Supported Models

Explore all available models on GroqCloud.

## [Featured Models and Systems](#featured-models-and-systems)

[![Groq Compound icon](https://console.groq.com/_next/image?url=%2Fgroq-circle.png&w=96&q=75)Groq CompoundGroq Compound is an AI system powered by openly available models that intelligently and selectively uses built-in tools to answer user queries, including web search and code execution.Token Speed\~450 tpsModalitiesCapabilities](/docs/compound/systems/compound)[![OpenAI GPT-OSS 120B icon](https://console.groq.com/_next/static/media/openailogo.523c87a0.svg)OpenAI GPT-OSS 120BGPT-OSS 120B is OpenAI's flagship open-weight language model with 120 billion parameters, built in browser search and code execution, and reasoning capabilities.Token Speed\~500 tpsModalitiesCapabilities](/docs/model/openai/gpt-oss-120b)

## [Production Models](#production-models)

**Note:** Production models are intended for use in your production environments. They meet or exceed our high standards for speed, quality, and reliability. Read more [here](https://console.groq.com/docs/deprecations).

| MODEL ID                                                                                                                                 | SPEED (T/SEC) | PRICE PER 1M TOKENS      | RATE LIMITS (DEVELOPER PLAN) | CONTEXT WINDOW (TOKENS) | MAX COMPLETION TOKENS | MAX FILE SIZE |
| ---------------------------------------------------------------------------------------------------------------------------------------- | ------------- | ------------------------ | ---------------------------- | ----------------------- | --------------------- | ------------- |
| [![Meta](https://console.groq.com/_next/image?url=%2FMeta_logo.png&w=48&q=75)Llama 3.1 8B](/docs/model/llama-3.1-8b-instant)llama-3.1-8b-instant                 | 560           | $0.05 input$0.08 output  | 250K TPM1K RPM               | 131,072                 | 131,072               | \-            |
| [![Meta](https://console.groq.com/_next/image?url=%2FMeta_logo.png&w=48&q=75)Llama 3.3 70B](/docs/model/llama-3.3-70b-versatile)llama-3.3-70b-versatile          | 280           | $0.59 input$0.79 output  | 300K TPM1K RPM               | 131,072                 | 32,768                | \-            |
| [![OpenAI](https://console.groq.com/_next/static/media/openailogo.523c87a0.svg)GPT OSS 120B](/docs/model/openai/gpt-oss-120b)openai/gpt-oss-120b                 | 500           | $0.15 input$0.60 output  | 250K TPM1K RPM               | 131,072                 | 65,536                | \-            |
| [![OpenAI](https://console.groq.com/_next/static/media/openailogo.523c87a0.svg)GPT OSS 20B](/docs/model/openai/gpt-oss-20b)openai/gpt-oss-20b                    | 1000          | $0.075 input$0.30 output | 250K TPM1K RPM               | 131,072                 | 65,536                | \-            |
| [![OpenAI](https://console.groq.com/_next/static/media/openailogo.523c87a0.svg)Whisper](/docs/model/whisper-large-v3)whisper-large-v3                            | \-            | $0.111 per hour          | 200K ASH300 RPM              | \-                      | \-                    | 100 MB        |
| [![OpenAI](https://console.groq.com/_next/static/media/openailogo.523c87a0.svg)Whisper Large V3 Turbo](/docs/model/whisper-large-v3-turbo)whisper-large-v3-turbo | \-            | $0.04 per hour           | 400K ASH400 RPM              | \-                      | \-                    | \-            |

## [Production Systems](#production-systems)

Systems are a collection of models and tools that work together to answer a user query.

  
| MODEL ID                                                                                                                      | SPEED (T/SEC) | PRICE PER 1M TOKENS | RATE LIMITS (DEVELOPER PLAN) | CONTEXT WINDOW (TOKENS) | MAX COMPLETION TOKENS | MAX FILE SIZE |
| ----------------------------------------------------------------------------------------------------------------------------- | ------------- | ------------------- | ---------------------------- | ----------------------- | --------------------- | ------------- |
| [![Groq](https://console.groq.com/_next/image?url=%2Fgroq-circle.png&w=48&q=75)Compound](/docs/compound/systems/compound)groq/compound                | 450           | \-                  | 200K TPM200 RPM              | 131,072                 | 8,192                 | \-            |
| [![Groq](https://console.groq.com/_next/image?url=%2Fgroq-circle.png&w=48&q=75)Compound Mini](/docs/compound/systems/compound-mini)groq/compound-mini | 450           | \-                  | 200K TPM200 RPM              | 131,072                 | 8,192                 | \-            |

  
[Learn More About Agentic ToolingDiscover how to build powerful applications with real-time web search and code execution](https://console.groq.com/docs/agentic-tooling) 

## [Preview Models](#preview-models)

**Note:** Preview models are intended for evaluation purposes only and should not be used in production environments as they may be discontinued at short notice. Read more about deprecations [here](https://console.groq.com/docs/deprecations).

| MODEL ID                                                                                                                                                                    | SPEED (T/SEC) | PRICE PER 1M TOKENS      | RATE LIMITS (DEVELOPER PLAN) | CONTEXT WINDOW (TOKENS) | MAX COMPLETION TOKENS | MAX FILE SIZE |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- | ------------------------ | ---------------------------- | ----------------------- | --------------------- | ------------- |
| [![Canopy Labs](https://console.groq.com/_next/image?url=%2Fcanopylabs.png&w=48&q=75)Canopy Labs Orpheus Arabic Saudi](/docs/model/canopylabs/orpheus-arabic-saudi)canopylabs/orpheus-arabic-saudi  | \-            | $40.00 per 1M characters | 50K TPM250 RPM               | 4,000                   | 50,000                | \-            |
| [![Canopy Labs](https://console.groq.com/_next/image?url=%2Fcanopylabs.png&w=48&q=75)Canopy Labs Orpheus V1 English](/docs/model/canopylabs/orpheus-v1-english)canopylabs/orpheus-v1-english        | \-            | $22.00 per 1M characters | 50K TPM250 RPM               | 4,000                   | 50,000                | \-            |
| [![Meta](https://console.groq.com/_next/image?url=%2FMeta_logo.png&w=48&q=75)Llama 4 Scout 17B 16E](/docs/model/meta-llama/llama-4-scout-17b-16e-instruct)meta-llama/llama-4-scout-17b-16e-instruct | 750           | $0.11 input$0.34 output  | 300K TPM1K RPM               | 131,072                 | 8,192                 | 20 MB         |
| [![Meta](https://console.groq.com/_next/image?url=%2FMeta_logo.png&w=48&q=75)Llama Prompt Guard 2 22M](/docs/model/meta-llama/llama-prompt-guard-2-22m)meta-llama/llama-prompt-guard-2-22m          | \-            | $0.03 input$0.03 output  | 30K TPM100 RPM               | 512                     | 512                   | \-            |
| [![Meta](https://console.groq.com/_next/image?url=%2FMeta_logo.png&w=48&q=75)Prompt Guard 2 86M](/docs/model/meta-llama/llama-prompt-guard-2-86m)meta-llama/llama-prompt-guard-2-86m                | \-            | $0.04 input$0.04 output  | 30K TPM100 RPM               | 512                     | 512                   | \-            |
| [![OpenAI](https://console.groq.com/_next/static/media/openailogo.523c87a0.svg)Safety GPT OSS 20B](/docs/model/openai/gpt-oss-safeguard-20b)openai/gpt-oss-safeguard-20b                            | 1000          | $0.075 input$0.30 output | 150K TPM1K RPM               | 131,072                 | 65,536                | \-            |
| [![Alibaba Cloud](https://console.groq.com/_next/image?url=%2Fqwen_logo.png&w=48&q=75)Qwen3-32B](/docs/model/qwen/qwen3-32b)qwen/qwen3-32b                                                          | 400           | $0.29 input$0.59 output  | 300K TPM1K RPM               | 131,072                 | 40,960                | \-            |

## [Deprecated Models](#deprecated-models)

Deprecated models are models that are no longer supported or will no longer be supported in the future. See our deprecation guidelines and deprecated models [here](https://console.groq.com/docs/deprecations).

## [Get All Available Models](#get-all-available-models)

Hosted models are directly accessible through the GroqCloud Models API endpoint using the model IDs mentioned above. You can use the `https://api.groq.com/openai/v1/models` endpoint to return a JSON list of all active models:

Python

```
curl -X GET "https://api.groq.com/openai/v1/models" \
     -H "Authorization: Bearer $GROQ_API_KEY" \
     -H "Content-Type: application/json"
```

```
import Groq from "groq-sdk";

const groq = new Groq({ apiKey: process.env.GROQ_API_KEY });

const getModels = async () => {
  return await groq.models.list();
};

getModels().then((models) => {
  // console.log(models);
});
```

```
import requests
import os

api_key = os.environ.get("GROQ_API_KEY")
url = "https://api.groq.com/openai/v1/models"

headers = {
    "Authorization": f"Bearer {api_key}",
    "Content-Type": "application/json"
}

response = requests.get(url, headers=headers)

print(response.json())
```

---
description: Use Groq&#x27;s server-side tools for instant web search, code execution, and browser automation without any setup.
title: Groq Built-In Tools - GroqDocs
image: https://console.groq.com/og_cloudv5.jpg
---

# Groq Built-In Tools

Built-in (or server-side) tools are the easiest way to add agentic capabilities to your application. Unlike [remote MCP](https://console.groq.com/docs/tool-use/remote-mcp) where you connect to external servers, or [local tool calling](https://console.groq.com/docs/tool-use/local-tool-calling) where you implement functions yourself, built-in tools require **zero orchestration**.

Just call the API, specify which tools you want to allow the model to use, and Groq's systems will handle the rest - tool execution, orchestration, and returning the final answer.

Built-in tools are not HIPAA Covered Cloud Services under Groq's Business Associate Addendum at this time. These tools are also not available currently for use with regional / sovereign endpoints.

## [How Built-In Tools Work](#how-builtin-tools-work)

With built-in tools, **execution happens entirely on Groq's servers**. The model autonomously calls built-in tools (web search, code execution) and handles the entire agentic loop internally. You get one response with everything completed.

Your App → Makes request to Groq API with allowed_tools parameter
   ↓
Groq API → Makes request to LLM with built-in tool definitions from 
           the allowed_tools parameter
         ← Model returns tool_calls with built-in tool names (or, if no 
           tool calls are needed, returns final response)
   ↓
Groq API → Parses tool call arguments server-side
         → Makes request to built-in tool with tool call arguments
         ← Built-in tool returns results
   ↓
Groq API → Makes another request to LLM with tool results
         ← Model returns more tool_calls (returns to step 3), or 
           returns final response
   ↓
Your App

## [Which Models Support Built-In Tools](#which-models-support-builtin-tools)

### [1\. Groq Compound Systems](#1-groq-compound-systems)

Groq's **Compound** systems are purpose-built for agentic workflows with a full suite of built-in tools:

**Models:**

* `groq/compound` \- Supports multiple tools per request
* `groq/compound-mini` \- Single tool per request, 3x lower latency

**Available Tools:**

| Tool                                           | Identifier          |
| ---------------------------------------------- | ------------------- |
| [Web Search](https://console.groq.com/docs/web-search)                 | web\_search         |
| [Code Execution](https://console.groq.com/docs/code-execution)         | code\_interpreter   |
| [Visit Website](https://console.groq.com/docs/visit-website)           | visit\_website      |
| [Browser Automation](https://console.groq.com/docs/browser-automation) | browser\_automation |
| [Wolfram Alpha](https://console.groq.com/docs/wolfram-alpha)           | wolfram\_alpha      |

**How to use Compound systems:**

Python

```
from groq import Groq

client = Groq()

completion = client.chat.completions.create(
    messages=[
        {
            "role": "user",
            "content": "What is the current weather in Tokyo?",
        }
    ],
    # Change model to compound to use built-in tools
    model="groq/compound",
)

print(completion.choices[0].message.content)
# Print all tool calls
# print(completion.choices[0].message.executed_tools)
```

```
import Groq from "groq-sdk";

const groq = new Groq();

export async function main() {
  const completion = await groq.chat.completions.create({
    messages: [
      {
        role: "user",
        content: "What is the current weather in Tokyo?",
      },
    ],
    // Change model to compound to use built-in tools
    model: "groq/compound",
  });

  console.log(completion.choices[0]?.message?.content || "");
  // Print all tool calls
  // console.log(completion.choices[0]?.message?.executed_tools || "");
}

main();
```

```
curl https://api.groq.com/openai/v1/chat/completions -s \
    -H "Content-Type: application/json" \
    -H "Authorization: Bearer $GROQ_API_KEY" \
    -d '{
    "model": "groq/compound",
    "messages": [{
        "role": "user",
        "content": "What is the current weather in Tokyo?"
    }]
}'
```

The system automatically determines which tools to use based on the query and executes them server-side. You can optionally restrict which tools are available using the `compound_custom.tools.enabled_tools` parameter (see [Configuring Tools](#configuring-tools)).

**Example Response:**

JSON

```
{
  "id": "stub",
  "object": "chat.completion",
  "created": 1761750004,
  "model": "groq/compound",
  "choices": [{
    "index": 0,
    "message": {
      "role": "assistant",
      "content": "**Current weather in Tokyo (as of the latest report on Oct 29 2025, 11:00 pm JST)**\\n\\n| Parameter | Value |\\n|-----------|-------|\\n| **Temperature** | 53 °F ≈ 12 °C |...",
      "executed_tools": [{
        "index": 0,
        "type": "search",
        "arguments": "{\"query\": \"current weather in Tokyo\"}",
        "output": "Title: Weather for Tokyo, Japan...\\n..."
      }]
    },
    "finish_reason": "stop"
  }],
  "usage": {
    "prompt_tokens": 116,
    "completion_tokens": 571,
    "total_tokens": 7340
  }
}
```

The `executed_tools` array shows which tools were called during the request, including the arguments passed and the results returned.

### [Configuring Tools](#configuring-tools)

Use the `compound_custom.tools.enabled_tools` parameter to restrict which tools are available. Pass an array of tool identifiers: `web_search`, `code_interpreter`, `visit_website`, `browser_automation`, `wolfram_alpha`.

Python

```
from groq import Groq

client = Groq(
    default_headers={
        "Groq-Model-Version": "latest"
    }
)

response = client.chat.completions.create(
    model="groq/compound",
    messages=[
        {
            "role": "user",
            "content": "Search for recent AI developments and then visit the Groq website"
        }
    ],
    compound_custom={
        "tools": {
            "enabled_tools": ["web_search", "visit_website"]
        }
    }
)
```

```
import Groq from "groq-sdk";

const groq = new Groq({
  defaultHeaders: {
    "Groq-Model-Version": "latest"
  }
});

const response = await groq.chat.completions.create({
  model: "groq/compound",
  messages: [
    {
      role: "user",
      content: "Search for recent AI developments and then visit the Groq website"
    }
  ],
  compound_custom: {
    tools: {
      enabled_tools: ["web_search", "visit_website"]
    }
  }
});
```

```
curl "https://api.groq.com/openai/v1/chat/completions" \
  -X POST \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer ${GROQ_API_KEY}" \
  -H "Groq-Model-Version: latest" \
  -d '{
        "messages": [
          {
            "role": "user",
            "content": "Search for recent AI developments and then visit the Groq website"
          }
        ],
        "model": "groq/compound",
        "compound_custom": {
          "tools": {
            "enabled_tools": ["web_search", "visit_website"]
          }
        }
      }'
```

### [Compatibility with Local Tool Calling and Remote MCP Tools](#compatibility-with-local-tool-calling-and-remote-mcp-tools)

Groq's Compound systems only support built-in tools and cannot be used with local tool calling or remote MCP tools.

For more details, see the [Compound Built-In Tools documentation](https://console.groq.com/docs/compound/built-in-tools).

[Compound Built-In ToolsFull details on tool configuration, versioning, and advanced features](https://console.groq.com/docs/compound/built-in-tools) 

### [2\. GPT-OSS Models](#2-gptoss-models)

OpenAI's open-weight models support a subset of built-in tools:

**Models:**

* `openai/gpt-oss-120b`
* `openai/gpt-oss-20b`

**Available Tools:**

| Tool                                   | Identifier        |
| -------------------------------------- | ----------------- |
| [Browser Search](https://console.groq.com/docs/browser-search) | browser\_search   |
| [Code Execution](https://console.groq.com/docs/code-execution) | code\_interpreter |

**Limitations:**

* Cannot use Visit Website, Browser Automation, or Wolfram Alpha

**How to use GPT-OSS models:**

Python

```
from groq import Groq

client = Groq()

# Automatically uses tools when needed
response = client.chat.completions.create(
    model="openai/gpt-oss-120b",
    messages=[{
        "role": "user",
        "content": "What's the current population of Tokyo?"
    }]
)

# Or specify which tool to enable
response = client.chat.completions.create(
    model="openai/gpt-oss-120b",
    messages=[{
        "role": "user",
        "content": "Search for recent AI developments"
    }],
    tools=[{"type": "browser_search"}]
)

print(response.choices[0].message.content)
```

```
import Groq from "groq-sdk";

const client = new Groq();

// Automatically uses tools when needed
const response = await client.chat.completions.create({
  model: "openai/gpt-oss-120b",
  messages: [{
    role: "user",
    content: "What's the current population of Tokyo?"
  }]
});

// Or specify which tool to enable
const responseWithTool = await client.chat.completions.create({
  model: "openai/gpt-oss-120b",
  messages: [{
    role: "user",
    content: "Search for recent AI developments"
  }],
  tools: [{ type: "browser_search" }]
});

console.log(response.choices[0].message.content);
```

GPT-OSS models are ideal when you need a large context window (131K tokens) with basic tool capabilities.

### [Configuring Tools](#configuring-tools)

Use the `tools` parameter with tool type objects. You can specify `browser_search` or `code_interpreter`.

Python

```
# Single tool
tools=[{"type": "browser_search"}]

# Or multiple tools
tools=[{"type": "browser_search"}, {"type": "code_interpreter"}]
```

```
// Single tool
const tools = [{ type: "browser_search" }];

// Or multiple tools
const tools = [{ type: "browser_search" }, { type: "code_interpreter" }];
```

### [Compatibility with Local Tool Calling and Remote MCP Tools](#compatibility-with-local-tool-calling-and-remote-mcp-tools)

GPT-OSS models can be used alongside local tool calling or remote MCP tools in the same request.

## [Viewing Tool Execution](#viewing-tool-execution)

To see which tools were used in a request, check the `executed_tools` field in the response:

Python

```
import os
from groq import Groq

client = Groq(api_key=os.environ.get("GROQ_API_KEY"))

response = client.chat.completions.create(
    model="groq/compound",
    messages=[
        {"role": "user", "content": "What did Groq release last week?"}
    ]
)
# Log the tools that were used to generate the response
print(response.choices[0].message.executed_tools)
```

```
import Groq from 'groq-sdk';

const groq = new Groq();

async function main() {
  const response = await groq.chat.completions.create({
    model: 'groq/compound',
    messages: [
      {
        role: 'user',
        content: 'What did Groq release last week?'
      }
    ]
  })
  // Log the tools that were used to generate the response
  console.log(response.choices[0].message.executed_tools)
}
main();
```

```
curl https://api.groq.com/openai/v1/chat/completions -s \
    -H "Content-Type: application/json" \
    -H "Authorization: Bearer $GROQ_API_KEY" \
    -d '{
    "model": "groq/compound",
    "messages": [{
        "role": "user",
        "content": "What did Groq release last week?"
    }]
}'
```

## [Next Steps](#next-steps)

[Remote Tools and MCPConnect to MCP servers for standardized tool integrations](https://console.groq.com/docs/tool-use/remote-mcp)[Local Tool CallingDefine and execute custom tools in your application code](https://console.groq.com/docs/tool-use/local-tool-calling)[Web Search ToolDeep dive into the web search tool capabilities](https://console.groq.com/docs/web-search)[Code Execution ToolLearn about running Python code securely](https://console.groq.com/docs/code-execution)[Compound SystemsFull documentation on Compound systems](https://console.groq.com/docs/compound)