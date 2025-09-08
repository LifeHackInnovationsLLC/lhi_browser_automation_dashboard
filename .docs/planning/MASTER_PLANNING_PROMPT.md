# LHI Browser Automation Dashboard - Master Planning Prompt

## Project Context
We are creating a unified browser automation dashboard that consolidates control of Puppeteer, Playwright, and Kapture MCPs with a consistent Chrome profile management system. This must be built as a modular LHI node module with UI-first development using the LHI UI Framework.

## Critical Requirements
1. **Modularity**: Every component must be reusable and standalone
2. **UI-First**: Start with interface design, add functionality incrementally
3. **Cross-Platform**: Must work on Mac and Linux (via web interface)
4. **LHI Standards**: Follow all LHI module conventions and use existing LHI modules
5. **Documentation**: Comprehensive documentation at every phase

## Multi-Phase Planning Process

### Phase Structure
- **4 Planning Phases**: Research → Architecture → Refinement → Pre-Implementation
- **5 Implementation Phases**: Foundation → Components → Integration → Functionality → Polish
- **Validation Checkpoints**: Between each phase
- **Sub-Agent Coordination**: Parallel and serial task execution

## Sub-Agent Task Assignments

### Phase 1: Research & Documentation Retrieval (4 Parallel Agents)

#### Agent 1: Documentation Retrieval Specialist
**Mission**: Gather latest documentation for all dependencies
**Tasks**:
```
1. Retrieve Puppeteer latest documentation
2. Retrieve Playwright latest documentation  
3. Retrieve React 18+ documentation
4. Retrieve Emotion CSS documentation
5. Document MCP protocol specifications
```
**Deliverable**: Complete docs in .docs/dependencies/

#### Agent 2: LHI Infrastructure Analyst
**Mission**: Map existing LHI modules and infrastructure
**Tasks**:
```
1. Analyze lhi_puppeteer_browser structure
2. Document lhi_chrome_profile_utils API
3. Map lhi_ui_framework components
4. Identify Sentinel implementation details
5. List all import patterns and paths
```
**Deliverable**: current_state.md in .docs/architecture/

#### Agent 3: Component Inventory Specialist
**Mission**: Catalog all UI components needed
**Tasks**:
```
1. List existing lhi_ui_framework components
2. Identify missing components needed
3. Document component props and usage
4. Map component hierarchy needs
5. Plan new component requirements
```
**Deliverable**: Component inventory and gap analysis

#### Agent 4: Dependency Mapping Specialist
**Mission**: Map all file dependencies and locations
**Tasks**:
```
1. Trace all file imports in lhi_puppeteer_browser
2. Document external script dependencies
3. Map temp file locations
4. Identify config file patterns
5. Document build processes
```
**Deliverable**: Complete dependency map

### Phase 2: Architecture Design (3 Mixed Agents)

#### Agent 1: System Architect
**Mission**: Design the overall system architecture
**Serial Tasks**:
```
1. Create layered architecture diagram
2. Define module boundaries
3. Design data flow patterns
4. Plan state management approach
5. Document API contracts
```

#### Agent 2: Component Designer
**Mission**: Design UI component architecture
**Parallel Tasks**:
```
1. Create component hierarchy
2. Design BrowserCard variants
3. Plan ProfileSelector component
4. Design ScriptLibrary interface
5. Plan RecordingControls layout
```

#### Agent 3: Integration Architect
**Mission**: Plan MCP integration strategy
**Serial Tasks**:
```
1. Design MCP adapter pattern
2. Plan profile management service
3. Design script conversion engine
4. Plan monitoring architecture
5. Document communication patterns
```

### Phase 3: Refinement & Validation (4 Serial Agents)

#### Agent 1: Architecture Reviewer
**Mission**: Validate all architectural decisions
**Questions to Answer**:
```
1. Are there any circular dependencies?
2. Is the module boundary clear?
3. Are all components truly reusable?
4. Is the data flow optimal?
5. Are there any security concerns?
```

#### Agent 2: Compatibility Validator
**Mission**: Ensure cross-platform compatibility
**Validation Tasks**:
```
1. Check Mac Chrome profile paths
2. Verify Linux Chrome profile paths
3. Test import patterns on both OS
4. Validate file system operations
5. Check network/IPC compatibility
```

#### Agent 3: Performance Optimizer
**Mission**: Identify performance optimizations
**Analysis Tasks**:
```
1. Calculate bundle size impact
2. Identify code splitting opportunities
3. Plan lazy loading strategy
4. Optimize real-time updates
5. Plan caching strategy
```

#### Agent 4: Risk Assessor
**Mission**: Document and mitigate risks
**Assessment Tasks**:
```
1. Identify technical risks
2. Document fallback strategies
3. Plan error recovery
4. Create contingency plans
5. Document known limitations
```

### Phase 4: Pre-Implementation Planning (2 Parallel Agents)

#### Agent 1: Implementation Planner
**Mission**: Create detailed implementation plan
**Tasks**:
```
1. Break down into concrete tasks
2. Estimate time for each task
3. Define success criteria
4. Plan testing strategy
5. Create rollback procedures
```

#### Agent 2: UI/UX Designer
**Mission**: Create UI mockups and workflows
**Tasks**:
```
1. Create dashboard wireframes
2. Design component mockups
3. Plan user workflows
4. Design error states
5. Create style guide
```

## Critical Questions Per Phase

### Phase 1 Must-Answer Questions
1. **Version Compatibility**: What versions of React, Emotion, and other deps are we using?
2. **Import Patterns**: How do we handle submodule vs npm imports?
3. **Existing Code**: What can be reused from lhi_puppeteer_browser?
4. **Chrome Profiles**: How does profile selection currently work?
5. **MCP Communication**: How do MCPs communicate with the host?

### Phase 2 Must-Answer Questions
1. **State Management**: Redux, Context, or Zustand?
2. **Component Reusability**: What goes in lhi_ui_framework vs local?
3. **Data Flow**: How does script recording data flow?
4. **Profile Persistence**: How do we store selected profiles?
5. **MCP Abstraction**: How do we normalize MCP differences?

### Phase 3 Must-Answer Questions
1. **Failure Modes**: What happens when an MCP disconnects?
2. **Profile Conflicts**: How do we handle concurrent profile access?
3. **Performance**: What's acceptable latency for updates?
4. **Compatibility**: Any browser-specific limitations?
5. **Security**: How do we protect profile data?

### Phase 4 Must-Answer Questions
1. **MVP Definition**: What's the minimum viable product?
2. **Testing Strategy**: Unit, integration, or E2E tests?
3. **Deployment**: How do we package and distribute?
4. **Migration**: How do existing users migrate?
5. **Documentation**: What documentation is essential?

## Validation Checkpoints

### After Each Phase
1. **Completeness Check**: Are all deliverables complete?
2. **Quality Check**: Does work meet LHI standards?
3. **Integration Check**: Will this integrate with existing tools?
4. **Risk Check**: Any new risks identified?
5. **Proceed/Pivot Decision**: Continue or adjust course?

## Expected Deliverables

### Phase 1 Deliverables
```
.docs/
├── dependencies/
│   ├── puppeteer_docs.md
│   ├── playwright_docs.md
│   ├── react_docs.md
│   ├── emotion_docs.md
│   └── mcp_protocol_docs.md
├── architecture/
│   ├── current_state.md
│   ├── dependency_map.md
│   └── component_inventory.md
└── planning/
    └── gap_analysis.md
```

### Phase 2 Deliverables
```
.docs/architecture/
├── target_architecture.md
├── component_hierarchy.md
├── data_flow_diagrams.md
├── state_management_plan.md
└── module_boundaries.md
```

### Phase 3 Deliverables
```
.docs/planning/
├── risk_assessment.md
├── compatibility_matrix.md
├── performance_benchmarks.md
├── optimization_plan.md
└── final_architecture.md
```

### Phase 4 Deliverables
```
.docs/
├── implementation_roadmap.md
├── ui_mockups/
├── testing_strategy.md
└── deployment_plan.md
```

## Success Criteria

### Planning Success
- [ ] All documentation retrieved and current
- [ ] Architecture validated by multiple agents
- [ ] No unresolved technical risks
- [ ] Clear implementation path defined
- [ ] UI mockups approved

### Implementation Success
- [ ] UI loads in <2 seconds
- [ ] Profile selection works across all MCPs
- [ ] Scripts convert with 90%+ accuracy
- [ ] No conflicts with existing tools
- [ ] Works identically on Mac/Linux

## Agent Coordination Rules

### Parallel Execution
- Use for independent research tasks
- Use for documentation retrieval
- Use for component design variants
- Report results to central planning doc

### Serial Execution
- Use for dependent architectural decisions
- Use for validation and review
- Use for risk assessment
- Use for final planning steps

### Communication Protocol
1. Each agent updates their section in PLANNING.md
2. Flag blockers immediately in TASK.md
3. Document decisions with justification
4. Cross-reference related work
5. Maintain running notes of findings

## Iterative Refinement Process

### At Each Phase Transition
1. **Review**: What did we learn?
2. **Refine**: What needs adjustment?
3. **Validate**: Are we still on track?
4. **Document**: Update all planning docs
5. **Proceed**: Get approval to continue

### Continuous Improvement
- Each phase builds on previous findings
- Assumptions are constantly challenged
- Documentation is living and updated
- Feedback loops are built in
- Course corrections are expected

---

*This prompt should be used to coordinate all planning phase agents*  
*Each agent should reference this document for their specific tasks*  
*Updates to this prompt require team synchronization*