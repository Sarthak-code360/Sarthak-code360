<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:B11313,100:0D1B4C&height=200&section=header&text=Sarthak%20Mishra&fontSize=50&fontColor=F5F7FA&fontAlignY=38&animation=fadeIn&desc=friendly%20neighbourhood%20robot%20whisperer&descAlignY=58&descSize=18&descColor=F5F7FA" width="100%"/>

<a href="https://sarthaksportfolio.netlify.app/"><img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=500&size=18&duration=2600&pause=700&color=E23636&center=true&vCenter=true&width=760&lines=%24+robofleet+factory+serve+--brain+qwen3.8-27b;%3E+robots+see+%E2%86%92+server+thinks+%E2%86%92+robots+move;%3E+250-300+cmds%2Fsec+%40+220ms+on+live+vehicle+fleets;%3E+pip+install+robofleet;%3E+spidey-sense%3A+tingling+(it%27s+always+DNS)" alt="typing"/></a>

<img src="assets/terminal.svg" alt="sarthak@sarthak fastfetch" width="100%"/>

</div>

```console
sarthak@sarthak ~ $ cat about.md
```

I build the software between a robot's camera and its next move. Vision models that
decide, servers that dispatch, dashboards that drive real hardware, and apps that put
all of it in your pocket.

Lately: humanoids, autonomous factory floors, and teaching a 27B model to run a
production line without hallucinating a robot that doesn't exist.

```console
sarthak@sarthak ~ $ ls -l ~/projects
```

```yaml
# robofleet  ·  pip install robofleet  ·  github.com/Sarthak-code360/vlm_robofleetSDK_qwen3.8_27b
what:       Python SDK that runs a factory floor with a vision-language model as the brain
brain:      Qwen3.8-27B over any OpenAI-compatible server (llama-server, vLLM, OpenRouter)
flow:       '"print the rocket nose cone" -> pick machine + file -> print -> dispatch robot -> collect part'
dispatch:   nearest robot that can do the job without dropping under battery reserve
guardrail:  model proposes, code verifies. hallucinated IDs, battery-draining jobs and tasks
            sent to charging/faulted robots get dropped. bad model output -> rule planner takes over
hardware:   Bambu Lab A1 on LAN. FTPS:990 upload, MQTT:8883 control, live JPEG camera feed
dashboard:  "Autonomous Factory" UI. three.js 3D rocket assembly, StarForge AI chat, production runs
robots:     each one runs its own agent, heartbeats zone/battery/status, pulls tasks
security:   bearer-token API, constant-time compare (hmac.compare_digest)
core_deps:  0
ship:       GitHub Actions CI, tag-checked release -> PyPI
```

```yaml
# robot-brain  ·  perception -> decision loop
eyes:       robot camera frames captured by a React Native app I built
ingest:     frames + robot state pushed over REST to my upload server
brain:      decision server reads the stream, VLM returns the next action
robots:     humanoids and factory fleet units
edge:       STM32MP25 board on Yocto, OpenCV capture, MJPEG out, VR stereo viewer in React Native
```

```yaml
# WingmanAI  ·  github.com/Sarthak-code360/WingmanAI
what:       real-time AI copilot overlay for calls and meetings (Electron)
input:      screen capture + system audio
providers:  Gemini Live, Groq (Whisper + LLM), AWS Bedrock, or fully offline
offline:    ships llama.cpp + whisper.cpp servers per platform. Qwen 3.5 GGUF presets
            from 0.8B to 35B-A3B, or any Hugging Face repo / local .gguf. nothing leaves the machine
```

```yaml
# ev-teleop  ·  drive real electric vehicles from a browser
throughput: 250-300 cmds/sec @ 220ms across live fleets
wire:       MQTT + WebSockets + BLE, TLS/mTLS
safety:     TTL-stamped commands. firmware (Zig) drops stale ones after a reconnect
            instead of replaying them in a burst
next:       Rust QUIC gateway (quinn), WebTransport dashboard, WebRTC video
```

```console
sarthak@sarthak ~ $ spidey-sense --status
```

```diff
+ factory brain ............ online (model proposes, code verifies)
+ robot fleet .............. heartbeating
+ local models ............. running locally, no API bill
+ robofleet ................ live on PyPI
- sleep schedule ........... not found
- "quick fix" .............. took 6 hours
- the robot ................ tried to deliver a part to a robot that was charging. validator said no.
```

```console
sarthak@sarthak ~ $ ls ~/web-shooters
```

<p align="center">
  <img src="https://skillicons.dev/icons?i=ts,js,py,cpp,rust,zig,react,nextjs,electron,threejs,tailwind&theme=dark" alt="languages and frontend"/><br/>
  <img src="https://skillicons.dev/icons?i=nodejs,express,flask,postgres,mongodb,redis,aws,gcp,docker,githubactions,nginx,linux,arch,opencv&theme=dark" alt="backend, cloud and tools"/><br/><br/>
  <img src="https://img.shields.io/badge/Qwen3.8--27B-0D1117?style=flat-square&logoColor=E23636" alt="Qwen"/>
  <img src="https://img.shields.io/badge/llama.cpp-0D1117?style=flat-square" alt="llama.cpp"/>
  <img src="https://img.shields.io/badge/vLLM-0D1117?style=flat-square" alt="vLLM"/>
  <img src="https://img.shields.io/badge/whisper.cpp-0D1117?style=flat-square" alt="whisper.cpp"/>
  <img src="https://img.shields.io/badge/React_Native-0D1117?style=flat-square&logo=react&logoColor=61DAFB" alt="React Native"/>
  <img src="https://img.shields.io/badge/MQTT-0D1117?style=flat-square&logo=mqtt&logoColor=E23636" alt="MQTT"/>
  <img src="https://img.shields.io/badge/QUIC-0D1117?style=flat-square" alt="QUIC"/>
  <img src="https://img.shields.io/badge/WebRTC-0D1117?style=flat-square&logo=webrtc&logoColor=4FA3FF" alt="WebRTC"/>
  <img src="https://img.shields.io/badge/BIP--39%20%2F%20BIP--32-0D1117?style=flat-square&logo=bitcoin&logoColor=E23636" alt="BIP-39 / BIP-32"/>
  <a href="https://pypi.org/project/robofleet/"><img src="https://img.shields.io/pypi/v/robofleet?style=flat-square&label=pypi%20robofleet&color=E23636" alt="robofleet on PyPI"/></a>
</p>

```console
sarthak@sarthak ~ $ git log --oneline -7
```

```text
e1f3a9c (HEAD -> main) fix: robot no longer accepts a task at 3% battery out of pure optimism
b72c0de feat: 27B model now runs the factory. I just press "Run Factory"
4d1e9aa fix: validator rejects robots the model made up. RBT-999 was never real
7b2d04e feat: teleop latency now lower than my reaction time to Slack pings
c9a1f77 chore: renamed "final_v2_REAL_final.py" to something I won't regret
3e8b521 fix: MQTT was fine. it was DNS. it's always DNS.
0000001 init: got bitten by a radioactive bug, started writing code
```

```console
sarthak@sarthak ~ $ cat principles.txt
```

> With great `sudo` comes great responsibility.
>
> The model proposes, the code verifies.
>
> Ship steady improvements. "Perfect" never makes it to prod.

```console
sarthak@sarthak ~ $ ./connect.sh
```

<div align="center">

<a href="https://sarthaksportfolio.netlify.app/"><img src="https://img.shields.io/badge/-Portfolio-0D1B4C?style=for-the-badge&logo=netlify&logoColor=E23636" alt="Portfolio"/></a>
<a href="https://linkedin.com/in/sarthak-mishra-ba32501bb"><img src="https://img.shields.io/badge/-LinkedIn-0D1B4C?style=for-the-badge&logo=linkedin&logoColor=E23636" alt="LinkedIn"/></a>
<a href="https://pypi.org/project/robofleet/"><img src="https://img.shields.io/badge/-PyPI-0D1B4C?style=for-the-badge&logo=pypi&logoColor=E23636" alt="PyPI"/></a>
<a href="https://leetcode.com/sarthak_mishra_"><img src="https://img.shields.io/badge/-LeetCode-0D1B4C?style=for-the-badge&logo=leetcode&logoColor=E23636" alt="LeetCode"/></a>
<a href="https://www.hackerrank.com/sarthakmishra301"><img src="https://img.shields.io/badge/-HackerRank-0D1B4C?style=for-the-badge&logo=hackerrank&logoColor=E23636" alt="HackerRank"/></a>

```console
sarthak@sarthak ~ $ exit
logout: thwip.
```

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1B4C,100:B11313&height=100&section=footer" width="100%"/>
