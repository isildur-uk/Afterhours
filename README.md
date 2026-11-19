# Afterhours prototype

This is the first local, no-model version of Afterhours. Python 3.10+ is required; there are no third-party packages.

Run these commands from this folder:

```powershell
python simulation.py status
python simulation.py step
python simulation.py feed
python simulation.py message "Rae" "Could you try a softer dub transition?"
```

The simulation saves state, projects, visitor notes, memories, and events in `afterhours.sqlite3` beside the script. Each `step` advances one decision interval. The fallback is deterministic for a given tick and constrained to actions in `world.json`. The first mix now progresses through record browsing, selection, headphone cueing, assembly, listening back, and revision. The database is local runtime data and can be removed to start a fresh world.

The current prototype has no web interface, model calls, real-time clock, or audio playback. Visitor messages are stored for the character to consider on a later step; replies are simulated text, not sent externally.
# Afterhours
