# Discovery Output Contract

## Purpose

Define the minimum discovery package required before client transformation moves from discovery into controlled design and implementation.

## Required outputs

### 1. Engagement mandate

Must identify:

- executive sponsor;
- engagement scope;
- success criteria;
- consultant execution authority;
- adoption authority;
- escalation path;
- confidentiality/access boundaries.

### 2. Discovery-mode declaration

One of:

- document-led;
- hybrid;
- interview-led.

Include rationale and date.

### 3. Evidence/source inventory

For each material information class:

- source;
- owner;
- authority status;
- currentness;
- known limitations;
- access method;
- reconciliation needs.

### 4. Current-State Confidence Map

Use `templates/CURRENT_STATE_CONFIDENCE_MAP.json` or a client-native equivalent preserving the same semantics.

### 5. Current operating picture

Summarize:

- workforce skeleton;
- critical recurring processes;
- key systems and working planes;
- material handoffs;
- major pain points;
- current AI/automation;
- consequential authority;
- unknowns/disputes.

### 6. Validation queue

Only unresolved items that justify additional human effort.

Prioritize by:

1. consequence if wrong;
2. confidence;
3. transformation dependency;
4. cost of validation.

### 7. Pilot recommendation

Identify one or more high-value pilot candidates and explain:

- why the work matters;
- why it is suitable for a durability/control-plane pilot;
- key dependencies;
- risk;
- current authority;
- expected measurable benefit.

The discovery team may recommend; current valid authority selects/adopts the pilot.

### 8. Bootstrap handoff

Provide the information required for M04/client control-plane bootstrap:

- client/control-repo identity;
- working planes;
- authoritative systems;
- initial state cursor;
- sponsor/adoption authority;
- first executable task;
- initial role/executor if known;
- confidentiality rules;
- unresolved discovery risks.

## Acceptance criteria

Discovery is sufficient when:

- the organization is legible enough to route work safely;
- material sources of truth are known;
- major current processes can be described without inventing them;
- consequential authority is documented or explicitly unresolved;
- inference is visibly separated from fact;
- remaining uncertainty is prioritized rather than hidden;
- a safe high-value pilot can be selected;
- the control-plane bootstrap can begin without relying on private consultant memory.

## Not required

Discovery does **not** require:

- perfect process maps;
- interviewing every employee;
- complete job architecture;
- target-state org design;
- every historical document;
- a finished enterprise ontology.

The output must be sufficient for safe transformation, not exhaustive for its own sake.
