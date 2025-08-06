# Interactive Product Canvas Menu

## Purpose

Provide guidance for selecting and using the appropriate product canvas type based on your current product development phase and specific needs.

## Context

Different product development phases require different strategic tools. This menu helps you choose the right canvas for your current situation and guides you to the appropriate command.

## Instructions

1. **Review available canvas types:**
   - **Lean Product Canvas** - Comprehensive product strategy identifying business problems, outcomes, users, solutions, and hypotheses
   - **Lean Strategy Canvas** - 12-18 month strategy with goals, obstacles, strategic approach, and OKRs
   - **Hypothesis Prioritization Canvas** - Evaluate and prioritize product hypotheses based on value and risk
   - **Hypothesis Tests** - Design experiments to validate prioritized hypotheses
   - **OKR Roadmap** - Translate strategic OKRs into actionable quarterly roadmap

2. **Choose based on your situation:**
   - Starting a new product idea? → Lean Product Canvas
   - Planning upcoming year strategy? → Lean Strategy Canvas
   - Have several features/ideas to prioritize? → Hypothesis Prioritization
   - Have specific hypothesis to test? → Hypothesis Tests
   - Ready to define quarterly implementation plan? → OKR Roadmap

3. **Execute the appropriate command:**
   - `/create_lean_product_canvas`
   - `/create_lean_strategy_canvas`
   - `/create_hypothesis_prioritization_canvas`
   - `/create_hypothesis_tests`
   - `/create_okr_roadmap`

## Output Format

Each canvas command will guide you through the relevant process step by step and create structured documentation in the `docs/product/` directory.

## Success Criteria

- User selects appropriate canvas type for their current needs
- Clear guidance provided for each canvas option
- Proper command execution leads to structured output
- All canvas outputs are saved as Markdown documents
- Documents include proper metadata, versioning, and date information

$ARGUMENTS
