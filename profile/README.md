


Autocua org profile readme · MD
<div align="center">
# AutoCua
 
### Automatic computer use for every screen you own
 
Mac · Windows · Linux · real iPhone · iOS Simulator · any browser
<br>
A multi-agent harness engine, driven by real input.
 
```
pip install AutoCua
```
 
[**Get the code**](https://github.com/AutoCua/AutoCua) · [**Full capabilities**](https://github.com/AutoCua/AutoCua/blob/main/agent_capabilities.md) · [**Report an issue**](https://github.com/AutoCua/AutoCua/issues)
 
</div>
---
 
## One string picks the surface
 
```python
from AutoCua.agent_launcher import run_agent
 
run_agent(
    mode="web use",
    provider="openrouter",
    model="gemini-3.8-flash",
    task="Open wikipedia.org and summarise today's featured article.",
)
```
 
| Mode | What it drives | Where it runs |
| --- | --- | --- |
| `computer use` | Any desktop app, with real mouse and keyboard input | macOS, Windows or Linux |
| `shell use` | A coding agent, straight into a real terminal | macOS, Windows or Linux |
| `web use` | Your own Chrome, through the AutoCua extension | Any host with Chrome |
| `mobile use, ios` | An iOS Simulator, or your paired iPhone or iPad | macOS host |
 
Windows 10 and 11 · Linux with GNOME · macOS on Apple Silicon or Intel
 
## Why it holds up on real software
 
- **No pixel guessing.** The model never sees a coordinate. It picks a numbered element from a view that fuses the operating system's accessibility tree with OCR, and a number it was never shown is rejected before anything moves.
- **No debugging port on your desktop.** Input goes in at the operating system's own input layer, so an ordinary app sees the same events it would get from your hand on the mouse.
- **No debugging port on your browser either.** A normal web run drives your own Chrome, logged in as you, through the AutoCua extension.
- **No context wall.** A separate compression agent splices a handoff summary into the transcript mid-run, so a long task finishes instead of dying at the context limit.
- **No telemetry.** AutoCua sends nothing anywhere except to the model provider you chose, and to Telegram if you connect it yourself.
## What is inside
 
- **An agent team.** A parent agent owns the screen. A coder agent handles real code work, and read-only minions scout the codebase in parallel.
- **A browser agent written in Rust.** Hand-written CDP, with no Playwright, Selenium or Puppeteer.
- **iPhone and iPad.** The same loop that drives your Mac drives a phone, over USB or in the Simulator.
- **Parallel runs.** Pass `extra_tasks` and every task runs at once, each in its own tab or simulator.
- **A desktop app.** Add `ui=True` for live screenshots, a live plan, resumable chats and skills.
- **Remote control from Telegram.** Send tasks from your phone and watch milestones stream back.
- **Nine providers.** Anthropic, AWS Bedrock, Cerebras, Google, Groq, OpenAI, OpenRouter, Perplexity and Together AI.
## Good to know
 
AutoCua is a language model driving real software, so two runs of the same task can take different routes. It is a strong fit for exploratory testing, smoke flows and repetitive back-office work. It is not a replacement for a deterministic test suite.
 
---
 
<div align="center">
Released under the MIT licence · Star the repo if it is useful to you
 
</div>
 
Claude finished the response
