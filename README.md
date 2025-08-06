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
I recorded several conversations between Open Hands AI and llama.cpp running GLM-4.5 Q4_K_M
using a tool called `mitmdump`.


# prompt

The prompt was:

````
You've been given access to the `llama.cpp` and `ik_llama.cpp` projects. There is a GLM-4.5 feature branch loaded in each project. You can view the diffs with:

`cd /workspace/llama.cpp && git diff master...glm-4-5`

and

`cd /workspace/ik_llama.cpp && git diff main...glm-4.5-clean`

What do you think of these changes?
````
