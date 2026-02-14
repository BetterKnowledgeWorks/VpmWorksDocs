# Board Design and Setup

## Physical vs. Virtual Boards

### Physical Boards: Best For

#### Advantages
- **Always visible** — can't be minimized or forgotten
- **Inviting to collaborators** — people naturally gather around
- **Perfect for co-located teams**
- **Spontaneous problem-solving** — pointing, discussion, quick decisions
- **Psychological impact** — more engaging than digital tools

> *"The physical board had a huge psychological effect compared to anything we got from the electronic tracking tool we used at Microsoft®."* — David Anderson

#### Disadvantages
- Limited to single location
- No automatic tracking/reporting
- Harder to backup or version control
- Remote team members excluded

### Virtual Boards: Best For

<!-- #### Advantages -->
- **Accessible from anywhere**
- **Fair to remote contributors**
- **Easy tracking across time zones**
- **Automatic data capture** for metrics
- **Integration with other tools**

#### Disadvantages  
- Lacks physical "presence"
- Easy to ignore when minimized
- Less spontaneous collaboration
- Can become overly complex

### Decision Matrix

| Team Type | Recommendation | Reason |
|-----------|----------------|--------|
| **Co-located** | Physical | Maximizes visibility and collaboration |
| **Distributed** | Virtual | Ensures equity and access |
| **Hybrid** | Start physical, add virtual | Best of both worlds |

## Standard Board Layouts

![Basic Kanban Board](Art/Kanban/Kanban5--ExampleSimpleKanban.png)

### Basic Flow (Recommended Start)
```
[ Backlog ] → [ Next Up ] → [ In Progress ] → [ Done ]
```

### Enhanced Flow (After Basic Works)
```
[ Backlog ] → [ Prep ] → [ Next Up ] → [ In Progress ] → [ Review ] → [ Done ]
```

## Column Definitions

### Backlog
- **Purpose**: Capture all requested work
- **WIP Limit**: None
- **Commitment**: None — just requests
- **Review Frequency**: Weekly prioritization

### Prep (Optional)
- **Purpose**: Clarify requirements before commitment
- **Activities**: Research, estimation, resource identification
- **WIP Limit**: 2-3 items
- **Output**: Tasks ready for Next Up

### Next Up
- **Purpose**: Committed work ready to start
- **WIP Limit**: 5-8 items (1-2 weeks of work)
- **Selection**: Highest value tasks that fit capacity
- **Review**: Weekly rationalization meeting

### In Progress  
- **Purpose**: Active work being executed
- **WIP Limit**: 3-5 items (strict enforcement)
- **Focus**: Single-tasking, minimize multitasking
- **Movement**: Pull-based only

### Awaiting/Review
- **Purpose**: Completed work pending validation
- **WIP Limit**: No limit (external dependency)
- **Action**: Regular follow-up required
- **Risk**: Work stalling indefinitely

### Release/Acceptance
- **Purpose**: Final customer/stakeholder sign-off
- **WIP Limit**: Monitor closely
- **Success**: Clear acceptance criteria
- **Celebration**: Acknowledge completion

### Done
- **Purpose**: Completed and accepted work
- **Maintenance**: Clear weekly or monthly
- **Value**: Historical record and motivation

## Wait Rows (Blocking Management)

![Expanded Kanban Board](Art/Kanban/Kanban9--ExampleSustainingKanban.png)

### When to Add Wait Rows
- Work frequently gets blocked
- Dependencies on external teams
- Approval processes create delays

### Types of Wait States
- **Waiting on Information**
- **Waiting on Approval**  
- **Waiting on Dependencies**
- **Waiting on Resources**

### Wait Row Benefits
- **Makes blockers obvious**
- **Triggers follow-up actions**
- **Prevents "almost done" black holes**
- **Enables blocking analysis**

## Work-in-Progress (WIP) Limits

### Setting Initial Limits

#### Conservative Approach (Recommended)
- **Next Up**: 1 week of work
- **In Progress**: 1 task per person + 1 buffer
- **Review columns**: No limits initially

#### Calculation Method
```
Team Size × Task Completion Rate × Time Period = WIP Limit

Example: 
3 people × 2 tasks/week × 1 week = 6 tasks in Next Up
3 people × 1 active task + 1 buffer = 4 tasks In Progress
```

### Adjusting Limits Over Time

#### Too High (Symptoms)
- Work sits too long in columns
- Multiple tasks per person
- Reduced focus and quality

#### Too Low (Symptoms)  
- People waiting for work
- Artificial bottlenecks
- Underutilized capacity

#### Right-Sized (Indicators)
- Steady flow through columns
- Minimal multitasking  
- Clear priority focus
- Team not overwhelmed

## Board Metrics Integration

### Visual Indicators on Board

#### Cumulative Flow Diagram
- Create a column for "Done in Month" for each column for the last 12 months so the team can see flow over time.
- Identify trending bottlenecks
- Spot capacity imbalances

#### Cycle Time Tracking
- Start dates on cards
- Completion dates recorded
- Track on-time delivery (to date on card)

#### Results Measurement
- Customer complaints resolved
- Revenue generated
- Cost savings implemented
- Quality issues addressed
- Obsolete parts removed from assemblies

## Kaizen Agenda

### Discovery (Day 1)
1. **Train team** on board usage
2. **Map current workflow** with team
3. **Determine invitatee list**
4. **List typical work types** and sources
5. **Choose physical or virtual platform**

### Design (Day 2--morning)
1. **Create initial column structure**
2. **Determine team meeting cadence, which is usually weekly**
3. **Limit "Next Up" column to about what can be done by the next meeting**
4. **Design card format**

### Phase 3: Launch (Day 2--afternoon)
1. **Populate backlog** with current work
3. **Establish daily** check-in process
4. **Schedule regular meetings** Sent invitations

## Common Design Mistakes

### Over-Engineering Initial Board
- **Problem**: Too many columns and rules from start
- **Solution**: Start simple, add complexity gradually

### Ignoring WIP Limits
- **Problem**: Board becomes fancy to-do list
- **Solution**: Enforce limits on "Up Next" and "In Progress" strictly, adjust if needed

### No Clear Column Definitions
- **Problem**: Work sits in wrong columns
- **Solution**: Write clear definitions, train team

### Missing Blocking States
- **Problem**: Blocked work becomes invisible
- **Solution**: Add wait rows or blocking indicators

---

## Next Steps
- [Sustaining Projects](kanban_sustaining_projects_wiki)
- [Dashboards](kanban_dashboards_wiki)
- [Performance](kanban_performance_wiki)

---

*Good board design balances simplicity with team needs. Start basic, evolve weekly 
based on actual usage patterns.*