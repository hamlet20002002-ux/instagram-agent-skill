# Graph Report - instagram-agent-skill  (2026-10-26)

## Corpus Check
- cluster-only mode — file stats not available

## Summary
- 202 nodes · 465 edges · 12 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS · INFERRED: 2 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `d79da3ea`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- json
- re
- .claude/skills/ig-human/detect.py
- skills/ig-human/detect.py
- argparse
- .claude/skills/ig-reel/hookscore.py
- skills/ig-reel/hookscore.py
- .claude/skills/ig-viral/swipe.py
- sys
- skills/ig-viral/swipe.py
- .claude/skills/ig-reel/beats.py
- marketplace.json

## God Nodes (most connected - your core abstractions)
1. `main()` - 10 edges
2. `main()` - 10 edges
3. `humanize()` - 9 edges
4. `humanize()` - 9 edges
5. `run()` - 9 edges
6. `run()` - 9 edges
7. `check_voice()` - 8 edges
8. `run()` - 8 edges
9. `scale()` - 8 edges
10. `check_voice()` - 8 edges

## Surprising Connections (you probably didn't know these)
- `main()` --calls--> `argparse`  [EXTRACTED]
  .claude/skills/ig-human/humanize.py →   _Bridges community 0 → community 4_
- `pass_invisible()` --calls--> `re`  [EXTRACTED]
  .claude/skills/ig-human/humanize.py →   _Bridges community 0 → community 1_
- `pass_invisible()` --calls--> `unicodedata`  [EXTRACTED]
  .claude/skills/ig-human/humanize.py →   _Bridges community 0 → community 2_
- `main()` --calls--> `argparse`  [EXTRACTED]
  skills/ig-human/humanize.py →   _Bridges community 1 → community 4_
- `pass_invisible()` --calls--> `unicodedata`  [EXTRACTED]
  skills/ig-human/humanize.py →   _Bridges community 1 → community 2_

## Import Cycles
- None detected.

## Communities (12 total, 0 thin omitted)

### Community 0 - "json"
Cohesion: 0.14
Nodes (13): _cp(), humanize(), load_lexicon(), main(), _match_case(), pass_invisible(), pass_lexical(), pass_typographic() (+5 more)

### Community 1 - "re"
Cohesion: 0.15
Nodes (13): _cp(), humanize(), load_lexicon(), main(), _match_case(), pass_invisible(), pass_lexical(), pass_typographic() (+5 more)

### Community 2 - ".claude/skills/ig-human/detect.py"
Cohesion: 0.18
Nodes (13): bar(), check_burstiness(), check_fingerprint(), check_slop(), check_specificity(), check_voice(), clamp(), main() (+5 more)

### Community 3 - "skills/ig-human/detect.py"
Cohesion: 0.19
Nodes (13): bar(), check_burstiness(), check_fingerprint(), check_slop(), check_specificity(), check_voice(), clamp(), main() (+5 more)

### Community 4 - "argparse"
Cohesion: 0.17
Nodes (10): analyse(), main(), render(), render_box(), visible_window(), analyse(), main(), render() (+2 more)

### Community 5 - ".claude/skills/ig-reel/hookscore.py"
Cohesion: 0.22
Nodes (12): bar(), check_address(), check_frontload(), check_length(), check_specificity(), check_stakes(), clamp(), main() (+4 more)

### Community 6 - "skills/ig-reel/hookscore.py"
Cohesion: 0.22
Nodes (12): bar(), check_address(), check_frontload(), check_length(), check_specificity(), check_stakes(), clamp(), main() (+4 more)

### Community 7 - ".claude/skills/ig-viral/swipe.py"
Cohesion: 0.27
Nodes (7): analyse(), classify(), load_formulas(), main(), read_rows(), render(), to_markdown()

### Community 8 - "sys"
Cohesion: 0.29
Nodes (7): analyse(), main(), pretty(), render(), split_beats(), tc(), words()

### Community 9 - "skills/ig-viral/swipe.py"
Cohesion: 0.29
Nodes (7): analyse(), classify(), load_formulas(), main(), read_rows(), render(), to_markdown()

### Community 10 - ".claude/skills/ig-reel/beats.py"
Cohesion: 0.31
Nodes (7): analyse(), main(), pretty(), render(), split_beats(), tc(), words()

### Community 11 - "marketplace.json"
Cohesion: 0.25
Nodes (7): description, name, owner, name, url, plugins, $schema

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `check_voice()` connect `.claude/skills/ig-human/detect.py` to `re`, `skills/ig-human/detect.py`?**
  _High betweenness centrality (0.019) - this node is a cross-community bridge._
- **Should `json` be split into smaller, more focused modules?**
  _Cohesion score 0.1422924901185771 - nodes in this community are weakly interconnected._