# CFB27 Roster Tool

**Copy a team's roster, a single player, or a coaching staff from one College Football 27 dynasty save into another (PC).**

- **Full Roster.** Copy a whole team from the source save into the target save. The target team ends up with exactly the
  source team's players, with the depth chart rebuilt to match. A Preview button shows who stays, who moves in from
  elsewhere in the file, and who is cut to free agency before anything is written.
- **Individual Players.** Pick players in the source and the rows they overwrite in the target, or swap two players inside
  one save.
- **Coaches.** Copy coaches between saves.
- **Program data.** Optionally copy facilities, prestige and attendance, program points and budget, schemes and playbooks,
  AD priorities and program philosophy, and team overall ratings. Players can be left out so only program data moves.
- **Self-check.** After a Full Roster copy the tool re-opens the file it wrote and checks it. If the check fails, the log
  says so, so treat that copy as failed.

## Back up your saves first

**This tool writes dynasty save files.** Keep an untouched copy of every save before you use it. Choose a *copy* as the
Target, never your only save. The tool asks where to save the result, so pick a new file name. Load the result in the game
and check it before you replace a save you care about.

## What you need

- Windows 10 or 11.
- Two College Football 27 dynasty save files (or one, to copy between teams or swap players inside it).
- Nothing else to install. The download includes everything.

## Install and run

1. Download the zip from the latest release, **CFB27-Roster-Tool-<version>-win64.zip**.
2. Unzip it anywhere you like.
3. Open `CFB27 Roster Tool.exe` inside the `CFB27 Roster Tool-win32-x64` folder. Keep the exe next to the other files in
   that folder. It does not run on its own.

## Choosing your saves

The tool does not guess where your saves are. Use the **Choose file...** buttons under **Source** and **Target** and pick
the dynasty save file yourself. College Football 27 keeps its saves in a folder under your Documents (the EA SPORTS
College Football 27 folder). Copy the saves you want to work on somewhere handy first if you like. Any location works.

## How to use it

1. Pick a mode at the top: Full Roster, Individual Players or Coaches.
2. Source: choose the save you are copying from, then the team.
3. Target: choose the save you are copying into (a copy!), then the team.
4. Choose what to copy.
5. In Full Roster mode, click **Preview** first. It never writes anything.
6. Click the copy button, choose where to save the result, and read the log at the bottom.
7. Load the result in the game and check it.

## Known limits

- Reference fields (contracts, coach assignments, visual asset links, depth chart position and similar) are not copied
  between saves, because they point at different things in a different save. Plain values like ratings, names, physical
  attributes and traits are copied.
- Players are matched between saves by name and asset name. A same-name collision is treated as no match.
- The school's identity (name, logo, colors, uniforms), current-season state (record, polls, standings) and league-wide
  ranks are never copied.
- If a team has no spare roster rows, players who can't be placed are reported as skipped instead of being invented.
- After a game update the tool may need an update too. If a save won't open, check for a newer release.
- The download is about 120 MB because it carries its own copy of the Electron runtime.
