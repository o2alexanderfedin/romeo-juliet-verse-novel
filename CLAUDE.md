# Claude Code Guidelines for Literature Project

## Task Execution Strategy

### Context Optimization
Extensively use tasks and subtasks (Task tool) to optimize the context usage.

### Parallel Execution
Extensively use parallel tasks and subtasks (multiple Task tools running in the same message) to make the work be done much faster.

### Map-Reduce Approach
Use map-reduce approach with parallel tasks and subtasks.

### Task Reporting
Ensure each task or subtask reports back a very brief explanation on what was done, and what still needs to be done (if any).

### Problem Resolution
Ensure that in case of any problem that task or subtask experiences, it **must** spawn another [set of] subtask(s) to do necessary research and/or experiments in order to resolve the issue.

### Planning and Tracking
Extensively use planning (with TodoWrite tool), so all work is being thoroughly and reliably tracked, and nothing is skipped or lost.

### Parallelization Limits
The maximum number of tasks or subtasks running in parallel should not be more than CPU cores on this machine.

## Software Engineering Principles

### SOLID Principles
You must religiously follow SOLID principles:
- **S**ingle Responsibility Principle
- **O**pen/Closed Principle
- **L**iskov Substitution Principle
- **I**nterface Segregation Principle
- **D**ependency Inversion Principle

### Additional Principles
- **KISS** (Keep It Simple, Stupid)
- **DRY** (Don't Repeat Yourself)
- **YAGNI** (You Aren't Gonna Need It)
- **TRIZ** (Theory of Inventive Problem Solving)

## Development Process

### Test-Driven Development (TDD)
You must religiously follow TDD (Test-Driven Development) process:
1. Write failing test first
2. Write minimal code to pass
3. Refactor while keeping tests green

### Testing Requirements
You must create both unit tests and integration tests.

### Type Safety
You must do the code as strongly-typed as possible, and even more, so we can find errors **before** we run code in production.

### Linting
You **must** extensively and exhaustively run applicable linters every time before sending code to github.

### Code Review
You must review the changes made with a separate subtask.

## Git Workflow

### Git Flow
You **must** use git flow for all git/github-related actions (if applicable).

### No Pull Requests
No Pull Requests - I am solo here.

### Commit and Push
You **must** commit and push code every time when you are done with any engineering task.

### Releases
You **must** do git release after each significant feature or piece is implemented.

---

## Literature Project: Resource Index

### Master Index Files

The Literature project has comprehensive research documentation for Russian poetry and verse novel composition. **Always consult these indexes before starting any poetry composition work.**

#### 📚 Primary Index: [`INDEX_MASTER.md`](INDEX_MASTER.md)
**USE THIS FIRST** - Comprehensive navigation guide for all research materials.

Contains:
- **Quick Reference section** - Fast lookup during composition (rhyme types, Onegin stanza, Pushkin style, rhyme dictionaries)
- **Complete Research Documents** - All 10 major research guides with summaries
- **Quick Lookup by Topic** - Tables organized by technical specs, narrative techniques, structure, culture, tools
- **Examples and Models** - What to study (Eugene Onegin, Romeo & Juliet, Pushkin's lyrics)
- **Cross-Reference by Use Case** - Organized by workflow ("I'm about to write a stanza", "I'm writing dialogue", etc.)
- **Workflow Recommendations** - Pre-writing, during writing, revision, chapter completion phases
- **Document Statistics** - Size and focus of each research document (~250K+ words total)

#### ⚡ Technical Quick Reference: [`INDEX_TECHNICAL_QUICK_REFERENCE.md`](INDEX_TECHNICAL_QUICK_REFERENCE.md)
**USE THIS DURING COMPOSITION** - Ultra-fast lookup for technical specifications.

Contains:
- **Onegin Stanza Quick Specs** - Complete 14-line pattern with rhyme scheme aBaBccDDeFFeGG
- **Iambic Tetrameter Checklist** - Meter verification with mandatory rules
- **FORBIDDEN RHYMES** - What to avoid (verb rhymes, grammatical rhymes, trite pairs)
- **GOOD RHYME PRACTICES** - Rich rhymes, deep rhymes, exact rhymes, mixed parts of speech
- **Russian Stress Rules** - Verification requirements (stress cannot be predicted!)
- **Character Voice Quick Reference** - Profiles for Romeo, Juliet, Mercutio, Nurse, Friar
- **Dialogue Quick Tips** - Stichomythia, extended speech, mixed with narration patterns
- **Pacing Quick Guide** - Fast vs. slow pacing techniques
- **Stanza Functions** - Types: narrative, lyrical, digressive, dialogue, transitional
- **Verification Checklist** - Use before finalizing each stanza (meter, rhyme, voice, content)
- **Resource Quick Links** - Rifmovnik.ru, stress dictionaries, Pushkin concordance
- **Common Problems & Solutions** - Troubleshooting guide
- **Quick Tips** - Before/during/after stanza composition

### Research Documents Organization

All research is organized in structured directories:

```
Literature/
├── INDEX_MASTER.md                    ← START HERE for navigation
├── INDEX_TECHNICAL_QUICK_REFERENCE.md ← Use during composition
├── CLAUDE.md                          ← This file
│
├── authors/russian/                   ← Russian poetry fundamentals
│   ├── pushkin_alexander/research/
│   │   └── poetry_style_analysis.md        (947 lines - Pushkin's style)
│   └── technical_analysis/versification/
│       └── russian_rhyme_and_meter_guide.md (947 lines - rhyme/meter system)
│
└── projects/romeo_and_juliet_verse_novel/research/
    ├── preparation_requirements_analysis.md  (1,599 lines - project overview)
    │
    ├── target_form/
    │   └── eugene_onegin_deep_analysis.md    (~54K words - primary model)
    │
    ├── technical_craft/
    │   ├── russian_prosody_complete_guide.md (~15K words - technical deep dive)
    │   └── verse_novel_craft_guide.md        (~8.5K words - form techniques)
    │
    ├── character_dialogue/
    │   └── character_dialogue_techniques.md  (~50K words - character methods)
    │
    ├── narrative_voice/
    │   └── narrator_creation_guide.md        (~56K words - voice development)
    │
    ├── cultural_adaptation/
    │   └── cultural_contexts_guide.md        (~40 pages - adaptation strategy)
    │
    └── resources/
        └── tools_and_resources_guide.md      (~90 pages - practical tools)
```

### Critical Rules for Poetry Composition

**ALWAYS verify these before finalizing any stanza:**

1. **Russian Stress Patterns**
   - NEVER guess stress - Russian stress is unpredictable
   - Use: Wiktionary, Rifmovnik.ru, Zalizniak's dictionary
   - ё (yo) is ALWAYS stressed (most reliable indicator)

2. **Forbidden Rhymes (Critical!)**
   - ❌ NO verb infinitive rhymes (любить/говорить)
   - ❌ NO verb conjugation rhymes (говорит/звонит)
   - ❌ NO grammatical ending rhymes (too easy/banal)
   - ❌ NO trite pairs (любовь/кровь, розы/морозы)
   - ✅ Prefer rich rhymes (consonants before stress match)
   - ✅ Mix parts of speech (noun with adjective, etc.)

3. **Onegin Stanza Form**
   - 14 lines exactly
   - Rhyme scheme: aBaBccDDeFFeGG (lowercase=feminine, uppercase=masculine)
   - Iambic tetrameter (8 syllables, or 9 for feminine ending)
   - Final stress position MANDATORY (syllable 8)
   - See: INDEX_TECHNICAL_QUICK_REFERENCE.md for complete specs

4. **Voice Consistency**
   - Narrator voice must remain consistent within work
   - Each character must have distinctive voice profile
   - Check character voice matrix in Character/Dialogue guide
   - Verify vocabulary, syntax, imagery, rhythm match character

5. **Quality Standards**
   - Precision and brevity paramount (Pushkin's principle)
   - Every word must earn its place
   - Show through sensory detail, not abstract telling
   - Natural sound within strict form (revision makes it effortless)

### Workflow for Poetry Composition

#### Phase 1: Pre-Writing
1. Review INDEX_TECHNICAL_QUICK_REFERENCE.md
2. Check relevant character voice profiles
3. Review previous stanzas for consistency
4. Open Rifmovnik.ru (https://rifmovnik.ru/) for rhyme search

#### Phase 2: Drafting
1. Keep INDEX_TECHNICAL_QUICK_REFERENCE.md open
2. Count syllables as you write each line
3. Mark stresses immediately (verify with dictionary)
4. Check rhyme scheme matches aBaBccDDeFFeGG
5. Avoid forbidden rhymes (verb rhymes, grammatical rhymes)

#### Phase 3: Verification (Before Finalizing)
Use the Verification Checklist from INDEX_TECHNICAL_QUICK_REFERENCE.md:
- [ ] Meter: 8 syllables (9 for feminine), final stress mandatory, no odd positions stressed
- [ ] Rhyme: Correct scheme, no verb/grammatical rhymes, prefer rich rhymes
- [ ] Voice: Character voice consistent, narrator voice consistent
- [ ] Content: Serves purpose, appropriate pacing, connects to adjacent stanzas

#### Phase 4: Revision
1. Read aloud for natural sound
2. Compare to Eugene Onegin examples
3. Check against Pushkin's style principles
4. Verify cultural appropriateness
5. Polish word choices for precision

### Key Resources During Composition

**When Writing:**
- **Rhyme Dictionary**: Rifmovnik.ru (5.4M Russian words with phonetic search)
- **Stress Verification**: Wiktionary Russian, RussianGram.com
- **Technical Specs**: INDEX_TECHNICAL_QUICK_REFERENCE.md (this file has everything)

**When Stuck:**
- **Problem Solving**: See "Common Problems & Solutions" in INDEX_TECHNICAL_QUICK_REFERENCE.md
- **Examples**: Eugene Onegin Deep Analysis for how Pushkin handled similar situations
- **Character Voice**: Character/Dialogue Techniques guide, Section 2

**For Major Decisions:**
- **Structure**: Eugene Onegin Analysis (chapter organization, pacing)
- **Cultural Elements**: Cultural Contexts Guide (Russian vs. Italian, adaptation theory)
- **Narrator Voice**: Narrator Creation Guide (Pushkin's approach, voice development)

### Important Notes

**Total Research Available**: ~250,000+ words of comprehensive reference material covering:
- Russian prosody and versification (complete technical specifications)
- Pushkin's style and the Onegin stanza form
- Eugene Onegin as verse novel model (54K word analysis)
- Verse novel craft techniques
- Character development and dialogue in verse (50K words)
- Narrator creation and voice development (56K words)
- Cultural contexts (19th c. Russia and Renaissance Italy)
- Practical tools and resources (rhyme dictionaries, stress guides, etc.)

**Remember**:
- The indexes (INDEX_MASTER.md and INDEX_TECHNICAL_QUICK_REFERENCE.md) are your primary navigation tools
- Always verify Russian stress patterns - never guess
- Always check rhyme quality - avoid verb and grammatical rhymes
- Pushkin's genius was making strict form seem effortless through meticulous revision
- Read aloud to test naturalness within meter

---

## Summary

For this Literature project:
1. **Software Engineering Principles** (above) apply to any code/tooling
2. **Poetry Composition** requires consulting the comprehensive research indexes
3. **Always start with INDEX_MASTER.md** for navigation
4. **Keep INDEX_TECHNICAL_QUICK_REFERENCE.md open** during composition
5. **Verify everything** - stress, meter, rhyme, voice consistency
