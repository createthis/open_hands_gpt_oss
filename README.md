# How

This was recorded with:

```bash
mitmdump --mode reverse:http://larry:11434 -p 8080 -w full_traffic.mitm
```

To install `mitmdump` so you can view this transcript: https://docs.mitmproxy.org/stable/overview/installation/

To view the entire conversation as plain text:

```bash
mitmdump -nr full_traffic.mitm --flow-detail 4
```

# What
I recorded several conversations between Open Hands AI and llama.cpp running GPT OSS 120b
using a tool called `mitmdump`. First convo was on linux/mac host. Second was on Windows without WSL.

## harmony patch
The conversation after the [llama.cpp harmony patch](https://github.com/ggml-org/llama.cpp/pull/15181) is this one:


```bash
mitmdump -nr full_traffic_harmony_parser_aug_11_2025.mitm --flow-detail 4
```
