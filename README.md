# pi-skills

My personal skills for [pi](https://github.com/badlogic/pi-coding-agent), the coding agent.

## Skills

| Skill | Description | Usage |
|---|---|---|
| [learn](learn/) | Interactive programming tutor — short explanations, runnable examples, and graduated hands-on exercises for any language, framework, or tool. Tracks your progress between sessions. | `/learn <topic>` |

## How the `learn` skill works

1. Asks (at most) two quick questions to gauge your level and goal.
2. Builds a real code workspace at `~/learning/<topic>/` — everything you make is yours to keep.
3. Teaches in a loop: **explain → show a runnable example → you do an exercise → review**.
4. Climbs a difficulty ladder: recall → apply → combine → mini-project.
5. Logs progress to `progress.md` so `/learn python` next week picks up where you left off.

## Install

```bash
git clone https://github.com/nodlac/pi-skills.git
ln -s "$PWD/pi-skills/learn" ~/.pi/agent/skills/learn
```

For the short `/learn <topic>` command, also add the prompt template:

```bash
cp prompts/learn.md ~/.pi/agent/prompts/learn.md
```

(Or just use `/skill:learn <topic>`, which needs no template.)

Run `/reload` in an active pi session after installing.
