# Software Engineering Principles Applied to Literary Creation: A Cross-Disciplinary Experiment

**Systematic Poetry Composition Using Agile, TDD, and Large Language Models**

---

## Executive Summary

This paper analyzes a cross-disciplinary experiment applying software engineering methodologies (Agile/SCRUM, Test-Driven Development, pair programming, continuous integration, parallel execution) to literary creation. Over 5 sprints, we adapted Shakespeare's Romeo & Juliet into a 400-stanza Russian verse novel using Pushkin's Onegin stanza form, treating poetry as an engineering problem requiring systematic decomposition, quality gates, and iterative development.

**Key Findings**: (1) SE principles successfully structured creative work, enabling completion of complex literary project; (2) Framework-driven development (analogous to software libraries) proved highly effective; (3) Parallel execution achieved 6.5× speedup; (4) Human-LLM pair programming effective for systematic tasks but limited for creative intuition; (5) TDD-style quality gates worked but required subjective assessment; (6) Agile sprints effective for planning but velocity metrics unreliable; (7) Over-systematization risks harming artistic quality.

**Contributions**: Novel application of full SE methodology stack to creative domain; replicable process for large-scale literary projects; insights into LLM capabilities/limitations in systematic creative work; analysis of when engineering helps vs. hinders creativity.

---

## 1. Introduction: Engineering Meets Literature

### 1.1 The Experiment

We conducted a controlled experiment: **Can software engineering methodologies—designed for code—effectively structure poetry composition?**

**Project**: Adapt Romeo & Juliet → 400-stanza Russian verse novel (Onegin stanza form)
**Duration**: 5 sprints (Sprints 35-39)
**Team**: 1 human expert + multiple Claude Sonnet 4.5 LLM instances
**Methodologies**: Agile/SCRUM, Kanban, TDD, pair programming, CI/CD, parallel execution

### 1.2 Why This Matters

**Computer Science**: Tests LLM capabilities beyond code generation; explores human-AI collaboration models; demonstrates systematic approaches to creative AI

**Literary Studies**: Provides replicable methodology for verse composition; challenges "inspiration-only" creative paradigms; enables project management for large literary works

**Cross-Disciplinary**: Case study in domain transfer; analysis of when engineering principles enhance vs. constrain creativity

---

## 2. Software Engineering Principles Applied

### 2.1 Agile/SCRUM Framework

**Sprint Structure** (5 sprints, 1 week each):

**Sprint 35-37**: Research Phase
- Sprint Goal: Establish technical and cultural foundation
- Deliverables: 250,000+ words across 10 research documents
- Definition of Done: All technical specs documented, tools identified
- Retrospective: Comprehensive but perhaps excessive documentation

**Sprint 38**: Framework Development
- Sprint Goal: Create compositional support for all 400 stanzas
- Deliverables: 82 framework files, 90,000+ lines
- Definition of Done: All frameworks marked "ready for composition"
- Retrospective: **CRITICAL DISCOVERY** - quality varied dramatically, many frameworks inadequate

**Sprint 39**: Enhancement and Composition
- Phase 1: Pre-composition enhancements (4 tasks)
- Phase 1B: Critical issue resolution (2 tasks - added post-audit)
- Phase 2: Novel composition (8 parallel tasks)
- Definition of Done: 400 stanzas composed, technically compliant
- Retrospective: Parallel execution successful; quality assessment deferred

**Agile Adaptations for Creative Work**:
- ✅ Sprint planning provided structure and clarity
- ✅ Incremental delivery prevented overwhelming scope
- ✅ Retrospectives identified issues (Phase 1B crisis)
- ⚠️ Velocity estimation unreliable (creative work inherently uncertain)
- ⚠️ "Working software" analog unclear (when is poetry "working"?)

### 2.2 Test-Driven Development (TDD)

**Traditional TDD**: Red (write failing test) → Green (minimal code) → Refactor

**Literary TDD Adaptation**:

**Red - Specify First**:
```
Framework for Stanza 54 (Lark & Nightingale):
Requirements:
  - Content: Dawn parting scene, "lark vs nightingale" debate
  - Voice: Yulia (gentle, denying), Roman (urgent, protective)
  - Emotional arc: Reluctance → denial → reality → acceptance → parting
  - Technical: 14 lines, aBaBccDDeFFeGG, iambic tetrameter
  - Line 8: Mandatory stress syllable 8
  - Forbidden: No verb rhymes
  - Quality: Heartrending (reader should feel sadness)
```

**Green - Compose to Spec**:
- Use framework vocabulary (pre-verified stress patterns)
- Apply framework rhyme pairs
- Follow emotional beat guidance
- Meet all technical requirements

**Refactor - Polish**:
- Read aloud for naturalness
- Strengthen weak rhymes
- Smooth phrasing
- Verify voice consistency

**Quality Gates** (before progression):
- ✅ Technical compliance (meter, rhyme, structure)
- ✅ Voice consistency
- ✅ Content requirements met
- ✅ No forbidden elements
- ✅ Read-aloud test passed

**Effectiveness**:
- ✅ Framework-as-specification provided clear targets
- ✅ Quality gates prevented progression with defects
- ✅ Specification-first reduced creative paralysis
- ⚠️ "Tests" ultimately subjective (human judgment required)
- ⚠️ Over-specification risked constraining creativity

### 2.3 Pair Programming: Human-LLM Collaboration

**Traditional Pair Programming**: Driver (writes code) + Navigator (reviews, thinks strategically)

**Our Model**: Human (Navigator) + LLM (Driver)

**Human Role** (Strategic):
- Define sprint goals and task specifications
- Provide creative direction
- Make final quality judgments
- Handle subjective aesthetic decisions
- Recognize when LLM output inadequate

**LLM Role** (Execution):
- Synthesize research systematically
- Generate framework structures
- Compose verse drafts using frameworks
- Perform technical verifications
- Document process

**Communication Protocol**:
```
Human: "Compose Chapter 1 (55 stanzas) using frameworks.
        Follow aBaBccDDeFFeGG rhyme scheme.
        Narrator voice: 60% ironic, 30% philosophical.
        Use pre-verified vocabulary/rhymes."

LLM: [Executes, generates 770 lines]

LLM: "Chapter 1 complete. 55 stanzas delivered.
      Technical compliance attempted.
      NOTE: Stress patterns require native speaker verification."      Human reviews output, notes limitations."