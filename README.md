# Phoenix Project
by Gene Kim, Kevin Behr, et al.

## Table of Content
#### Main Concepts
- The 4 Types of Work
- The 3 Ways
- The Theory of Constraints (Dr. Goldratt)
#### Secondary Concepts
- Risk Evaluation
- Total Productive Maintenance
- Idle Time / Slack
- Continuous Improvement
#### Other Referenced Concepts
- 5 Dysfunctions of A Team
- CIA data triangle
- The Five Core Lean Principles
- Value Stream Map (VSM)
- Kaizen
- Order to cash cycle
- Total Productive Maintenance
#### Misc
- Interview Questions for Product Owner
- Common Business Challenges
- Internal hurdle rate for project
- Chief Financial Officer (CFO) Goals
- Question to ask about change, task or projects
- Work Center
- Core Qualities of a Project
- Water spider (factory position)
- Reading List
- Quotes

---
## Main Concepts
Concepts referenced multiple times through the book and extensively expanded upon.

---
### The 4 types of work

1. Business projects: These are business initiatives, of which most Development projects encompass.

2. Internal IT projects (Technical Support):  Infrastructure or IT Operations projects that business projects might create, as well as internally generated improvement projects. Often these are not centrally tracked anywhere, instead residing with the budget owners. This creates a problem when IT Operations is a bottleneck, because there is no easy way to find out who much of capacity is already committed to internal projects.

3. Changes: Generated from the previous two types of work and are typically tracked in a ticketing system.

4. Unplanned work / Firefighting / anti-work: Operational incidents and problems. Always come at the expense of other planned work commitments and moves you away from your goals

“A ‘*change*’ is any activity that is physical, logical, or virtual to applications, databases, operating systems, networks, or hardware that could impact services being delivered.”

---
### The 3 Ways

---
#### TL;DR

**The First Way (Flow of Work):** Focus on the left-to-right flow of work from Development to IT Operations to the end user, emphasizing the importance of reducing bottlenecks, enhancing flow, and achieving fast and reliable delivery.
   
**The Second Way (Feedback Loop):** Prioritize the right-to-left flow of information from IT Operations back to Development, highlighting the need for feedback loops to prevent problems and enable continuous improvement.
   
**The Third Way (Continuous Learning):** Embrace a culture of continual experimentation and learning, fostering a risk-taking mindset and understanding that repetition and practice lead to mastery.

---
#### First Way: Flow of Work

**Objective:** Create a fast and efficient workflow that aligns business processes with customer needs.
##### **Key Principles:**
**Optimize for Global Goals:** Shift focus from local departmental goals to the larger system's success. Think beyond individual metrics like Ops availability and prioritize overall system optimization.

**Identify and Optimize Constraints:**
In most plants, there are a very small number of resources, whether it's men, machine or material, that dictate the output of the entire system. See Theory of constraint. 

- Always search for constraints and verify if they are the true bottlenecks.
- Make sure constraint is at full capacity
- (Drum-Buffer-Rope)
    - **Drum**: Set the production pace based on the constraint's capacity.
    - **Buffer**: Create safety margins to handle disruptions.
    - **Rope**: Control the release of work to maintain smooth flow.

**Building Adaptive Systems:**
- Develop systems and organizations that are safe to change.
- Implement strategies to limit work in process.
- Embrace continuous integration and deployment.
- Create environments on-demand.

**Visualize and Limit Work-in-Progress (WIP):**

**Story Example**: When Bill tried to organize the change process, making his people put their intended changes on index cards and then put the cards on a Kanban board. The cards visualized the work in progress in a way that everyone could see.

- All important activities must go through the task manager software, not by emails, phone calls, or messaging.
- Limiting what gets put in task planner leads to work being completed faster.

> "Taking needless work out of the system is more important than putting more work into it"

Limit how many task can be at any given time in one of the section (todo, doing, testing, done). Doing this will stop production when work accumulate thus helping you to visualize problems and constraints. "Stop starting, start finishing"

**Appreciate the System:**
- Gain a deep understanding of the business system IT operates within.
- Identify dependencies on IT and improve its role in enhancing the system.
- Address under-scoped and over-scoped work.
 
**Manufacturing Production Control:**    
Ensure each work center has enough capacity and necessary input.

"Your job as IT Operations is to ensure the fast, predictable and uninterrupted flow of planned work that delivers value to the business while minimizing the impact of and disruption of unplanned work, so you can provide stable, predictable and secure IT service"

**Reduce Waste:**
Waste is the use of material or resources beyond what the client requires and is willing to pay for.

7 types of waste: Inventory, overproduction, extra processing, transportation, waiting motion, defects.

**Best Practices:**

- **Work in Small Batches:** Smaller work portions facilitate faster completion, quicker feedback, and more efficient problem resolution.

- **Change Management:** Effective change management processes minimize disruptions and help adapt to new challenges smoothly.

- **Prioritize Meaningful Work:** Only accept work/projects aligned with business objectives. Always check for available capacity.

- **Task Clarity:** Clearly identify the which main business projects/goals supported by the task. Make blocked task clearly visible.

- **Automation:** Automate processes to improve productivity, reduce manual work, increase efficiency, and ensure consistency and reliability in IT operations.

#### Second Way: Feedback Loop

**Objective:** Fix quality issues at the source to avoid rework and enable faster detection and recovery of problems by maintaining a constant flow of fast feedback throughout the entire development process.
##### **Key Principles:**

**Early Feedback Loop** 
Implement a feedback loop from the earliest stages of product definition, design, and development to create quality at the source. This enables faster detection and recovery of problems

**Practices to Apply the Second Way**
- **Make wait times visible**
- **Make sure Important metric are accessible and reliable**
- **Stop Production Line on Failures:** Halt the deployment pipeline when builds and tests fail. This makes problems more visible.
- **Swarming**: Implement a practice of "swarming" when problems occur, encouraging everyone to stop and collaborate to solve issues. This approach promotes a diversity of perspectives and provides learning opportunities for all involved.
- **Collaboration:** Foster better cooperation between Development and IT Operations, emphasizing shared goals and shared pain.
- **Production Telemetry:** Implement production telemetry to ensure code and environments function properly and meet customer requirements.

**Important Metrics**
- **Lead Time:** Measure the time from the creation of a ticket to its completion, as it directly impacts the customer experience.
- **Process/Task Time:** Track the time from the beginning of work to its completion.
- **Percent Complete & Accurate:** Assess how often the delivered work is usable as is.

**Assessing Project Worthiness**
- Does the project enhance operational stability?
- Does it reduce the time required to detect and recover from security breaches?
- Does it increase the capacity of the most constrained resource in the company (Brent)?

**Performance Indicator Integration**
Engage with business process owners to identify risks associated with their processes and incorporate these risks into performance indicators. The goal is not only to improve performance but to obtain early indicators that prompt action.

**Documentation and Flow Improvement**
Document the steps and resources for frequently requested tasks and analyze their workflow for optimization.

**Focus on Customer Value**
Always align IT goals with customer needs and business value, ensuring that technology serves the larger purpose of the organization.

**Tracking Faint Signals**
Consider tracking even subtle signs of improvement after resolving significant issues. For example, after reducing injuries in an aluminum plant by 96% by tracking and responding to all injuries, they started tracking and responding to minor injuries and close calls to maintain safety improvements.

#### The Third Way: Continuous Learning

**Objective:** Foster a culture of experimentation, learning from failure, and recognizing that repetition and practice are essential for mastery.
##### **Key Principles:**

- Be open to innovation and risk taking instead of blindly taking orders;
- Cultivate an environment of trust and openness among team members
- Allocating at least 20% of Development and IT operations to Internal improvement.
- Encourage and Celebrate Improvements
- Conduct Blameless Post-Mortems

**Consistent Practice**
Consistently practice and refine skills, as "five minutes of daily practice is more beneficial than three hours once a week."

**Kaizen Blitz** 
Organize self-organized team cycles to address and resolve any issues they identify, promoting continuous improvement.

**On the Importance of Trust**
Building a foundation of trust within the organization is crucial. Trust empowers teams to take ownership of their work, collaborate effectively, and communicate openly.

Without trust our first instinct is to protect ourselves at the detriment of the team and the organization. It prevent us from raising issues, share ideas, admit to errors, etc.

**Repetition Builds Trust**
Repetition, especially in teamwork, is essential as it creates transparency and trust. Trust is crucial for tackling complex business problems and encourages team members to share ideas, admit errors, and raise concerns.

**Technical Debt Chain**
Technical debt -> fragility -> breakage -> Unplanned work -> less time for planed work.

**Fire Drills (Unsure of how practical it is)**
Conduct incident calls to develop problem-solving skills systematically. Consider integrating this with learning from Finland's approach to avoiding unnecessary repetition. Each successful drill would push back the schedule for the next one and vice versa.

---
### The Theory of Constraints (Dr. Goldratt)

“Until you create a trusted system to manage the flow of work to the constraint, the constraint is constantly wasted, which means that the constraint is likely being drastically underutilized.”  

 5 steps in the Theory of Constraints:

1. Identify the constraint

2. Exploit the constraint: Don't allow constraint to be working on something else than main priority or be waiting for someone else.

3. Subordinate other activities to constraint

4. Elevate the constraint to new levels: Offload tasks, integrate tasks, simplify tasks, or as ends up being a common choice in the book, eliminate tasks.

5. Find the next constraint

> "Improvements made besides the bottleneck are illusory: the improvements made after the bottleneck are useless as they still wait for work from the bottleneck, and the improvements made before it result in more problems piling up."

**Story Example**:
Brent is the most apt at building and fixing everything at the company, more so than other senior dev. Because of this he ends up supporting too many project and department (AKA Work Centers), which is why he is a constraint. One person can only work at one work center at a time.

The projects that prevent escalation to Brent (The constraint) and document is knowledge to be usable by anyone, are therefore the most important one.

---
## Secondary Concepts
Concepts referenced a few times through the book.

---
### Risk Evaluation

- Fragile: must be authorized by CAB
- List most fragile services
- Document success rate of similar changes and associted downtime

low risk: daily standard stuff done many times before successfully (still need to be submited, auto approve but can be scheduled at will)
medium risk: unknown, rare task (need too provide info and seek permission from affected parties)

---
### 5 Dysfunctions Of A Team 

1. **Absence of trust**: unwilling to be vulnerable within the group

2. **Fear of conflict**: seeking artificial harmony over constructive passionate debate

3. **Lack of commitment**: feigning buy-in for group decisions creates ambiguity throughout the organization

4. **Avoidance of accountability**: ducking the responsibility to call peers on counterproductive behavior which sets low standards
   
5. **Inattention to results**: focusing on personal success, status and ego before team success

---
### Continuous Improvement 

2 week improvement cycle

Implement one small Plan-Do-Check-Act project

1. **Plan**: In this stage, you identify the problem or opportunity for improvement and plan how to address it. This involves setting clear objectives, defining goals, and determining the scope of the project. You also develop a detailed plan, outlining the actions to be taken, resources required, and a timeline for implementation.

2. **Do**: This stage involves implementing the plan developed in the first stage. It's the execution phase where you put your plan into action. This may involve making process changes, conducting experiments, or implementing new procedures or practices.

3. **Check**: After implementing the plan, you monitor and measure the results to assess whether the changes have had the desired effect. This stage involves data collection and analysis to evaluate the impact of your actions. You compare the actual results with the expected outcomes and determine if any variations or discrepancies exist.

4. **Act**: Based on the findings from the "Check" stage, you make decisions and take action to either standardize the new process if it has improved performance or adjust the plan if necessary. If the results meet the objectives, you can implement the changes as standard practice. If not, you refine the plan and go through the PDCA cycle again until the desired improvements are achieved.

---
### Key Performance Indicator (KPI)

You need to find your Key Performance Indicator that align with goals

**Example**: 
	**Industry**: Trucking 
	**Company goal**: On time delivery
	**Factor**: Vehicle break 
	**KPI**: Percent of truck who had their required oil change done
	**Why?**: High percent leads to breakage and late delivery

---
## Other Referenced Concepts
Concepts referenced a once through the book.

---
### The Five Core Lean Principles

1. **Value**: Identify what creates value from the customer's perspective. Understand customer needs and preferences to determine what they are willing to pay for. Focus resources and efforts on delivering that value.

2. **Value Stream**: Map the entire value stream for a product or service, including all the steps and activities required to bring it from concept to delivery. This helps identify areas of waste, inefficiency, and bottlenecks.

3. **Flow**: Create a continuous and smooth flow of work through the value stream. Minimize interruptions, delays, and handoffs. Ensure that work moves steadily and efficiently from one stage to the next.

4. **Pull**: Implement a pull system where work is initiated based on customer demand rather than pushing work through the process. This reduces overproduction, excess inventory, and unnecessary work.

5. **Perfection**: Strive for continuous improvement and perfection. Continuously seek ways to eliminate waste, reduce defects, and improve processes. Encourage a culture of learning and Kaizen (continuous improvement).

---
### Value Stream Map (VSM) 

A visual representation and analysis tool used in Lean and Continuous Improvement methodologies, particularly within the realm of process optimization and waste reduction. It is a detailed and holistic illustration of a specific process or set of processes within an organization, showing the flow of materials, information, and actions from the beginning (typically customer demand) to the end (delivery of the final product or service).

**Key characteristics and components of a Value Stream Map:**

1. Process Steps: The VSM identifies all the individual steps or activities that make up the process being analyzed. These steps can include tasks, workstations, machines, or decision points.

2. Information Flow: It shows how information flows within the process, including data, instructions, orders, and feedback. This helps identify potential bottlenecks and delays caused by information gaps.

3. Material Flow: The map illustrates how raw materials, components, and products move through the process. This includes transportation, inventory points, and storage locations.

4. Time Metrics: Value Stream Maps often include time-related metrics, such as cycle time (the time it takes to complete one unit), lead time (the time from order to delivery), and processing time at each step. These metrics are crucial for identifying areas of improvement.

5. Work in Progress (WIP): WIP is the amount of unfinished or partially completed work within the process at any given time. VSMs typically show WIP levels at various stages of the process.

6. Process Symbols: Standard symbols are used in Value Stream Maps to represent specific elements, such as processes, inventory, transportation, decision points, and delays. These symbols make the map easy to understand and interpret.

7. Data Boxes: Data boxes provide additional information and metrics related to each process step, including the number of operators, cycle times, and other relevant data.

8. Customer and Supplier Icons: Value Stream Maps include icons representing customers (external or internal) and suppliers, indicating where the process begins and ends in relation to customer demand.

**The primary objectives of creating a Value Stream Map are:**

1. Identify Waste: VSMs are used to pinpoint areas of waste, such as overproduction, excessive waiting, unnecessary transportation, and defects. These areas are often targeted for improvement to streamline the process.
 
2. Improve Flow: By visualizing the flow of materials and information, organizations can identify bottlenecks and areas of congestion and take steps to optimize the flow.
 
3. Reduce Lead Time: Analyzing the VSM helps organizations reduce lead times, allowing them to respond more quickly to customer demand and improve overall efficiency.

4. Enhance Quality: By identifying defects and areas prone to errors, organizations can implement measures to improve product or service quality.

5. Align with Customer Demand: VSMs help align production and process capabilities with customer demand, reducing the risk of overproduction or stockouts.

Value Stream Mapping is a valuable tool for organizations striving to eliminate waste, improve processes, and create value for their customers. It is often used in conjunction with other Lean tools and methodologies to drive continuous improvement efforts.

---
### CIA data triangle

- Confidentiality
- Integrity
- Availability
  
  Note: Any change that can affect this should be tagged and scrutinized

---
### Kaizen

1. **Incremental Improvement:** Kaizen encourages employees at all levels of an organization to identify and implement small, manageable improvements in their work processes. These improvements can be as simple as optimizing a workstation layout, streamlining a production process, or reducing waste.

2. **Continuous Effort:** Kaizen is not a one-time initiative but an ongoing and never-ending process. It fosters a culture of continuous learning and improvement within an organization. Employees are encouraged to consistently seek ways to enhance their work and make it more efficient.

3. **Employee Involvement:** Kaizen promotes the idea that those closest to the work processes are best equipped to identify areas for improvement. It encourages employees to actively participate in problem-solving and decision-making, empowering them to contribute their insights and ideas.

4. **Elimination of Waste:** One of the primary goals of Kaizen is to eliminate waste in all its forms, including overproduction, excess inventory, waiting times, unnecessary motion, defects, and underutilized employee skills. By reducing waste, organizations become more efficient and cost-effective.

5. **Standardization:** While Kaizen encourages continuous improvement, it also emphasizes the importance of standardizing improved processes to sustain the gains achieved. Standardized work processes help maintain efficiency and consistency.

6. **PDCA Cycle:** The Plan-Do-Check-Act (PDCA) cycle is a problem-solving methodology often used in Kaizen. It involves planning a change, implementing it, checking the results, and acting to standardize or improve further based on the outcomes. The cycle is repeated continually for ongoing improvement.

7. **Top-Down and Bottom-Up Approach:** Kaizen can be initiated and supported by management, but it is also driven from the bottom up, with employees actively participating in improvement efforts. This two-way approach ensures that ideas flow freely throughout the organization.

Kaizen has been widely adopted in various industries beyond manufacturing, including healthcare, services, and software development, as it offers a systematic and sustainable way to improve quality, productivity, and overall performance. It promotes a culture of excellence and continuous learning within organizations.

Toyota Improvement quota?

---
### Order to cash cycle
from the initial order placement to the final payment receipt

1. Order Entry: When a customer places an order for products or services.    
   
2. Order Processing: Check for accuracy, availability of inventory, pricing, and credit terms. Any necessary adjustments or validations are made to the order during this stage.

3. Order Fulfillment: Picking, packing, and shipping the ordered products or preparing the services for delivery. Ensures that the customer receives what they ordered in a timely manner.

4. Invoicing: The formal request for payment sent to the customer.

5. Accounts Receivable: The invoice amount is recorded as accounts receivable until it is paid.

6. Payment Processing: Payment for the products or services received.

7. Cash Application: Recording and applying to the specific customer's account. The accounts receivable balance is reduced by the amount of the payment received.

8. Reconciliation: The company reconciles its records to ensure that all invoices have been paid and that there are no discrepancies or outstanding balances. Any disputes or discrepancies with the customer are addressed and resolved during this phase.

9. Reporting and Analysis: Businesses often analyze O2C data to track key performance metrics, such as Days Sales Outstanding (DSO), collection rates, and order fulfillment efficiency. This data helps identify areas for improvement and optimize the O2C process.

10. Credit Management: Throughout the O2C cycle, credit terms and credit limits for customers are managed to minimize credit risks and ensure timely payments.

---
### Total Productive Maintenance

Ref: https://www.leanproduction.com/tpm/

 Prioritize maintenance to assure machine availability
 
> "Improving daily work is more important than doing work"
> 
> "Entropy is inevitable, therefore there will always be errors, accidents and loss. You need to be resilient to those."

---
### Idle Time / Slack

Paradoxically being at or near full capacity when it come to time usage leads to unproductivity. This is because it means that work transfer between 2 person is bound to get stuck into queue. It also means any delay in a task affects the next one.

**Example**:
Imagine two 1h meetings scheduled back-to-back, if the first one runs long then the second one gets delayed affecting all participants. If buffer is given between the meetings then the second one is not disrupted.

People should have Slack between 20% to 50% of their time.

The wait time is the "percentage of time busy" divided by the "percentage of time idle". If a resource is fifty percent busy, then it's fifty percent idle. The wait time is fifty percent divided by percent, so one unit of time. Let's call it one hour. So, on average our task would wait in the queue of one hour before it gets worked.

If a resource is ninety percent busy, the wait time is "ninety percent divided by ten percent", or nine hours. A task would wait in the queue nine times longer than if the resource were fifty percent idle.

---
## Misc
Anything worth of note that is not a explicit reference to a specific concept.

---
### Interview Questions for Product Owner
To makes sure you have a clear picture and don't have incorrect preconceived notion.

- What is your role (not title)?
- What differentiate a good day from a bad day?
- What are your goals, objectives and measurements for this year?
- Which of these measurements are the most at risk?
- Who is responsible and accountable for each? 
- What is challenging you to achieve your goals?

---
### Common Business Challenges
- Unrealistic expectations (Leads to feelings of helplessness)
- Demoralized employee quite and finding / training new one take time before they become profitable
- Lack of coordination (Lost sales because inventory was not tracked reliably)
- Lack of information about customer needs and want
- Lack of internal information
- Lack of reliable/accurate information (like entry errors, bad assumptions)
- Lack of timely information (info updated daily vs every months)
- Lack of proper funding
- Lack of proper prioritization
- Lack of testing (A/B testing)
- Fragility leading to no room for experimentation / risk taking
- Too long to get to market leading to missed sales and locked capital not providing returns
- Too long of a planning horizon

You need a system to prevent challenges or at lest detect and remedy.
Need to be aware of which business risk are related to IT

---
### Internal hurdle rate for project 
Return on investment must be above 10% or else you could just invest the money in the stock market.

---
### Chief Financial Officer (CFO) Goals

- Health of company
- Revenue
- Market share
- Average order size
- Profitability
- Return on assets
- Health of Finance
- Order to cash cycle (from the initial order placement to the final payment receipt)

> "Without the right product or service (Business Goals), the goals of an department may be achieved but the company will still fail. The entire organization need to reach their goals not just part of it."

---
### General Business Goals
- Are we competitive
- Understanding customers wants and needs: Do we know what to build?
- Product Portfolio: Do we have the right product?
- R&D effectiveness: Can we build it effectively?
- Time to market: Can we ship it soon enough to matter?
- Sales pipeline: Can we convert products to interested prospect? Are we effective?
- Customer on-time delivery: Are customer getting what we promised them?
- Customer retention: Are we gaining or losing customers?
- Sales forecast accuracy: Can we factor this into our sales planning process?

---
### Question to ask about change, task or projects

- Does it increase the flow of project?
- Does it increase operational stability or decrease time required to detect and recover from outage or security breach?
- Does it increase the constraints capacity to work on main goals?
- Would it increase the amount of work (stuck) in progress?

If the impact of change, task or project is negative then it doesn't bring value to the company and should probably not be done at all.

---
### Work Center
work centers are made of
- Machine
- Man
- Method
- Measure

---
### The only 3 internal control objective needed

1. Reliability of financial reporting
2. Compliance with the law
3. Compliance with efficacy and effectiveness of operation.

---
### Core Qualities of a Project

- Features
- Stability
- Security
- Scalability
- Manageability
- Operability
- Continuity
- Survivability
- Supportability
- etc.

---
### Water spider (factory position) 
Someone assigned to carry around task from person to person like a waiter
should be automated

---
### Reading List

Continuous delivery - Jez Humble
The Goal - Dr Goldratt
Beyond The Goal - Dr Goldratt
Lean Thinking - James
The Lean Startup - Eric Ries
The high velocity edge - Spear
The fifth discipline - Senge
5 Dysfunctions Of A Team - Patrick Lencioni’s
The devOps Handbook - Gene Kim - Jez Humble
John Allpaw - IT Flikr (10 deploys a day) DevOps
Toyota Kata - Mike Rother
Release It!: Design and Deploy Production-Ready Software - Mike Nygard
Visible Ops and ITIL Service Support

---
### Quotes 

>  "Your job as IT Operations is to ensure the fast, predictable and uninterrupted flow of planned work that delivers value to the business while minimizing the impact of and disruption of unplanned work, so you can provide stable, predictable and secure IT service"
>  
> "Features are always a gamble. If you’re lucky, 10% will get the desired benefits. So the faster you can get those features to market and test them, the better off you’ll be. Incidentally, you also pay back the business faster for the use of capital, which means the business starts making money faster, too.”
> 
> "Every company todays is in the technology business whether they realize it or not"
> 
> "Work only generate value when deployed"
> 
> "Commiting code should automatically deploy in prod" (Should we really?)
> 
> "When people have concern they don't want their mind change (avoid charismatic people who are likely to try to change their mind)"
> 
> "The flow of work should go into one direction only: Forward"
> 
> “To tell the truth is an act of love. To withhold the truth is an act of hate. Or worse, apathy.”
> 
> “until code is in production, no value is actually being generated, because it’s merely WIP stuck in the system.”
> 
> “Resilience engineering tells us that we should routinely inject faults into the system, doing them frequently, to make them less painful.”
> 
> “If you can’t out-experiment and beat your competitors in time to market and agility, you are sunk"
> 
> "How in the hell do you support and secure something that’s written in Microsoft Access?"
> 
> "The operational risks posed by IT need to be managed like any other business risk"



