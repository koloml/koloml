# LLM Usage

I have mixed feelings about LLMs and usage of agents. I will try to write about it here for anyone wondering.

## Purposes

### For writing

I completely avoid using LLMs for writing texts. I don't like how LLM-ish English sounds like. I don't like usage of
buzz words all over the place. I don't like patterns LLM constantly repeat in writing. Because of that I only write
something I actually want to write by myself.

Yes, I'm not that good at writing. English is my second language, so I often make mistakes I can't even detect myself.
But that's still way better than whatever goes out of the LLM output.

I do enjoy using "em-dashes" — I started using them way-way before LLMs became popular. Perhaps I use them incorrectly,
but I still like them. I also like following proper capitalization, use commas and periods, even when I'm just chatting
with someone.

### For coding

I use coding agents on my current workplace. They're offering subscription to Claude Code funded by the client. 

I don't trust them for 100%, so I never let the agent go loose and code without my review. From my personal experience, 
I've seen many cases where agent will start something it shouldn't do. Like not following code style. Or duplicating 
code which already exist in the codebase. Or inflating the code with huge code comments, which contain agent's rambling 
about some bugs they found and fixed.

I avoid using coding agents in my personal projects. These projects are usually done for the fun of it. Or to learn 
something new, to familiarize myself with some libraries or frameworks. The only uses I might accept for my own projects
is to write occasional unit tests, search something, review code or brainstorm something I might be stuck on.

### General use (questions/searching)

I do occasionally use LLMs to query the internet with more complex questions. I can even use local LLMs for this 
purpose, since you don't really need huge model for this kind of stuff.

But I don't really trust the LLM to tell me the "truth" for everything I would ask it about. Had enough cases where LLM
will just make up details on the spot. Or where LLM will trust anything search results will show to them.

### For chatting

No.

## Cloud LLMs vs Local LLMs

I don't like the fact all currently capable LLMs are available only by subscription on some random server I don't have
control over. It feels like nobody is worried about that.

I've tried using different local LLMs on my own machine — mainly GPT-OSS, and Qwen models. They're practically useless
for complex coding tasks (at the parameters count I could offer), but they're fine enough for general use.

## What I've tried

### Agents

- Claude Code — main thing I'm using on my workplace. Anthropic LLMs doing their job just fine, usually completes whatever I ask for without major problems. TUI is uncomfortable.
- OpenCode — used only with local models, working just fine. Local models are not as good at coding, so I only really used it for exploration or occasional review.

#### Software with ACP support

- JetBrains Air — quite comfy, but Claude Code doesn't like being used in other apps outside their own TUI.
- AI Chat in PhpStorm — fine for some general questions or exploration/explaining, but at the time of me testing it, ACP was a bit uncomfortable to use.

### Models

- Anthropic
  - **Haiku** — never using it, only invoked by the Claude Code when some light research from the codebase needs to be done. 
  - **Sonnet** — main model I'm relying on. Doing stuff just fine, as long as I request something specific and properly explain what I want from the agent.
  - **Opus** — sometimes use this model to plan something for the **Sonnet** model and to reduce potential for the model to do something completely wrong.
  - **Fable** — avoiding it, too expensive to use.
- Local LLMs
  - **Qwen 3.6 35B** — general use is good, coding is fine, but prone to hallucinations, so practically unusable. Quite slow for super interactive usage.
  - **GPT OSS 20B** — pretty fast, general use is fine, coding is completely unusable. Makes a bit too much tables. Overly restrictive in some topics.
