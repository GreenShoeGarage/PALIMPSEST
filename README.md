# PALIMPSEST v3.0.0

PALIMPSEST is a local first reverse engineering studio for understanding unfamiliar objects, machines, circuits, installations, and spaces.

Its core investigation remains:

**Observe → Decompose → Measure → Infer → Test → Reconstruct**

PALIMPSEST keeps direct observations separate from proposed explanations. It preserves uncertainty, provenance, unresolved work, review conditions, and release exceptions rather than flattening the investigation into one score.

Version 3.0 introduces **PALIMPSEST Studio**, a professional shell that coordinates the complete investigation, multi-project library, diagrams, baselines, ecosystem handoffs, review, and controlled release workflow.

## Quick start

1. Open `palimpsest-v3.0.0.html` in a current browser.
2. Choose **Guided setup**, load the demo, or open **Studio**.
3. Define the investigation mission, scope, exclusions, owner, target date, disposition, and required deliverables.
4. Work through Observe, Decompose, Measure, Infer, Test, and Reconstruct.
5. Use the Studio work queue to find blockers, weak hypotheses, pending tests, reconstruction work, and open review comments.
6. Capture named baselines before disassembly, repair, modification, or reconstruction.
7. Review each release gate independently.
8. Capture a release candidate, resolve or document exceptions, and mark the investigation released when appropriate.
9. Export JSON and portable project packages regularly.

The HTML application is self contained and can be opened directly from disk. PWA installation and service-worker caching require serving the included app files through HTTPS or localhost.

## PALIMPSEST Studio

The Studio workspace provides one project-level command center for all PALIMPSEST capabilities.

### Investigation mission brief

The brief records:

- Investigation mission
- Owner
- Priority
- Target date
- Intended disposition
- Work included in scope
- Work intentionally excluded
- Required deliverables
- Release label and release notes

The mission brief is stored with the project and included in Studio exports.

### Studio work queue

The queue brings together actionable work from across the application:

- Explicit workflow blockers
- Missing and suspected components
- Low-confidence or unresolved hypotheses
- Planned and ready tests
- Blocked reconstruction steps
- Open review comments

Items retain their source stage and open the appropriate workspace directly.

### Release gates

PALIMPSEST v3.0 keeps release readiness separated into visible dimensions:

- Evidence
- Structure
- Dimensions
- Reasoning
- Verification
- Interfaces
- Safety
- Review
- Reconstruction

A gate can be **Pass**, **Attention**, or **Not ready**. These conditions are never collapsed into one readiness score.

### Controlled releases

The Studio release workflow supports:

- Named release labels
- Release candidate capture
- Automatic baseline creation with each candidate
- Gate-state snapshot at candidate time
- Release history
- Release with visible exceptions
- Reopening a released investigation
- Studio manifest export

Marking a project released does not erase unresolved records or review conditions.

### Command palette

Open the command palette with:

- `Ctrl + Shift + P` on Windows and Linux
- `Command + Shift + P` on macOS

The palette can navigate workspaces, create common records, capture baselines, save views, prepare releases, export reports, and toggle focus or field modes.

### Saved workspace views

A saved view remembers the active workspace and record-density preference. Saved views appear on the Studio dashboard for quick return to repeated investigation tasks.

### Focus mode

Focus mode reduces persistent interface chrome while retaining project navigation. It is useful for review sessions, diagrams, field entry, and projected workshop use.

## Core workflow

### Observe

- Guided investigation setup
- Multiple reference photographs
- Camera-compatible capture
- Layered image annotations
- Observed, inferred, unknown, damage, interface, and measurement layers
- Vector field sketches
- Direct observation register

### Decompose

- Hierarchical assembly tree
- Assemblies, subassemblies, components, and features
- Component photographs and states
- Parent-child relationships
- Fasteners, access constraints, removal tools, and disassembly sequence
- Mechanical, electrical, data, fluid, thermal, spatial, and human connections
- Exploded diagrams

### Measure

- Measurement sessions
- Repeated readings
- Minimum, maximum, mean, and range
- Unit conversion
- Instruments and calibration information
- Datum references
- Derived formulas
- Tolerance stack analysis
- Dimensional conflict warnings

### Infer

- Hypothesis register
- Supporting and contradicting evidence
- Assumptions and alternatives
- Confidence rationale and history
- Dependency and circular reasoning checks
- Uncertainty mapping
- Explicit disconfirmation criteria

### Test

- Reproducible protocols
- Equipment and preconditions
- Procedure, hazards, and preservation risks
- Expected results and pass/fail criteria
- Recorded results
- Linked hypotheses, measurements, and images
- Suggested confidence changes requiring user approval

### Reconstruct

- Repair, restore, replicate, adapt, simulate, and documentation-only objectives
- Independent fidelity targets
- Reconstruction BOM
- Make, buy, salvage, repair, substitute, and existing decisions
- Step dependencies, tools, skills, materials, effort, blockers, and acceptance criteria
- Deviation register
- Final target-versus-actual comparison

## Investigation workspaces

### Library

- Multiple local projects
- Search, tags, status filtering, duplication, archive, and deletion
- Project thumbnails
- Related investigations
- Storage estimates
- Safe project switching

### Baselines and comparison

- Named snapshots
- Current-state comparison
- Added, removed, and changed records
- Change report export
- Safe restoration with automatic pre-restore baseline

### Advanced diagrams

- Functional decomposition
- Connection graph
- Electrical block
- Signal flow
- Mechanical relationship
- Fluid path
- Thermal path
- Spatial adjacency
- Disassembly sequence
- Manual node editing and SVG export

### Spatial reverse engineering

- Plan, site image, and photograph backgrounds
- Two-point scale calibration
- Zones, routes, utilities, viewpoints, dimensions, and hidden spaces
- Observed, inferred, and unknown states
- Layer controls and SVG export

## Field Instrument handoffs

### Trace

Observations, measurements, and completed tests become evidence. Hypotheses remain claims. Supporting and contradicting links and PALIMPSEST provenance are retained.

### Handshake

Traced component connections become interface records. Controlled decisions can return to PALIMPSEST by stable source connection or interface identity without replacing original evidence.

### COGWRIGHT

Possible gears, pulleys, sprockets, shafts, and rotating components can be prepared as editable reference profiles. Generated outlines require validation before fabrication.

### Makefile

Reconstruction steps become tasks, dependencies remain dependencies, BOM records remain BOM items, tests become verification records, and unresolved high-impact hypotheses become project risks.

## Review and handoff

PALIMPSEST supports local-first peer review with:

- Reviewer directory
- Record-linked comments
- Critical, major, minor, and question severities
- Comment responses and status history
- Separate approvals for evidence, measurements, interfaces, safety, testing, and reconstruction
- Local signoffs
- Read-only review packages
- External response JSON import

Local signoffs are accountability records, not cryptographic signatures or substitutes for required organizational approval systems.

## Portable project package

The v3.0 package includes:

```text
project.json
report.html
manifest.json
studio/
  studio-manifest.json
  work-queue.csv
release/
  release-record.json
data/
images/
sketches/
diagrams/
spatial/
baselines/
handoffs/
  trace/
  handshake/
  cogwright/
  makefile/
review/
app/
  palimpsest.html
  manifest.webmanifest
  icon.svg
  sw.js
```

Use `project.json` to continue editing. Use `report.html` for the evidence dossier. Studio and release records preserve the project-level mission, open work, gate conditions, and release history.

## Local storage and backups

PALIMPSEST stores project data in the browser and uses IndexedDB for image media where available. Browser storage is not a durable archive.

Export regularly before:

- Clearing browser data
- Changing browsers or devices
- Major disassembly or reconstruction work
- Restoring an older baseline
- Installing a significantly newer release

## Keyboard shortcuts

Existing shortcuts include stage navigation, capture, search, undo, redo, reports, backups, and field mode. v3.0 adds:

| Shortcut | Action |
|---|---|
| `Ctrl/Command + Shift + P` | Open command palette |
| `Ctrl/Command + K` | Search the investigation |
| `1` through `6` | Open the six investigation stages when focus is not in a form field |

## Privacy

PALIMPSEST does not require an account or server. Project information stays in the browser unless the user exports or deliberately shares it.

Reference photographs and reports can contain sensitive technical, personal, location, or proprietary information. Review packages before sharing them.

## Compatibility

Recommended browsers:

- Current Chromium-based browsers
- Current Firefox
- Current Safari

Direct file use supports the principal application. Camera, speech recognition, PWA installation, and some storage behaviors depend on browser and security context.

## Migration

PALIMPSEST v3.0 migrates projects created by v1.0 through v2.9. New Studio fields are added without deleting earlier records.

Keep an exported JSON backup before migration when the project is important.

## Version

**PALIMPSEST v3.0.0 — Studio Release**
