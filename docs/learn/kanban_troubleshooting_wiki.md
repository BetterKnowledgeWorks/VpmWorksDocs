# Kanban Troubleshooting & FAQ

## Common Issues and Solutions

### Work-in-Progress (WIP) Management

**Problem: Team consistently exceeds WIP limits**
- **Causes**: Unrealistic limits, lack of understanding, external pressure
- **Solutions**: 
  - Review and adjust WIP limits based on actual capacity
  - Provide team training on WIP limit benefits
  - Address external pressure sources with stakeholders
  - Use visual indicators (red cards, alerts) when limits are approached

**Problem: Work items get stuck in columns**
- **Causes**: Blockers, unclear acceptance criteria, skill gaps
- **Solutions**: 
  - Implement daily standup blocker discussions
  - Create clear definition of done for each column
  - Cross-train team members to reduce bottlenecks
  - Use blocker tracking and escalation processes

### Flow and Cycle Time Issues

**Problem: Long cycle times**
- **Causes**: Large work items, frequent context switching, bottlenecks
- **Solutions**: 
  - Break down large items into smaller, manageable pieces
  - Implement WIP limits to reduce multitasking
  - Identify and address bottlenecks through flow analysis
  - Standardize work item sizes where possible

**Problem: Unpredictable delivery times**
- **Causes**: Varying work complexity, unclear requirements, external dependencies
- **Solutions**: 
  - Implement work item sizing and estimation
  - Improve requirement gathering and analysis
  - Track and manage external dependencies proactively
  - Use probabilistic forecasting based on historical data

### Team Collaboration Challenges

**Problem: Poor communication and coordination**
- **Causes**: Remote work, unclear roles, insufficient meetings
- **Solutions**: 
  - Implement regular standup meetings focused on flow
  - Use collaborative digital boards for remote teams
  - Define clear roles and responsibilities
  - Establish communication protocols and channels

**Problem: Resistance to Kanban adoption**
- **Causes**: Change resistance, misunderstanding benefits, poor implementation
- **Solutions**: 
  - Start with current process and evolve gradually
  - Provide education on Kanban principles and benefits
  - Involve team in board design and rule creation
  - Celebrate early wins and improvements

## Frequently Asked Questions

### Getting Started

**Q: How do I know if Kanban is right for my team?**
A: Kanban works well for teams that:
- Handle ongoing operational work or support requests
- Need flexibility to respond to changing priorities
- Want to improve flow and reduce cycle times
- Prefer evolutionary change over revolutionary transformation
- Work with varying types and sizes of requests

**Q: What's the difference between Kanban and Scrum?**
A: Key differences include:
- **Kanban**: Continuous flow, no fixed iterations, pull-based system, evolve existing process
- **Scrum**: Time-boxed sprints, defined ceremonies, commitment-based, prescriptive framework
- Both can be combined (Scrumban) for hybrid approaches

**Q: How many columns should my Kanban board have?**
A: Start with 3-5 columns representing your current workflow:
- Basic: To Do → In Progress → Done
- Extended: Backlog → Analysis → Development → Testing → Done
- Add columns as needed to reflect actual work stages, but avoid over-complication

### Implementation

**Q: How do I set appropriate WIP limits?**
A: Start conservatively:
1. Count current work in progress for each person/stage
2. Set initial limits slightly below current levels
3. Monitor flow and adjust based on observations
4. Typical starting point: 1-2 items per person per column

**Q: Should we estimate work items in Kanban?**
A: Estimation is optional but can be helpful for:
- Forecasting delivery dates
- Identifying unusually large items that should be broken down
- Understanding capacity and planning
- Use simple sizing (S/M/L) rather than complex point systems

**Q: How often should we have meetings in Kanban?**
A: Common cadences:
- **Daily**: Brief standup (5-15 minutes) focused on flow and blockers
- **Weekly**: Replenishment meeting to prioritize new work
- **Bi-weekly/Monthly**: Review and retrospective for continuous improvement
- **As needed**: Risk review, escalation meetings

### Metrics and Improvement

**Q: What metrics should we track?**
A: Focus on flow metrics:
- **Cycle Time**: Time from start to completion
- **Throughput**: Items completed per time period
- **WIP**: Current work in progress vs. limits
- **Blockers**: Frequency and resolution time
- **Quality**: Defect rates, rework frequency

**Q: How do we handle urgent requests?**
A: Establish clear policies:
- Define what constitutes "urgent" with stakeholders
- Create expedite lane with strict entry criteria
- Limit expedite work (e.g., max 1-2 items at a time)
- Track expedite frequency to identify systemic issues
- Consider separate SLA for expedite vs. normal work

**Q: Can we use Kanban for project work?**
A: Yes, with adaptations:
- Break projects into smaller, deliverable work items
- Use portfolio Kanban for project-level visualization
- Track project milestones and dependencies
- Consider hybrid approach with project phases
- Maintain focus on flow rather than project completion dates

### Tools and Technology

**Q: Do we need digital tools for Kanban?**
A: Start with what works for your team:
- **Physical boards**: Great for co-located teams, tactile experience
- **Digital tools**: Essential for remote/distributed teams
- **Hybrid**: Digital for tracking, physical for daily work
- Popular tools: Jira, Trello, Azure DevOps, Kanban Tool, LeanKit

**Q: How do we handle dependencies between teams?**
A: Dependency management strategies:
- Visualize dependencies on boards (using dependency links or swimlanes)
- Establish regular coordination meetings between teams
- Create shared backlogs for cross-team work
- Use portfolio-level Kanban for organizational view
- Track and escalate dependency-related delays

### Scaling and Advanced Topics

**Q: How do we scale Kanban across multiple teams?**
A: Scaling approaches:
- **Portfolio Kanban**: Higher-level view of initiatives and projects
- **Program Kanban**: Coordinate related teams working on same product
- **Service-oriented**: Each team manages their service delivery
- **Flight levels**: Strategic, tactical, and operational Kanban systems
- Maintain team autonomy while enabling coordination

**Q: Can we combine Kanban with other frameworks?**
A: Yes, common combinations:
- **Scrumban**: Scrum ceremonies with Kanban flow
- **SAFe**: Scaled Agile Framework incorporating Kanban
- **DevOps**: Kanban for continuous delivery pipelines
- **Lean Startup**: Kanban for feature experimentation
- **Design Thinking**: Kanban for design process flow

## Troubleshooting Checklist

When Kanban isn't working well, check:

### Board Design
- [ ] Columns reflect actual workflow stages
- [ ] WIP limits are realistic and enforced
- [ ] Work items are appropriately sized
- [ ] Board is visible and accessible to all team members

### Team Practices
- [ ] Regular standup meetings focused on flow
- [ ] Blockers are identified and escalated quickly
- [ ] Team pulls work rather than having it pushed
- [ ] Policies and definitions are clear and followed

### Metrics and Feedback
- [ ] Flow metrics are tracked and reviewed
- [ ] Regular retrospectives for continuous improvement
- [ ] Stakeholder feedback is incorporated
- [ ] System performance trends are monitored

### Organizational Support
- [ ] Management understands and supports Kanban principles
- [ ] External dependencies are managed proactively
- [ ] Team has authority to manage their workflow
- [ ] Resources and training are available when needed

## Getting Help

### Internal Resources
- Facilitate team retrospectives to identify specific issues
- Engage with other teams using Kanban for lessons learned
- Involve management in removing organizational impediments
- Create communities of practice for knowledge sharing

### External Resources
- **Books**: "Kanban" by David Anderson, "Essential Kanban Condensed" by David Anderson and Andy Carmichael
- **Online Communities**: Kanban University, Lean Kanban Community
- **Training**: Kanban System Design (KSD), Kanban Systems Improvement (KSI)
- **Consultants**: Consider expert help for complex implementations or organizational resistance

### Red Flags - When to Seek Additional Help
- Cycle times consistently increasing over time
- Team stress and burnout increasing
- Stakeholder satisfaction declining
- Resistance to improvement suggestions
- Inability to identify or resolve systemic issues
- Organizational impediments blocking progress

Remember: Kanban is about evolutionary improvement. Small, consistent changes often yield better results than dramatic overhauls.