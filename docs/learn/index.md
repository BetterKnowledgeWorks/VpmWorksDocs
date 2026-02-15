# VpmWorks Wiki Site

## Overview

### Why Visual Project Management (VPM)?

Most companies deliver only **30%** of their new product projects on time. The common belief is that projects go wrong somewhere along the way — but the truth is, most start wrong.

Outdated planning methods, weak customer engagement, lack of team buy-in, and poor communication set the stage for failure before work even begins. 

**Visual Project Management (VPM)** fixes this by:

- Building teams that are capable *and* accountable  
- Visualizing progress daily to expose issues in real time  
- Driving rapid, team-based responses to delays and information gaps  

With VPM, it’s common to see on-time delivery rates jump from **30% to 85%** — along with higher quality, more satisfied customers, and deeper developer engagement.

### [Theory of Operation](TheoryofOperation)
The **Theory of Operation** outlines the core principles behind how VpmWorks™ helps teams manage complex, multi-function projects. It focuses on synchronizing efforts across separated functions, enabling hybrid project structures, and reducing waste caused by handoffs and unexpected changes. Central to the method are visual tools like the **Project Scoreboard** and **Team Planning** to align contributors and track progress. Key concepts include managing **predecessors and successors**, understanding **focal project types and sizes**, and clearly defining **resource classifications** such as project managers, swim lane owners, extended team members, leadership, and third parties.

### History of VPM
#### Gantt Charts
Gantt charts have long been the go-to tool for visualizing project schedules, tracing their roots back to the early 1900s. They present a timeline view of tasks, clearly showing start and end dates, durations, and dependencies in a horizontal bar format. Gantt charts brought structure and predictability to project planning, and their popularity has been reinforced by the widespread support in tools like Microsoft Project, Smartsheet, and dozens of other project management platforms. This deep integration across enterprise tools has made Gantt charts a default standard—easy to adopt, easy to share, and deeply embedded in how organizations think about schedules.

But despite their strengths, Gantt charts often contribute to late projects. One key issue is that they treat all tasks equally, with each assigned a single line regardless of its complexity or criticality. A minor administrative task receives the same visual weight as a major cross-functional handoff. This flattens the view and dilutes attention from the workflows that truly drive progress. Moreover, the sheer number of tasks—often in the hundreds—creates a dense web of interconnections that spans many pages, making it hard to see what matters most. As a result, teams lose sight of the critical path and struggle to coordinate major transitions. Plan changes are painful to implement, and the complexity makes forecasting unreliable—contributing to the industry’s disappointing record of on-time delivery, with success rates often below 30%.

In Visual Project Management (VPM), we build directly on the legacy of the Gantt chart by keeping its greatest strength: a calendared, visual representation of project timing. We retain the clarity of seeing when things happen and how they align across time—but we eliminate the clutter. Rather than trying to map every small task, VPM focuses on a streamlined view that shows only the most critical elements of the project. These include major deliverables and key handoffs between functions, which are displayed visually to help the team track progress and risk in real time. The timeline remains central, but it is cleaner, more readable, and far more actionable.

Rather than listing hundreds of tasks, VPM forces the team to concentrate on the most important ones—those that generate tangible deliverables and those that represent handoffs between functions. We distinguish between in-function tasks, which stay within a department, and cross-functional tasks, where the work moves between groups like engineering, operations, and marketing. Our emphasis will be on these cross-functional transitions, as they often create the greatest risk and delay. This sharper lens makes the critical path more visible and actionable. 

#### Gantt Dependencies:  Brittle depdendency networks where a flexible RACI architechture is more effective

**The Problem With Gantt Dependencies**

If you've managed a development project with a Gantt chart, you know the pattern: You spend weeks building a detailed project plan with hundreds of task dependencies. Within three months, it's out of date. Requirements change, technical challenges emerge, resources shift—and your carefully crafted dependency network becomes so fragile that updating it is more work than abandoning it.

**The data:** In our work with dozens of development organizations, projects managed with traditional Gantt charts deliver on time less than 25% of the time. Virtually every Gantt chart more than 12 weeks old is obsolete.

**This isn't a user problem—it's a tool problem.**

Gantt charts were designed in the 1950s for construction: fixed scope, sequential work, minimal iteration. Development projects are the opposite: requirements evolve, teams work in parallel, learning is continuous. The tool doesn't match the work.

**The fundamental flaw:** Gantt dependencies treat all relationships the same. "QA reviews Engineering's draft specification" gets the same dependency arrow as "Engineering delivers firmware to Operations for testing." One is internal coordination. The other is a critical cross-team handoff. Gantt can't tell the difference, so you end up with 200+ dependencies when the project really has 12-15 critical interfaces.

When requirements change (and they will), you face an impossible choice: spend hours rewiring the dependency web, or let the chart go stale. Most teams choose the latter.

**How VPM Changes This: Summary Task Dependencies**

VPM takes a fundamentally different approach based on a simple question: **When does the "Accountable" role shift between teams?**

This comes from the RACI model (Responsible, Accountable, Consulted, Informed):
- **Accountable (A):** The team that owns the deliverable and must sign off
- **Responsible (R):** Teams that do work or provide input

**VPM focuses exclusively on when "A" shifts from one team to another.** These are true handoffs—the moments where one team commits a deliverable and another team takes accountability for the next phase.

**Example: Firmware Development**

**Traditional Gantt shows:**
- Task 47: QA reviews firmware spec → Engineering (dependency)
- Task 48: Manufacturing reviews firmware spec → Engineering (dependency)
- Task 49: Operations reviews firmware spec → Engineering (dependency)
- Task 50: Engineering incorporates feedback → QA review (dependency)
- Task 51: Engineering incorporates feedback → Manufacturing review (dependency)
- Task 52: Run initial firmware tests → Operations (dependency)
- Task 53: Operations validates test environment → Engineering (dependency)

*Result: 7+ dependencies representing coordination and back-and-forth reviews.*

**VPM shows:**
```
Summary Task: "Firmware Test Build Ready"
  Accountable: Engineering
  Successor: "Operations Testing Phase"
  Accountable: Operations
```

*Result: 1 clean handoff representing the commitment.*

**What happened to tasks 47-53?** They still exist as subtasks under "Firmware Test Build Ready" for the Engineering team to manage. But VPM doesn't visualize them because they represent the Engineering team coordinating with others (RACI: "R" roles) while Engineering remains Accountable.

**The key insight:** There may be 20 internal coordination points to get a firmware build ready, but VPM visualizes only the handoff—the moment Engineering commits the build and Operations becomes Accountable for testing it. We trust teams to manage their internal coordination if we keep them focused on their cross-team commitments.

**Why VPM Doesn't Import Dependencies**

When you import from MS Project or a Gantt chart, VPM imports:
- ✓ Task names and structure
- ✓ Dates (as reference points)
- ✓ Function assignments
- ✗ **Dependencies (you'll redesign these)**

**Why strip the dependencies?**

Because Gantt dependencies mix true handoffs with internal coordination and create structures too fragile to maintain. VPM asks you to redesign your project around 12-15 clean deliverable interfaces between teams, not 200+ task-level dependencies.

**The investment:** 2-4 hours using VPM's import wizard to identify your critical cross-team handoffs.

**The payoff:** When requirements change (and they will), you update deliverable dates on Summary Tasks, not rewire a web of 200 dependencies. Your project plan stays current instead of becoming obsolete.

**Two Tools, Two Purposes**

VPM doesn't replace your detailed Gantt chart—it complements it:

**Gantt (MS Project):** Detailed task scheduling, critical path analysis, resource leveling, day-to-day execution
- **Users:** Project team, task owners
- **Update frequency:** Daily/weekly
- **Focus:** "What's the next task?"

**VPM:** Cross-functional commitments, interface management, executive visibility
- **Users:** Leadership, cross-functional teams, stakeholders
- **Update frequency:** Weekly/monthly
- **Focus:** "When does each team deliver to other teams?"

**The Bottom Line**

Development projects need flexibility to respond to change. Gantt's 200+ dependencies create rigidity. VPM's 12-15 interface commitments create clarity while allowing teams autonomy to manage their internal work.

**We don't import Gantt dependencies because they're part of the problem we're solving.**

When you import your project into VPM, you're not migrating a mess—you're redesigning your project around clean handoffs. It's more work upfront, but it's the only project plan that will still be accurate three months from now.

#### Critical Path Management 
To improve focus within Gantt charts, project managers often augment them with a Critical Path analysis—a powerful enhancement that highlights the sequence of tasks that directly determine the project’s duration. By identifying which tasks cannot slip without delaying the entire project, Critical Path Management (CPM) brings clarity to complex plans and helps teams prioritize effort and attention. This advancement was so impactful that it became a discipline in its own right, with CPM now a cornerstone of traditional project management. By pulling the critical tasks to the foreground, teams can track the real drivers of schedule performance and manage risk more proactively.

Still, CPM doesn't fully resolve the underlying challenges. First, finding the critical path among hundreds of interdependent tasks is complex, and often the path identified early is just a best guess—it shifts as the project unfolds. Unfortunately, these shifts often become visible only after delays start to accumulate. Adapting to changing critical paths mid-project requires substantial rework, and with large Gantt charts, that means navigating a maze of dependencies. The second issue is unpredictability: even a well-crafted plan can be upended by unexpected events—like a supplier delay due to a factory accident. These kinds of disruptions can't be forecasted and demand agile responses. But Gantt-based systems, with their dense networks and rigid structures, are inherently slow to adapt. This mismatch between complexity and agility limits the effectiveness of both Gantt and CPM in dynamic, fast-moving projects.

In Visual Project Management (VPM), we embrace the value of Critical Path thinking and build directly on the foundation laid by Gantt and CPM. But we sharpen its effectiveness by recognizing that critical paths are not fixed. VPM moves beyond the idea of a single critical path. In real projects, multiple workflows often have the potential to become critical, and our method supports tracking several likely candidates from the start. Maybe one path is 60% likely to drive the schedule—but others, with 15% or 20% probability, still pose serious risk. By identifying and monitoring these paths, we treat critical path prediction as a non-deterministic forecast, not a one-time decision. This prepares teams to adjust more quickly when the unexpected happens, enhancing agility throughout the project. In this way, VPM retains the strengths of Gantt and CPM, while solving many of their long-standing weaknesses.

#### Critcal Chain Project Management  
Critical Chain Project Management (CCPM), developed by Eliyahu Goldratt, represents a major evolution in traditional planning methods. CCPM builds on critical path principles by sharpening the focus on essential tasks and protecting the project timeline with time buffers—both at the end of the chain and at key junctions between task sequences. These buffers absorb variability and make schedules more resilient to disruption. A major innovation is the fever chart, a visual tool that tracks buffer consumption over time and helps teams recognize when a project is slipping before it’s too late. CCPM also introduces the concept of reflection—quantifying every issue by its impact on time. For example, if a design flaw will delay quality testing by six weeks, that delay becomes the unit of analysis. Since time is the bottleneck in most projects, CCPM treats it as the common denominator for all risk and decisions, aligning everyone around schedule impact.

Despite its strengths, CCPM has limitations. It still assumes a single dominant critical chain, which can oversimplify the reality of complex, uncertain projects where multiple paths have the potential to drive the timeline. The model also tends to focus on resource-level task assignments rather than visualizing clear ownership across functions, which makes coordination difficult—especially in cross-functional handoffs that often introduce the greatest risk. These transitions are not treated as special or high-priority in CCPM, limiting visibility into workflow alignment. Furthermore, the structured and analytical nature of CCPM can feel rigid. The formalism and terminology—buffers, chains, fever charts—create a steep learning curve that can alienate teams unfamiliar with the Theory of Constraints. And when the plan feels fixed, teams may hesitate to step back, rethink the structure, or act with agility. These gaps open the door for a new approach—one that keeps the strengths of CCPM but reorients project visibility, flexibility, and ownership for modern teams.

#### Agile
Agile project management emerged from the world of software development as a response to the rigidity of traditional methods like CPM and CCPM. It emphasizes collaboration, fast feedback, and iterative progress. Agile teams plan in short bursts—called sprints—and hold daily stand-up meetings to assess progress and adjust course. A core goal is to get working product into users’ hands as quickly as possible so feedback can shape development early, before big investments are made. Agile also encourages parallel thinking by reducing the hard dependencies that define critical path-based approaches. In fact, Agile often refers to CPM-style planning as waterfall—a term that’s become pejorative, suggesting inflexible, overly linear workflows that fail to adapt. In contrast, Agile champions flexibility and empowers teams to self-organize and adjust continuously.

But this strength in agility can also become a weakness—especially in complex, cross-functional projects. Agile methods often deprioritize the calendar, making it hard to predict when intermediate milestones will be met. When work runs long, it’s simply pushed to the next sprint, which may be fine within a software team but creates serious issues when another function is waiting. For example, if firmware needed for compliance testing isn’t complete, hardware development stalls. This looseness in connecting tasks to calendar days makes it difficult to synchronize across departments. Hand-offs become unpredictable, and integrated planning breaks down. VPM addresses this gap by recognizing that software teams will naturally operate using Agile Scrum for their own planning and execution—but cross-functional coordination happens in a different language. VPM provides that language. It centers on handoff timing—ensuring that when one function needs output from another, the date is visible, tracked, and honored. So while software teams may speak “Agile” inside the sprint, the broader project speaks “VPM”—the language of inter-functional synchronization.

#### Swim Lane Visualization
One of the key innovations in Visual Project Management (VPM) is the use of swim lanes—horizontal bands that group all tasks from a single function into one continuous row stretching across the calendar. Unlike traditional Gantt charts, where tasks are listed line by line regardless of role, swim lanes organize work visually by function, making cross-functional coordination far more intuitive. Each swim lane focuses on the tasks that matter most for coordination: handoffs and key deliverables. For complex functions like engineering or software development, it’s understood that detailed, intra-functional planning still occurs—using Gantt charts, Agile Scrum boards, or other discipline-specific methods. But within the VPM, only the tasks that interact with other teams are shown. This ensures clarity, accountability, and visibility for cross-functional flow without getting lost in the weeds of daily team execution.

Visually, VPM swim lanes resemble Gantt charts in that they use a calendar across the top and represent task durations with horizontal bars. But the similarities end there. While Gantt charts allocate a full line to every task—resulting in plans filled with white space and complex dependency arrows—VPM condenses all of a function’s work into a single lane. That lane may contain 50 to 70 tasks in a long project, and yet still occupy the vertical space of just a few Gantt lines. This dramatically increases the visual density of the chart—often 5 to 10 times more information per page. As a result, large portions of a project—or even an entire program—can be viewed at once. This bird’s-eye view doesn’t just reduce clutter; it fuels insight. When more of the project is visible, it becomes easier to spot misalignments, gaps, and structural issues early, while there’s still time to act. Swim lanes make complex work simpler to see, and that clarity creates a powerful foundation for better decision-making.

### VPM Theory of Operation
Visual Project Management (VPM) operates on a clear principle: teams deliver results when they are aligned around who owes what to whom, and by when. VPM visualizes cross-functional handoffs and key deliverables on a shared calendar using function-based swim lanes, while allowing each function to manage its internal work with the tools best suited to their discipline—whether Agile, Gantt, or another method. This separation of functions enables hybrid projects to operate smoothly, preserving local control while supporting global coordination. VPM charts act as a shared project scoreboard, allowing all roles—project managers, swim lane owners, extended team members, leadership, and even third parties—to track progress and see upcoming responsibilities. Team planning is collaborative, with a focus on identifying predecessors, successors, and timing dependencies to avoid the delays and rework caused by missed handoffs. By simplifying complexity into a single, high-density visual plan, VPM creates the clarity needed to synchronize large, multi-function projects and adapt quickly as priorities shift.  [VPM Theory of Operation](TheoryOfOperation)

### Using Kanban to Complement VPM for Smaller Projects
Visual Project Management (VPM) is designed for large-scale efforts—typically from 4 developers over 4 months to teams of 50 working for 3 years. But most development teams also support a steady flow of smaller, faster-moving efforts—what we call sustaining projects—ranging from a day of work by one developer to 4 developers over 4 months. These sustaining projects can number in the hundreds or thousands annually, and if unmanaged, they can disrupt the focus and resources needed for VPM-led initiatives. A customized Kanban board can help teams manage these smaller efforts effectively, working alongside VPM to create a comprehensive project management approach for product development.  Click [Kanban board for smaller projects](kanban_wiki_home) to see more.

### [Swimlane Diagram](swimlanediagram)

### [Role of Critical Path](RoleOfCriticalPath)
-The critical path is the sequence of tasks that determines a project’s minimum duration—any delay on this path delays the entire project. While the critical path sets the schedule and focuses attention, it’s only a hypothesis at the start. In complex projects, multiple near-critical paths often exist and may shift over time. Actively monitoring and updating the critical path gives the most accurate picture of current project risk and timing.

### [Wasteful Automation](WastefulAutomation)

- Many teams are eager to automate project processes—auto-calculated critical paths, automatic emails, self-adjusting schedules. But successful projects require an intelligent eye on every scope change, task expansion, and delay. Without that, automation can quietly lock in decisions that cause failure long after the fact. Click link to see more.

### [Team Selection](TeamSelection)
-Selecting the right team is one of the most critical decisions in any project. Success hinges not just on having smart people involved—but on assembling a group that has all the capabilities needed, and just as importantly, the availability to contribute when it matters most. Too often, projects stall or suffer because key skills are missing or team members are stretched too thin.

To keep the team focused and efficient, we organize it into two levels:

The core team is small, dedicated, and deeply involved in the day-to-day work and decision-making. These are the people who attend all key meetings and own major deliverables.

The extended team includes subject matter experts, support functions, and other contributors who may not be full-time but are vital for specific parts of the project. They’re pulled in as needed.

This structure keeps communication crisp and allows the core team to move quickly—while still ensuring the full breadth of expertise is available to the project.

### [VPM Stand-Up Meetings](VpmStandUpMeetings)
-VPM stand-up meetings are short, focused sessions designed to maintain momentum, surface issues early, and keep teams aligned. Like Agile daily stand-ups, they’re fast-paced (usually 15 minutes or less), happen at a regular time, and are intended to be lightweight. The key difference lies in the visual context—VPM stand-ups happen in front of a shared project visualization, such as a wallboard, whiteboard, or digital canvas that reflects current project status.

### Two Paths to Better Problem Solving

VpmWorks™ includes two proven approaches to problem solving—each designed to help teams move **together** toward better understanding. These methods are not just about generating solutions—they're about building **shared clarity**. You'll notice that 90% of the effort is spent defining the problem. Why? Because once everyone sees the issue the same way, the right solutions are usually obvious. Without that shared view, all you get are scattered opinions and misaligned actions.

This thinking isn't new—it was core to how **Toyota transformed its business** starting in the mid-20th century. Their problem-solving methods weren’t just tools—they were cultural cornerstones that taught teams to slow down, ask the right questions, and fix the process instead of blaming the people. We're carrying that legacy forward at VpmWorks, making it accessible, visual, and easy for modern teams.

- [Toyota A3 Method](ToyotaA3)
- [5 Whys](FiveWhys)

### VPM:  a Visual Single Point of Truth
- SPOT
- Courage from Goldratt
- Vary the Process to Fit the Project
- Aspire to Display Truth

### [Visualization Principles](VisualizationPrinciples)
- Hierarchical over Linear
- Magnify Handoffs
- [Managing Visibility]

### [Multi-Phase and Single-Phase Projects](MultiVsSinglePhaseProjects)
- In Visual Project Management (VPM), a project phase typically spans 3 to 6 months—long enough to achieve meaningful progress, yet short enough to maintain a strong sense of urgency where each week (and ideally each day) matters. VPM is designed to support both single- and multi-phase projects, though its primary use case is multi-phase initiatives.

### Creating Ownership and Accountability
- The flaw of Project-Manager Planning
- Create a Team Mentality
- People will do more not to let down teammate than the boss -attribution-
- Create Accountability at Planning; Nurture at Daily Stand-ups

### Agile, Waterfall, and VPM

### Central Role of Planning Event

### Phase-Gate Systems and Quality Management Systems (QMS)

## Adopting VPM
- Project Start
- Phase Start
- Mid Phase

## [The VpmWorks Process](VpmWorksProcess)
- Planning Event Preparation
- Planning Event
- Project Execution
- Launch Sustainment

## [Certification](Certification)

## [VPM and Design Thinking](DesignThinking)

