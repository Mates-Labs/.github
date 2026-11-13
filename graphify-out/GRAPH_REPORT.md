# Graph Report - central-playwright-ci-worktree  (2026-11-13)

## Corpus Check
- 1 files · ~1,882 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 1 file(s) not represented in the graph (top: (none) 1)

## Summary
- 33 nodes · 39 edges · 6 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `fae4885e`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- secret-scan
- steps
- ci.yml
- with
- quality
- env

## God Nodes (most connected - your core abstractions)
1. `steps` - 8 edges
2. `steps` - 7 edges
3. `secret-scan` - 6 edges
4. `with` - 6 edges
5. `quality` - 6 edges
6. `contents` - 3 edges
7. `jobs` - 3 edges
8. `env` - 3 edges
9. `on` - 2 edges
10. `permissions` - 2 edges

## Surprising Connections (you probably didn't know these)
- None detected - all connections are within the same source files.

## Import Cycles
- None detected.

## Communities (6 total, 0 thin omitted)

### Community 0 - "secret-scan"
Cohesion: 0.25
Nodes (8): secret-scan, permissions, contents, permissions, name, permissions, runs-on, timeout-minutes

### Community 1 - "steps"
Cohesion: 0.36
Nodes (8): steps, steps, id, if, name, run, shell, uses

### Community 2 - "ci.yml"
Cohesion: 0.40
Nodes (4): jobs, name, on, workflow_call

### Community 3 - "with"
Cohesion: 0.40
Nodes (5): with, fetch-depth, node-version, persist-credentials, python-version

### Community 4 - "quality"
Cohesion: 0.50
Nodes (4): quality, name, runs-on, timeout-minutes

### Community 5 - "env"
Cohesion: 0.67
Nodes (3): GITLEAKS_SHA256, GITLEAKS_VERSION, env

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `steps` connect `steps` to `secret-scan`, `with`, `env`?**
  _High betweenness centrality (0.380) - this node is a cross-community bridge._
- **Why does `secret-scan` connect `secret-scan` to `steps`, `ci.yml`?**
  _High betweenness centrality (0.351) - this node is a cross-community bridge._
- **Why does `steps` connect `steps` to `with`, `quality`?**
  _High betweenness centrality (0.336) - this node is a cross-community bridge._