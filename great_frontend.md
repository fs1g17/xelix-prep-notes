## Behavioral Interview Cue Cards

### Walk Me Through Your Resume

- I started my career at 1Spatial as a junior full-stack developer.
- I worked on 1Streetworks, a roadworks planning product, and learned a lot from strong senior engineers.
- That gave me solid foundations across the stack and taught me how professional software teams operate.
- I then joined Capgemini Invent, where I worked on a greenfield healthcare application.
- On that project I became the dedicated frontend developer, working closely with design and user research.
- That experience strengthened my frontend skills and taught me how to translate user needs into practical interfaces.
- Most recently, I joined Ai-UP as a founding frontend engineer at an early-stage startup.
- We helped over 12,000 businesses generate leads, and I helped build the product from the ground up.
- That is where I really fell in love with startup culture: ownership, speed, ambiguity, and delivering customer value.
- Xelix feels like a natural next step: AP is new to me, but AI, automation, finance, and complex enterprise workflows are exactly the kind of challenge I want next.

### Why Have You Applied For This Role And Team?

- I am applying because the role sits at the intersection of things I enjoy: frontend, customer impact, data-heavy workflows, and startup ownership.
- I love frontend because of the short feedback loop and the direct connection to user experience.
- Frontend is not only about function; it is also about form, clarity, trust, and helping users make better decisions.
- Xelix’s product appeals to me because AP is complex, data-rich, and business-critical.
- The idea of using AI and automation to turn financial control workflows into something clearer and faster is genuinely exciting.
- I want to keep growing beyond implementation into product judgment, solution design, and owning problems end-to-end.
- Ai-UP taught me that I enjoy ambiguity, speed, and responsibility; Xelix feels like a place where those traits would be useful.
- The timing feels right because I am ready for a new level of challenge with larger customers, deeper workflows, and a more mature engineering environment.

### Improved Work After Feedback

- At Ai-UP, we were building a call-centre feature and needed to show lead status and call attempts clearly.
- I proposed a compact traffic-light-style design that combined both pieces of information into one visual column.
- The CEO pushed back and said it could be confusing for users.
- My initial instinct was that the design was efficient, but I realised efficiency is not useful if users have to decode the interface.
- I listened to the concern, stepped back from my preferred solution, and focused on the customer outcome.
- We moved to a clearer design: one column for the number of call attempts and another for the current status.
- The feature shipped quickly, users understood it, and it generated revenue soon after release.
- The lesson was to keep bringing ideas, but validate assumptions early and prefer clarity over cleverness in workflow-heavy interfaces.

### Difficult Stakeholder Or Teammate

- I try not to frame people as difficult; usually the difficulty is misalignment, constraints, or different priorities.
- On the SR1 healthcare project at Capgemini, design and user research were pushing for the best user journey, while I had to work within CASA framework constraints.
- One design idea was a cyclical questionnaire flow: if a user skipped a question, the final "next" action would loop them back before completion.
- After prototyping it, I found that this was not feasible within CASA's questionnaire model.
- Rather than just saying "no", I built quick prototypes, often within a couple of hours, so the team could see the constraint clearly.
- I also used PowerPoint and simple visual explanations to make the technical limitation understandable to non-technical stakeholders.
- We agreed on a different solution: users completed the questionnaire, then revisited skipped questions from the summary page.
- This kept the user need intact while fitting the technical framework.
- The lesson was to move difficult discussions away from opinions and toward evidence, prototypes, constraints, and shared goals.

### Creatively Solved An Engineering Problem

- At Ai-UP, users needed to generate leads by selecting OKVED business category codes.
- The challenge was that OKVED codes are hierarchical, with parent categories and many nested subcategories.
- I designed a hierarchical dropdown so users could browse the structure intuitively.
- When a user selected a parent category, all relevant subcategories were selected automatically.
- The first implementation used local React state, but with 2,800+ categories it became slow and laggy, especially on mobile.
- I moved the state management to Zustand and used selectors so updates only re-rendered the affected category branches.
- This made the dropdown much more responsive without needing to redesign the whole feature.
- We also needed search, and I kept the first version frontend-only so we could ship quickly without adding backend complexity.
- The result was a complex data-selection flow that felt simple to users and could be delivered quickly.

### Important Engineering Decision And Tradeoffs

- At Ai-UP, one important early decision was how to build the MVP quickly without creating a frontend we would immediately regret.
- We chose Next.js, shadcn/ui, and Tailwind because they reduced boilerplate around routing, styling, and common UI patterns.
- The tradeoff was that we accepted some framework and component-library conventions instead of designing every pattern from scratch.
- That was the right decision because our biggest risk was not technical originality; it was getting customer value into users' hands quickly.
- We also chose to prioritise desktop first because the initial high-value workflow was primarily used in a work context.
- The tradeoff was delaying a polished mobile experience, but we kept the layout flexible enough to add mobile support later.
- This helped us ship the MVP in just over four weeks and validate the product with real customers.
- The principle was to be pragmatic on reversible choices, but careful with foundations like maintainability, data flow, and architecture.
- Backup example: for OKVED search, I kept the first version as simple frontend substring matching rather than adding backend fuzzy search, because it was good enough for the MVP and avoided unnecessary backend complexity.

### Team Compromise

- I could use the traffic-light call-centre story here, but a better second example is the amoCRM integration at Ai-UP.
- We needed to send some default values as part of the integration.
- The backend engineer suggested adding those defaults on the frontend.
- My first instinct was that the backend might be a slightly cleaner place for defaulting logic.
- After discussing it, I agreed the frontend was pragmatic in this case because the data was already fetched, displayed, and submitted from the frontend.
- Putting the defaults in the backend would have added extra lookup logic for data the frontend already had.
- We chose the simpler approach, kept the integration moving, and avoided unnecessary backend complexity.
- The lesson was that compromise is easier when you focus on the total system cost, not just where code would look theoretically neatest.

### Greatest Area For Improvement

- My biggest growth area is deepening my product judgment.
- Technically, I am confident I can learn new stacks, tools, and patterns quickly.
- At this stage, the bigger challenge is not syntax; it is choosing the right problem and shaping the right solution.
- I want to get better at connecting engineering decisions to customer value, business impact, and user behaviour.
- Ai-UP helped me grow here because I was close to customers and had to think beyond implementation.
- I still want more exposure to mature product processes, enterprise workflows, and customer feedback loops.
- That is one reason Xelix stands out: the company seems very focused on customer value, adoption, ROI, and real workflow improvement.
- I want to become stronger at asking product questions earlier, not just executing well once the direction is set.

### Failed And Adopted A New Approach

- I tend to view failure as a systems signal rather than a personal label: what assumption was wrong, and what should change?
- At Ai-UP, I initially built the OKVED hierarchical dropdown using local React state.
- The approach seemed reasonable at first, but it failed once we tested it with the full dataset of 2,800+ categories.
- The UI became slow and laggy, especially on mobile, because state updates caused too many components to re-render.
- That was the signal that the approach needed to change: the feature worked functionally, but not at the quality level users needed.
- I changed course and moved the state into Zustand, using selectors so only affected category branches re-rendered.
- This made the dropdown much more responsive and kept the user experience usable.
- The lesson was to validate performance with realistic data earlier, especially when building data-heavy interfaces.

### Tight Timeline Without Clear Direction

- At Ai-UP, urgent work often came up: bug fixes to prevent customer complaints or feature requests with clear revenue potential.
- Sometimes the UI/UX designer was not immediately available, but the work still needed to move forward.
- In those situations, I tried to make progress using existing product patterns, previous design decisions, and the user outcome we were trying to achieve.
- I would make sensible assumptions, keep the implementation flexible, and avoid over-investing in details likely to change.
- Because I had built a strong working relationship with the designer, I could usually predict the direction they would later suggest.
- Once the designer reviewed it, I would refine the UI based on their feedback rather than treating my first version as final.
- This helped us keep momentum on urgent work without ignoring design quality.
- The lesson was to make assumptions explicit, move quickly when needed, and leave room for expert feedback.

### Adapted To Changing Priorities Or Requirements

- At Capgemini, requirements on the SR1 healthcare project changed regularly because user research was ongoing.
- Sometimes that meant changing direction after implementation work had already started.
- It could feel frustrating because the team had invested effort, and occasionally it looked like regression.
- I tried to reframe it as progress: we had learned more about real user needs.
- If new research showed a better path, keeping the old implementation just because we had written it would have been the wrong tradeoff.
- I focused on adapting quickly, keeping code flexible, and helping the team move toward the updated user need.
- This mindset made requirement changes easier to handle because the goal was not preserving code; it was building the right product.
- The lesson was that iteration can feel inefficient locally but still be the fastest route to a better outcome.

### Learned A Skill Outside Work And Applied It

- I enjoy learning outside work and often choose technically challenging projects to stretch myself.
- Earlier in my career, I gained my Next.js and Tailwind skills through personal projects before applying them professionally.
- A stronger recent example was learning about CRDTs outside work.
- When Ai-UP was hiring backend developers, I saw an opportunity to apply that learning to a real internal need.
- I built a small self-hosted, Dockerised pair-programming platform for coding tests.
- The platform allowed collaborative code editing in the browser, using the CRDT concepts I had been studying.
- This helped me turn abstract learning into a practical tool rather than keeping it theoretical.
- The lesson was that outside learning is most valuable when I connect it back to real problems the team has.

### Learned A Skill After Observing Others Use It Well

- I have seen strong engineers use AI tools to move faster, explore ideas, and reduce boilerplate.
- That made me curious about how to use AI effectively without lowering engineering standards.
- Outside work, I experimented with AI-assisted coding on personal projects to understand where it helps and where it can be risky.
- It allowed me to spend more time in an architectural role: shaping the solution, reviewing tradeoffs, and steering implementation.
- I am also exploring agentic coding after discussing it with a friend who had been getting good results from it.
- The key lesson is that AI is most useful when the engineer still owns the outcome.
- I see it as a way to accelerate iteration, but not as a replacement for understanding the code, testing it, and making good product decisions.

### Communicated Technical Information To Non-Technical Audience

- At Capgemini, I often had to explain frontend and CASA framework constraints to non-technical stakeholders.
- The difficult part was that some design ideas looked simple from the outside but were not feasible within the framework.
- I tried not to overwhelm people with implementation details or framework internals.
- Instead, I used simple analogies, diagrams, and PowerPoint slides to explain the constraint visually.
- I focused on why certain options were risky or expensive, not just whether they were technically possible.
- Where possible, I used quick prototypes so stakeholders could see the behaviour rather than only hear an explanation.
- This helped the team understand why we chose certain solutions and reduced the feeling that engineering was just blocking ideas.
- The lesson was that technical communication is about giving people enough context to make a good decision, not proving technical knowledge.
