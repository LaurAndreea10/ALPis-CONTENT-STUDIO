# Contrast Audit (Initial)

## Scope
Quick manual pass for core UI tokens in dark theme.

## Findings
- Primary text (`--t1`) on background (`--bg`) is high contrast.
- Secondary text (`--t2`, `--t3`, `--t4`) may be low contrast for small labels in some contexts.
- Focus visibility was improved with explicit green outline and soft glow.

## Actions taken
- Added global `:focus-visible` outline and shadow.

## Recommended next steps
- Run a full automated audit (Lighthouse + axe).
- Raise contrast for tiny mono labels (`--t4`) where informationally critical.
- Add high-contrast mode toggle.
