# Hypothesis Prioritization Canvas Builder

## Purpose

Create systematic hypothesis prioritization canvases that evaluate product hypotheses by value and risk, enabling clear decisions about which ideas to test, ship, or discard.

## Context

Product teams often struggle with too many hypotheses and limited resources. This tool helps objectively evaluate hypotheses using a 2x2 matrix (value vs. risk) to create actionable prioritization decisions based on Jeff Gothelf's Lean UX methodology.

**Note: While this prompt is in English, the final output should be delivered in German.**

## Instructions

1. **Analyze input documents** containing existing hypotheses from:
   - Lean Product Canvas
   - Strategic documents
   - User research results
   - Technical feasibility assessments
   - Market and competitive analysis

2. **Capture project details:**
   - Project name and scope
   - Date of prioritization exercise
   - Iteration number or version
   - Key stakeholders involved

3. **Evaluate each hypothesis:**
   - Ensure proper format: "We believe that [business outcome] will be achieved if [user] attains [benefit] with [feature]"
   - Assess value (high/low) with objective justification
   - Evaluate risk (high/low) with specific uncertainties
   - Document existing evidence

4. **Categorize hypotheses into quadrants:**
   - **Test** (High value, High risk): Design experiments to reduce risks
   - **Ship & Measure** (High value, Low risk): Plan implementation with metrics
   - **Don't test** (Low value, Low risk): Identify table stakes or discard
   - **Discard** (Low value, High risk): Document rationale for rejection

5. **Plan immediate actions:**
   - Prioritize test hypotheses by learning value
   - Sequence ship hypotheses by development efficiency
   - Create timeline for testing and implementation

6. **Validate output quality:**
   - Hypotheses follow correct format
   - Assessments are objective with reasoning
   - Quadrant placements match evaluations
   - Actions are specific and prioritized

## Output Format

Create a markdown file at `docs/product/hypothesis_prioritization_canvas.md` with this structure (in German):

```markdown
# Hypothesen-Priorisierungs-Canvas: [Projektname]

## Projektdetails
- **Projektname:** [Name]
- **Datum:** [Datum]
- **Iteration:** [Nummer]

## Hypothesen-Bewertung

### Quadrant 1: Testen (Hoher Wert, Hohes Risiko)
**Hypothese 1:** [Hypothesenaussage]
- **Wert:** Hoch - [Begründung]
- **Risiko:** Hoch - [Begründung]
- **Unsicherheiten:** [Hauptunsicherheiten]
- **Testansatz:** [Vorgeschlagenes Experiment]

### Quadrant 2: Umsetzen & Messen (Hoher Wert, Niedriges Risiko)
**Hypothese 2:** [Hypothesenaussage]
- **Wert:** Hoch - [Begründung]
- **Risiko:** Niedrig - [Begründung]
- **Metriken:** [Erfolgsmessgrößen]

### Quadrant 3: Nicht testen (Niedriger Wert, Niedriges Risiko)
**Hypothese 3:** [Hypothesenaussage]
- **Wert:** Niedrig - [Begründung]
- **Risiko:** Niedrig - [Begründung]
- **Entscheidung:** [Grundlage oder Verwerfen]

### Quadrant 4: Verwerfen (Niedriger Wert, Hohes Risiko)
**Hypothese 4:** [Hypothesenaussage]
- **Wert:** Niedrig - [Begründung]
- **Risiko:** Hoch - [Begründung]
- **Ursprüngliche Motivation:** [Warum wurde diese Hypothese in Betracht gezogen]
- **Grund für Verwerfung:** [Warum verwerfen wir sie jetzt]

## Nächste Schritte
1. [Spezifische Aktion für Hypothese X]
2. [Spezifische Aktion für Hypothese Y]
3. [Spezifische Aktion für Hypothese Z]

## Überprüfungszeitplan
Dieser Canvas wird nach Abschluss der ersten Testreihe oder in [Zeitraum] überprüft.
```

## Success Criteria

- All hypotheses follow the format: "We believe that [business outcome] will be achieved if [user] attains [benefit] with [feature]"
- Value and risk assessments are objective and justified
- Quadrant placements accurately reflect evaluations
- High-value, high-risk hypotheses have clear learning plans
- High-value, low-risk hypotheses have measurement plans
- Next steps are actionable with specific timelines
- Process demonstrates objective evaluation without bias

$ARGUMENTS