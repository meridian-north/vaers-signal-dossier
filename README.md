# VAERS, rebuilt clean — in a weekend

An open, reproducible rebuild of U.S. VAERS plus a five-nation safety-signal
analysis — assembled with AI assistance over a weekend, to show that a clean,
searchable vaccine-safety surveillance view can be built
cheaply and verified by anyone.

**The webform / evidence page:** `index.html` (open it in any browser, or via the
GitHub Pages link below). Self-contained — no server, no tracking.

## What it demonstrates

1. **The signal is real and cross-national.** Disproportionality computed
   directly from the raw data shows the myocarditis pattern (young-male,
   dose-related) converging across **five independent national systems** —
   VAERS (US), MHRA (UK), TGA (AU), JADER (JP), CVAR (CA) — while a control
   (anaphylaxis) correctly comes out the other way. A pattern that replicates
   across five systems with no shared reporting infrastructure is not a US
   artifact.

2. **Signals, not proven links.** Every metric here is a *signal* metric
   (disproportionality), the thing surveillance exists to find — not proof of
   cause. A signal is a question that earns investigation; acting on one does not
   require a proven link.

3. **The one thing every system lacks: a denominator.** Spontaneous reporting is
   a numerator with no denominator, so a *rate* ("per million doses") is
   structurally impossible from it. The denominator exists (dose-administration
   data, active cohorts, registries) and is publicly funded — it is simply not
   surfaced alongside the signal in real time. The civic ask is to join them.

## The claim

This was assembled in a weekend with AI assistance (claude.ai). If two people and
a weekend can produce a searchable, cross-nationally validated
view of public safety data, the publicly funded systems that hold this data can
do at least as well — and release the denominator in
real time.

## Honesty guardrails (baked in)

- Disproportionality is labeled a signal metric, not causation.
- Cross-system *levels* are not comparable (different reporting environments);
  the convergent findings are demonstrated in **direction and timing**, not
  magnitude.
- The death signal is reported as the **weakest and most confounded** (elderly-
  skewed, denominator-dependent), not inflated.
- Confirmed relative risks in the historical "signal → action" set come from
  controlled studies (case-control, self-controlled case series, cohort), not
  from VAERS.

## Reproduce it

The dataset and method are designed to be re-derived: same public CDC input +
same fixed method → same output, with content hashes and a manifest so any number
can be traced to its source row. The analysis queries are deterministic DuckDB
over the harmonized source files.

## Not

Not medical advice. Not affiliated with CDC, FDA, or any manufacturer or agency.
Not a claim that any vaccine caused any individual outcome — that requires the
controlled studies a reporting system cannot perform alone.

## License

Code: MIT. Data: public-domain / CC0 (derived from public CDC and peer-agency
sources). Cite freely; verify everything.
