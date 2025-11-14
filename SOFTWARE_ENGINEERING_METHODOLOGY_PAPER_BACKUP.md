# Software Engineering Principles Applied to Literary Creation: A Cross-Disciplinary Experiment in Systematic Poetry Composition

**An Academic Analysis of Agile Methodologies, Test-Driven Development, and Large Language Model Integration in Verse Novel Adaptation**

---

## Abstract

This paper presents a rigorous analysis of a cross-disciplinary experiment applying software engineering principles—specifically Agile methodologies (SCRUM/Kanban), Test-Driven Development (TDD), pair programming, and Large Language Model (LLM) integration—to literary creation. The project adapted Shakespeare's *Romeo and Juliet* into a 400-stanza Russian verse novel using Pushkin's Onegin stanza form, treating literary creation as an engineering problem requiring systematic decomposition, iterative development, quality assurance, and continuous integration.

Spanning five sprints over multiple weeks, the project applied: (1) **Sprint-based planning** with clear acceptance criteria and deliverables, (2) **Task decomposition** breaking complex creative work into manageable units, (3) **Framework-driven development** analogous to software libraries, (4) **Test-driven refinement** with explicit quality gates, (5) **Pair programming** between human expert and LLM, (6) **Parallel execution** using multiple AI agents, and (7) **Version control** with Git for all artifacts.

Results demonstrate that software engineering principles successfully structure creative work, reducing cognitive overhead and enabling systematic progress tracking. However, critical findings reveal limitations: (1) creative work resists complete systematization (over-specification may harm artistry), (2) "testing" literary quality requires subjective human judgment unlike objective unit tests, (3) LLM pair programming effective for systematic tasks but limited for creative intuition, (4) sprint velocity metrics misleading when quality assessment delayed.

This experiment contributes to both computer science (LLM applications in creative domains, human-AI collaboration models) and literary studies (systematic approaches to verse composition, computational poetics). The methodology is replicable for other large-scale creative projects, though with caveats about the tension between engineering rigor and artistic freedom.

**Keywords**: Software engineering, Agile methodology, SCRUM, Kanban, Test-Driven Development, Large Language Models, human-AI collaboration, computational creativity, verse composition, digital humanities, systematic literary creation

---

## 1. Introduction

### 1.1 The Experiment: Engineering Meets Literature

Traditional approaches to literary creation emphasize inspiration, organic process, and artistic intuition. This experiment inverts the paradigm: **What if we treat poetry composition as an engineering problem?**

Between [Sprint 35-39 dates], we conducted a cross-disciplinary experiment applying rigorous software engineering methodologies to create a 400-stanza verse novel—a substantial literary work with highly technical formal constraints. The project deliberately employed:

- **Agile/SCRUM Framework**: 5 sprints with defined goals, acceptance criteria, retrospectives
- **Kanban Task Management**: Visual task boards, WIP limits, flow optimization
- **Test-Driven Development (TDD)**: Quality gates before progression, specification-first approach
- **Pair Programming**: Human-LLM collaboration throughout development
- **Continuous Integration**: Git version control, frequent commits, branch management
- **Parallel Execution**: Multiple AI agents working simultaneously (distributed computing)
- **Quality Assurance**: Comprehensive audits, technical verification, acceptance testing

The literary artifact—a Russian verse novel adapting Shakespeare's *Romeo and Juliet*—served as the "software product" being engineered.

### 1.2 Motivation: Why Apply SE to Literature?

**Software Engineering Perspective**:
- Large Language Models (LLMs) represent new "developers" in human-AI teams
- Creative domains test LLM capabilities beyond code generation
- Systematic methodologies may scale to complex creative projects
- Replicable processes enable quality control and knowledge transfer

**Literary Perspective**:
- Verse novels are highly constrained (like software specs)
- 400 stanzas = large-scale project requiring project management
- Formal poetry has "testable" technical requirements (meter, rhyme, structure)
- Systematic approaches may reduce creative paralysis, enable completion

**Cross-Disciplinary Hypothesis**:
> Engineering methodologies successfully applied to code (a highly structured creative artifact) might transfer to poetry (another highly structured creative artifact), with adaptations for subjective quality assessment.

### 1.3 Research Questions

1. **Applicability**: Can software engineering methodologies structure literary creation effectively?

2. **Agile Fit**: Do Agile/SCRUM principles adapt to creative work's different nature?

3. **TDD in Literature**: Can "test-driven" approaches apply when "tests" are subjective judgments?

4. **LLM Pair Programming**: How does human-AI collaboration compare to human-human pair programming?

5. **Quality Metrics**: What metrics meaningfully measure literary work progress and quality?

6. **Systematic vs. Organic**: Does engineering rigor enhance or constrain creativity?

7. **Scalability**: Does methodology scale from short poems to 400-stanza novels?

8. **Replicability**: Can others reproduce results using documented processes?

### 1.4 Contributions

This paper contributes to:

**Computer Science**:
- Novel application of SE methodologies to creative domains
- LLM integration in systematic creative workflows
- Human-AI collaboration models for non-code tasks
- Distributed computing approaches to literary creation (parallel agents)

**Literary Studies / Digital Humanities**:
- Systematic methodology for large-scale verse composition
- Framework-driven approach to formal poetry
- Computational support for traditional literary forms
- Replicable process for verse novel adaptation

**Cross-Disciplinary**:
- Case study in domain transfer (engineering → literature)
- Analysis of when engineering principles help vs. hinder creativity
- Methodology applicable to other creative domains (music composition, visual art, etc.)

### 1.5 Paper Organization

Section 2 reviews relevant work in SE methodologies and computational creativity. Section 3 details the experimental methodology. Sections 4-8 analyze each SE principle's application (Agile, TDD, pair programming, CI/CD, parallel execution). Section 9 evaluates quality metrics. Section 10 discusses tensions between engineering and creativity. Section 11 presents comparative analysis. Section 12 offers recommendations. Section 13 concludes.

---

## 2. Background and Related Work

### 2.1 Software Engineering Methodologies

#### 2.1.1 Agile and SCRUM

**Core Principles** (Agile Manifesto, Beck et al., 2001):
- Individuals and interactions over processes and tools
- Working software over comprehensive documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan

**SCRUM Framework** (Schwaber & Sutherland, 2020):
- **Sprints**: Time-boxed iterations (1-4 weeks)
- **Sprint Planning**: Define sprint goal and tasks
- **Daily Standups**: Quick status updates
- **Sprint Review**: Demonstrate completed work
- **Sprint Retrospective**: Continuous improvement
- **Product Backlog**: Prioritized feature list
- **Definition of Done**: Clear completion criteria

**Typical Application**: Software development teams
**Our Application**: Literary creation process

#### 2.1.2 Kanban

**Core Concepts** (Anderson, 2010):
- **Visualize Work**: Task boards showing status
- **Limit WIP**: Work-in-progress constraints prevent overload
- **Manage Flow**: Optimize task progression
- **Explicit Policies**: Clear rules for task movement
- **Feedback Loops**: Regular reviews and adjustments
- **Collaborative Improvement**: Team-driven optimization

**Typical Application**: DevOps, continuous delivery
**Our Application**: Creative task flow management

#### 2.1.3 Test-Driven Development (TDD)

**Red-Green-Refactor Cycle** (Beck, 2003):
1. **Red**: Write failing test first
2. **Green**: Write minimal code to pass test
3. **Refactor**: Improve code while maintaining pass

**Principles**:
- Specification before implementation
- Automated verification
- Incremental development
- Continuous quality assurance

**Typical Application**: Unit testing in software
**Our Application**: Quality gates in verse composition

#### 2.1.4 Pair Programming

**Model** (Williams & Kessler, 2002):
- **Driver**: Writes code
- **Navigator**: Reviews in real-time, thinks strategically
- Roles rotate frequently
- Continuous communication and collaboration

**Benefits Claimed**:
- Higher quality code
- Knowledge sharing
- Reduced bugs
- Better design decisions

**Typical Application**: Two human developers
**Our Application**: Human-LLM collaboration

### 2.2 Large Language Models in Creative Work

**Recent Developments**:
- GPT-3/4 (Brown et al., 2020): 175B+ parameter language models
- Claude (Anthropic, 2023): Constitutional AI with extended context
- Demonstrated capabilities: Code generation, creative writing, reasoning

**Creative Applications**:
- Story generation (Roemmele & Gordon, 2018)
- Poetry composition (Gervás, 2013; Veale, 2013)
- Dialogue writing (Zhou et al., 2020)
- Game narrative design (Guzdial et al., 2015)

**Limitations Documented**:
- Difficulty maintaining long-form consistency
- Struggles with highly technical constraints
- Non-native language competence limited
- Subjective quality assessment unreliable

**Our Experiment Position**: Treats LLM as "junior developer" in pair programming model, requiring human "senior developer" oversight.

### 2.3 Computational Creativity

**Boden's Framework** (2004):
- **Combinatorial Creativity**: Novel combinations of familiar ideas
- **Exploratory Creativity**: Pushing boundaries of established style
- **Transformational Creativity**: Changing fundamental rules

**Evaluation Criteria** (Colton et al., 2011):
- **Value**: Is output worth creating?
- **Novelty**: Is output original?
- **Quality**: Is output well-crafted?

**Computational Poetry Specific**:
- ASPERA (Gervás, 2000): Automatic Spanish poetry generation
- WASP (Gervás et al., 2007): Full poetry generation system
- PoeTryMe (Gonçalo Oliveira, 2012): Template-based Portuguese poetry

**Our Experiment**: Hybrid human-AI approach vs. fully automated systems

### 2.4 Systematic Approaches to Literature

**Historical Precedents**:
- **Oulipo Movement** (1960s): Mathematical constraints in literature (Queneau, Perec)
- **Procedural Writing**: Rule-based text generation
- **Algorithmic Poetry**: Computer-assisted verse (pre-LLM era)

**Modern Digital Humanities**:
- **Computational Poetics**: Algorithmic analysis of verse structure
- **Digital Scholarly Editing**: Version control for literary texts
- **Collaborative Writing Platforms**: Systematic co-authorship

**Gap**: Few documented attempts to apply full SE methodology stack to single large literary work.

### 2.5 Human-AI Collaboration Models

**Existing Frameworks**:
- **AI as Tool**: Human fully in control, AI provides suggestions
- **AI as Collaborator**: Peer relationship, mutual influence
- **AI as Autonomous Agent**: AI works independently, human reviews

**Documentation Systems**:
- **Ghostwriter** (Roemmele et al., 2015): Story writing assistant
- **Dramatron** (Mirowski et al., 2022): AI co-playwright
- **Wordcraft** (Yuan et al., 2022): AI-assisted writing tool

**Our Model**: Pair programming adaptation—human as "navigator" (strategic), LLM as "driver" (execution), roles documented throughout.

---

## 3. Experimental Methodology

### 3.1 Project Overview

**Artifact**: 400-stanza Russian verse novel adapting *Romeo and Juliet*
**Form**: Pushkin's Onegin stanza (14 lines, aBaBccDDeFFeGG rhyme, iambic tetrameter)
**Duration**: 5 sprints (Sprints 35-39)
**Team**: 1 human expert + multiple Claude Sonnet 4.5 LLM instances
**Tools**: Git, Markdown, command-line interface, todo tracking

### 3.2 Sprint Structure (Agile/SCRUM)

Each sprint followed SCRUM framework adapted for creative work:

#### Sprint 35: Research Phase - Russian Prosody (Week 1)
- **Sprint Goal**: Establish technical foundation for Russian verse composition
- **Sprint Planning**: Define research documents needed (prosody, meter, rhyme)
- **Tasks**: 8 research tasks (Russian stress rules, rhyme types, forbidden rhymes, etc.)
- **Deliverables**: Technical guides documenting Onegin stanza requirements
- **Definition of Done**: All technical specs documented with examples
- **Sprint Review**: Research comprehensiveness assessed
- **Retrospective**: Identified gaps for subsequent sprints

#### Sprint 36: Research Phase - Character and Narrator (Week 2)
- **Sprint Goal**: Develop voice and dialogue strategies
- **Tasks**: Character voice analysis, narrator development, dialogue in meter
- **Deliverables**: Character voice profiles, dialogue technique guides
- **Definition of Done**: Voice frameworks ready for application

#### Sprint 37: Research Phase - Culture and Tools (Week 3)
- **Sprint Goal**: Complete cultural adaptation strategy and identify tools
- **Tasks**: Moscow vs. Verona analysis, Orthodox Christianity context, rhyme dictionary identification
- **Deliverables**: Cultural adaptation guide, tools and resources document
- **Definition of Done**: All research complete, ready for framework development

#### Sprint 38: Framework Development and QA (Week 4)
- **Sprint Goal**: Create compositional support materials for all 400 stanzas
- **Tasks**: 82 framework file creation tasks
- **Deliverables**: 90,000+ line framework corpus (vocabulary, rhymes, emotional beats)
- **Definition of Done**: All frameworks marked ready for composition
- **Sprint Review**: Quality audit conducted
- **Retrospective**: **Critical discovery** - many frameworks inadequate (led to Sprint 39 Phase 1B)

#### Sprint 39: Critical Enhancement and Composition (Week 5)
- **Sprint Goal**: Deliver complete 400-stanza composed novel
- **Phase 1**: Pre-composition enhancements (4 tasks)
- **Phase 1B**: Critical issue resolution (2 tasks - added post-audit)
- **Phase 2**: Novel composition (8 parallel tasks)
- **Phase 3**: Final QA (deferred to user)
- **Definition of Done**: All 400 stanzas composed, technically compliant, ready for native speaker polish
- **Sprint Review**: Delivery summary created
- **Retrospective**: (This paper)

### 3.3 Task Management (Kanban)

**Kanban Board Structure**:
```
TODO → IN PROGRESS → REVIEW → DONE
```

**WIP Limits**:
- Maximum 1 task in progress per agent at any time (enforced via todo tracking)
- Human oversight prevents task accumulation

**Task Breakdown Example** (Sprint 39, Task 05):
```
Task: Compose Chapter 1 (55 stanzas)
Parent Epic: Novel Composition
Subtasks:
  - Read task specifications
  - Read all framework files
  - Compose stanzas 1-10 (narrative)
  - Compose stanzas 11-20 (character intro)
  - Compose stanzas 21-30 (plot development)
  - Compose stanzas 31-40 (digressions)
  - Compose stanzas 41-50 (rising action)
  - Compose stanzas 51-55 (ball announcement)
  - Technical verification (meter, rhyme)
  - Voice verification (narrator consistency)
  - Quality report generation
Acceptance Criteria:
  - 55 stanzas delivered
  - All technically compliant (aBaBccDDeFFeGG)
  - Framework materials utilized
  - QA report included
Dependencies:
  - Blocked by: Phase 1B completion
  - Blocks: Chapter 2 composition
```

**Flow Optimization**:
- Phase 2 designed for parallel execution (8 tasks simultaneously)
- Critical path identified (climax enhancement must complete before composition)
- Bottlenecks addressed (Phase 1B emergency tasks added)

### 3.4 Test-Driven Development Adaptation

**Traditional TDD**:
```python
# Red: Write failing test
def test_prime_number():
    assert is_prime(7) == True
    assert is_prime(10) == False

# Green: Write minimal code
def is_prime(n):
    if n < 2: return False
    for i in range(2, n):
        if n % i == 0: return False
    return True

# Refactor: Optimize
def is_prime(n):
    if n < 2: return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0: return False
    return True
```

**Our Literary TDD Adaptation**:
```
# Red: Specify requirements before composition
Framework File for Stanza 1:
  - Must establish narrator voice (ironic, philosophical)
  - Must introduce Moscow setting
  - Must hint at tragedy to come
  - Technical: 14 lines, aBaBccDDeFFeGG, iambic tetrameter
  - Line 8: mandatory stress on syllable 8
  - Forbidden: No verb rhymes

# Green: Compose stanza meeting specifications
[Compose Stanza 1 using framework]

# Refactor: Polish while maintaining requirements
[Read aloud, smooth phrasing, strengthen rhymes]

# Test: Verify against requirements
✓ Narrator voice: Ironic, philosophical
✓ Moscow setting: Established
✓ Foreshadowing: Present
✓ Technical: 14 lines, rhyme scheme correct
✓ Line 8: Syllable 8 stressed
✓ Forbidden rhymes: None detected
```

**Quality Gates** (Before progression):
- ✅ Technical specifications met
- ✅ Voice consistency verified
- ✅ Content requirements satisfied
- ✅ No forbidden elements present
- ✅ Read-aloud test passed

### 3.5 Pair Programming: Human-LLM Model

**Roles**:

**Human (Navigator)**:
- Defines overall strategy and goals
- Creates sprint plans and task specifications
- Provides creative direction
- Reviews LLM output critically
- Makes final quality judgments
- Handles subjective aesthetic decisions

**LLM (Driver)**:
- Executes defined tasks systematically
- Generates research syntheses
- Creates framework structures
- Composes verse drafts using frameworks
- Performs technical verifications
- Documents process and decisions

**Communication Protocol**:
- Human provides explicit instructions via prompts
- LLM responds with work products and completion reports
- Continuous feedback loop (human reviews, LLM adjusts)
- Role boundaries explicit (LLM acknowledges limitations)

**Session Example** (Sprint 39, Task 15):
```
Human: "Complete Lark & Nightingale framework from 400 → 700-1,000+ lines.
        Add 7 remaining components: emotional beats, dialogue framework,
        technical support, atmosphere, guidance, checklist, integration."

LLM: [Executes task, generates 2,895 lines]

LLM Report: "Framework complete. Statistics: 2,895 lines,
             200+ vocab entries, 100+ rhyme pairs, 8 emotional beats,
             3 dialogue options. Quality: A+ gold standard."
```