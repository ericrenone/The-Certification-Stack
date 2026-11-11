# The Certification Stack

## Why accumulating agile credentials manages around the work, copies prestige downward, and leaves enterprise transformation with no one who can read the architecture

*A long-form analysis, November 2026. The two senior-leader examples are composites drawn from executive-level conversations at a large card issuer and a universal bank; no individual is identified and no detail is exact.*

---

## Summary

1. The agile certification market is large, cheap to enter, and almost impossible to fail. Two million credentials from one body alone; two-day courses with 50-question exams and pass rates near 95 percent; total cost between $400 and $1,500 per credential. Anyone with a free weekend and a corporate card can hold five by spring.

2. A certification certifies vocabulary, not capability. It verifies that the holder can describe a framework's roles, ceremonies and artifacts. It does not verify that the holder has ever specified a data pipeline, designed an evaluation gate, traced lineage across a system of record, or made a trade-off between latency and consistency. Those are the decisions that decide whether an enterprise transformation ships.

3. Certifications stack for a reason that has nothing to do with the work: prestige copies downward. When a senior leader's profile carries a column of badges, the people below optimize for the same column, promotion criteria quietly encode it, and the organization ends up selecting for the proxy instead of the thing. The cheaper the credential, the faster the cascade.

4. The result is a leadership layer fluent in managing *around* the work: cadences, ceremonies, release trains, program increments, maturity assessments. Fluent in everything except the system being transformed. When that layer meets a real architecture decision, it delegates to a vendor, a consultant, or the one engineer in the room, and then owns the outcome without understanding it.

5. The evidence is consistent with this. Independent studies find no relationship between project-management certification and project outcomes, and at least one finds a negative one. Only about one in eight non-degree credentials produces a meaningful wage gain. The practices that *do* predict delivery performance are technical: automated testing, continuous integration, trunk-based development, small batches, observability. None of them is on a Scrum Master exam.

6. The alternative is not "no credentials." It is depth made visible: artifacts the holder specified, decisions the holder made and can defend, and a record that survives a technical interview. The sections below lay out the market, the mechanism, the two canonical cases, the evidence, and what an enterprise should select for instead.

---

## 1. The market, in numbers

The certification industry around agile is not a cottage business. It is a mature, multi-body market with its own pricing tiers, renewal fees, and sales channels.

**Volume.** Scrum Alliance announced in 2025 that its community had passed two million credentials earned. Scaled Agile claims more than a million practitioners and says it has trained over two million SAFe-certified professionals across twenty thousand organizations, with adoption at more than 70 percent of the Fortune 100. Scrum.org, PMI, ICAgile and APMG each run their own ladders. Taken together, the number of agile credentials in circulation is in the several millions, against a global population of software and product professionals in the tens of millions. In large enterprises, the ratio is far higher: it is common for a transformation office to require one.

**Price.** The entry-level credentials cluster in a narrow band:

| Credential | Format | Typical all-in cost | Pass bar |
|---|---|---|---|
| Certified ScrumMaster (CSM) | Mandatory 2-day course, then 50 questions in 60 minutes, two attempts included | $400–$1,500 | 74% (37 of 50); pass rate estimated near 95% |
| SAFe Agilist (SA) | Mandatory 2-day course, then 45 questions in 90 minutes | $995–$1,200 | 77% (35 of 45) |
| Professional Scrum Master I (PSM I) | Exam only, 80 questions in 60 minutes | about $200 | 85% |
| Certified Scrum Product Owner (CSPO) | Mandatory 2-day course; no exam | $400–$1,500 | none |
| PMI-ACP | 120 scenario questions in 180 minutes; requires documented experience | $700–$2,500 | not published |

Renewal runs $60 to $150 a year plus "education units," which are frequently satisfied by attending the vendor's own webinars.

**Difficulty.** With one exception, the exams are designed to be passed. The CSM requires attendance at a course and then a 60-minute multiple-choice test on material covered the day before; the course fee includes two attempts. The CSPO has no exam at all: attendance is the credential. SAFe's 45-question exam follows a two-day course that walks through the exact material. The PMI-ACP is the outlier: it requires documented agile experience and a three-hour scenario exam, and it is correspondingly rarer on senior profiles, which is itself a signal about what people are optimizing for.

**Stacking cost.** A plausible stack of CSM, CSPO, SAFe Agilist, SAFe POPM and ICP runs roughly $3,000 to $5,000 and ten working days. A corporate learning budget covers it. An individual with time and $500 to $1,000 can accumulate two or three a year indefinitely. There is no upper bound, no portfolio review, and no point at which a governing body asks the holder to show something they built.

**What the market sells.** Look at what the bodies advertise when challenged. When the Wall Street Journal reported in 2025 that most certificates and digital badges don't pay off, Scaled Agile's response did not argue that SAFe makes transformations succeed. It argued that SAFe-certified professionals earn about $12,000 more per year and that postings referencing SAFe advertise higher salaries. The defense of the credential was that the credential is rewarded. That is the market's own account of what it is for.

---

## 2. What a certification can certify, and what it cannot

Be precise about what a two-day course and a 50-question exam can establish.

**It can establish** that the holder:
- knows the names and purposes of the roles (Scrum Master, Product Owner, Release Train Engineer);
- knows the names and cadence of the ceremonies (sprint planning, daily scrum, review, retrospective, PI planning);
- knows the names of the artifacts (product backlog, sprint backlog, increment, program board);
- can answer vocabulary questions about them under light time pressure;
- sat in a room for two days.

**It cannot establish** that the holder has ever:
- written a requirement that an engineer could build without a follow-up meeting;
- read an architecture diagram and found the problem in it;
- specified how data moves from a system of record to a consumer, with ordering, freshness, and failure handling;
- designed an evaluation that blocks a release;
- made a trade-off between consistency and latency, or between throughput and cost, and lived with the consequence;
- told a sponsor that the date is not achievable and been right;
- shipped anything.

Every item in the second list is the job of leading a transformation. None of them is examinable in multiple choice, and none of the governing bodies attempts to examine them. The gap between the two lists is the whole argument.

Notice also what the certifications are *about*. They are about the process that surrounds the work: how to organize people, how to run meetings, how to sequence time. The work itself (the data, the integrations, the models, the controls) is treated as a black box that the process is wrapped around. This is why a leader can hold six of them and be unable to answer "where does this field come from" or "what happens when the upstream feed is late." The curriculum never asked.

---

## 3. Two canonical cases

What follows is a composite. The details are deliberately blurred and no individual is identified. The pattern, however, is specific enough to recognize, because it recurs across large financial institutions with a consistency that suggests a structural cause rather than individual failing.

### 3.1 The executive director at the card issuer

A senior leader running a transformation program in a payments business. The profile carries a column of credentials: a Scrum Master certification, a Product Owner certification, an enterprise scaling certification, an agile leadership certification, and a project-management credential. The résumé language is fluent in the framework: release trains, program increments, value streams, lean portfolio management, communities of practice.

In a technical conversation about a real product (say, a decisioning or routing capability with hard latency requirements), the questions come from the process side: how would you structure the backlog, how would you run the PI planning, how would you handle a dependency between trains. The questions that do not come: what's the latency budget, where does the decision data live, what happens when the model is stale, how do you know the output is right, who owns the schema.

When the candidate volunteers those questions, the conversation moves back to process. Not from hostility; from vocabulary. The leader has a rich language for organizing the work and a thin one for the work itself. Decisions about the system are made by the engineering lead and ratified by the leader, who then owns the outcome in the operating review without the ability to interrogate it.

### 3.2 The executive director at the universal bank

A senior leader in a control or governance function at a large bank, running what the organization calls a transformation: the modernization of a reporting or surveillance platform. The credential column is similar, with a heavier emphasis on the enterprise scaling framework and a scattering of vendor product certifications.

Here the pattern is subtler, because the domain is data. The leader can talk about data governance, data quality, lineage, and controls in the abstract, because those words appear in the framework's portfolio-level material. What the leader cannot do is follow a lineage map. Asked which of forty-two tables a regulatory figure comes from, the answer is a delegation. Asked what the reconciliation rule is between two sources that disagree, the answer is a meeting. The transformation is "on track" in the program increment metrics and quietly stuck on the three architecture decisions nobody in the leadership layer can make.

### 3.3 What the two have in common

- **The stack is the career.** Each credential arrived at a promotion boundary, which is exactly when a proxy is most valuable and depth is least examined.
- **Fluency in managing around.** Both can run a program. Neither can run the system the program is changing.
- **Delegation as decision.** Architecture choices are made below and owned above. When they go wrong, the operating review attributes the failure to execution, never to the fact that the person accountable couldn't evaluate the choice.
- **Downward copying.** In both organizations, the people reporting to these leaders have, within a year or two, acquired the same credentials. Not because the work required them. Because the leader had them, and the leader decides promotions.

That last point is the mechanism, and it deserves its own section.

---

## 4. The prestige-copy cascade

Why do certifications stack, when nobody can point to a transformation that succeeded because its leader held five of them? Because the incentive to acquire a credential has almost nothing to do with the credential's content and almost everything to do with who else has it.

### 4.1 The leader sets the template

A senior leader's profile is a template for everyone below. People do not read the job description for the next level; they read the person who holds it. If that person's profile shows a column of badges, the badges become the visible definition of what senior looks like. The content of the badges is irrelevant to this effect. What matters is that they are visible, countable, and cheap.

### 4.2 The proxy enters the promotion criteria

Promotion committees need legible evidence. Depth is hard to make legible: it lives in decisions, artifacts and outcomes that take time to explain and expertise to evaluate. A credential is legible in one line. So the credential enters the criteria, first informally ("she's SAFe certified, that helps") and then formally ("SPC preferred" in the internal posting). Once it is in the criteria, the organization is selecting for it, and whatever an organization selects for, it gets more of.

### 4.3 The cheapness accelerates the cascade

If the credential cost two years and a thesis, the cascade would be slow and self-limiting. It costs two days and a corporate card. So it spreads at the speed of the learning budget. Within a cycle or two, everyone at the level below the leader has the same column, which means the column no longer differentiates, which means the next cohort adds one more credential to stand out, which is how a profile ends up with seven.

### 4.4 The proxy displaces the thing

This is the step that does the damage. When the proxy is cheap and the thing is expensive, people allocate their scarce development time to the proxy. The weekend that could have gone to reading the architecture goes to the exam prep. The year that could have produced one specified pipeline produces three badges. The organization's aggregate depth declines while its aggregate credential count rises, and the dashboards show the second number.

### 4.5 The market feeds the cascade

The governing bodies and their training partners are not neutral observers of this process. Their revenue is the cascade. The enterprise scaling framework's top credential, the program consultant, licenses the holder to train others, which means every certified consultant is a sales channel for the next cohort. Internal "transformation offices" staffed by holders of the credential have a direct interest in making the credential a requirement. Vendors fund the conferences where the credentials are advertised. The system is self-reinforcing by design, and it is a travesty of what the original movement intended; one of the authors of the agile manifesto has said as much, calling the imposition of methods by what he named the "Agile Industrial Complex" an "absolute travesty," and naming the neglect of technical excellence as a core problem.

### 4.6 Why the cascade ends in nowhere

A cascade of this kind doesn't produce a bad outcome immediately. It produces a leadership layer that is uniformly fluent in process and uniformly thin on the system. That layer performs well in the steady state, because steady-state management is mostly process. It fails at exactly the moment transformation requires: when the architecture has to change, when a migration has to be sequenced, when a model has to be evaluated, when two systems of record disagree and someone has to decide which one is right. Those decisions need depth, the layer has none, and the credentials provide no mechanism for acquiring it. The transformation stalls, the program increment metrics stay green, and the organization concludes it needs a better framework.

---

## 5. Managing around the work

The phrase deserves definition, because it describes a real competence that the certifications do teach.

*Managing around the work* is everything that organizes, sequences, reports and governs the work without touching it: backlogs, cadences, ceremonies, dependency boards, release trains, portfolio reviews, maturity assessments, communities of practice. It is necessary. A transformation without it is chaos.

*Managing the work* is deciding what the system should do and how: the data model, the integration contracts, the freshness and ordering guarantees, the evaluation that gates a release, the controls in the delivery path, the trade-offs between latency, cost, consistency and risk. It is also necessary. A transformation without it is a well-organized march toward a system that doesn't work.

The certification stack produces people who are expert at the first and absent from the second. Here is the gap, mapped against what actually breaks in enterprise data and AI programs:

| What breaks the transformation | Which credential covers it | What the credential actually teaches instead |
|---|---|---|
| Upstream data is a day stale; the product is wrong by morning | None | How to add a story to the backlog |
| Two systems of record disagree; the regulatory number depends on which wins | None | How to escalate a dependency at the program board |
| Events arrive out of order; a client's record goes backwards in time | None | How to run a retrospective |
| The model's output is accepted without a measurement of whether it's right | None | How to define a Definition of Done (as a checklist, not an evaluation) |
| A schema change breaks three downstream consumers | None | How to track cross-team dependencies |
| The review queue for high-risk outputs can't absorb the volume | None | How to assess team maturity |
| The migration has to run in parallel with the old path, with a verified cutover | None | How to plan a program increment |
| Latency at peak load exceeds the budget; the system falls over at month-end | None | How to prioritize by weighted shortest job first |
| Nobody can produce the lineage for an audit | Portfolio-level mention of "data governance" | Vocabulary |
| The vendor says the new model is better; nobody can check | None | How to run a supplier review |

Every row in the left column is a decision that a transformation leader will be asked to make or ratify. Every row in the middle column is empty. The credentials are not wrong about what they teach; they are silent on what matters, and the silence is structural, because the frameworks were designed to be domain-independent. Domain independence is precisely the property that makes a credential cheap to issue at scale, and precisely the property that makes it useless when the domain is the problem.

---

## 6. The evidence

Claims about credentials should be held to the same standard as the credentials claim to teach: measure the outcome.

**Certification and project outcomes.** A survey of 93 IT project managers found that certified project managers did not manage scope, time or cost better than uncertified ones. A 2019 university study expected certification to predict better outcomes and found instead that certification was statistically significantly correlated with *poorer* project quality. Neither study is large, and both concern project-management credentials broadly rather than agile ones specifically. But the direction is consistent, and there is no body of independent evidence pointing the other way. The governing bodies publish salary surveys, not outcome studies.

**Credentials and earnings.** The Burning Glass Institute, working with the American Enterprise Institute on 65 million career records, found that only about one in eight non-degree credentials produces a material wage gain, and that bottom-tier credentials provide few or no benefits. The Wall Street Journal's report on this work in 2025 is what prompted Scaled Agile's defense, and the defense, as noted, argued pay rather than performance.

**What does predict delivery performance.** The largest body of evidence on software delivery, the multi-year DORA research summarized in *Accelerate*, finds that performance is predicted by technical and organizational practices: version control for everything, continuous integration, trunk-based development, automated testing, deployment automation, loosely coupled architecture, monitoring, small batch sizes, and a culture that treats failure as information. Frequent releases and low defect rates go together. Certification is not among the predictors. The practices that predict performance are the ones a Scrum Master course does not cover and a SAFe course mentions in passing.

**The founders' view.** The people who wrote the original manifesto have been unusually direct. One called the imposition of methods by the certification and consulting industry an absolute travesty and named the lack of recognition of technical excellence as a core problem, noting that agile conferences rarely discuss the techniques of writing software. Another declared the word itself dead and advised dropping it in favor of describing the practices. The movement's own authors regard the credential economy as a corruption of what they proposed.

**The absence that matters most.** There is no published study, from any governing body or independent researcher, showing that organizations whose transformation leaders hold more agile credentials complete transformations faster, cheaper, or with better outcomes than organizations whose leaders hold fewer. For a market measured in millions of credentials and billions of dollars, that absence is the finding.

---

## 7. The transformation leader who cannot read the diagram

Bring the threads together into the single scene that recurs in every stalled program.

A transformation review. The leader at the head of the table holds five credentials. On the wall is an architecture diagram: systems of record on the left, an integration layer in the middle, consumers on the right, with a new component (a model, a platform, a data product) drawn in. An engineer is explaining why the cutover slipped: an ordering guarantee the design assumed doesn't hold under end-of-month volume.

Watch what the leader can and cannot do.

The leader *can* ask when it will be fixed, who owns it, whether it's on the risk register, and what the impact on the program increment is. Those are the questions the credentials taught. They are good questions. They are also the questions a competent administrator with no credentials would ask.

The leader *cannot* ask whether the ordering guarantee was ever necessary, whether keying by a different entity would remove the problem, whether the consumer could tolerate eventual consistency, or whether the fix the engineer is proposing introduces a new failure at the next scale. Those are the questions that decide whether the slip is a week or a quarter. The leader cannot ask them because nothing in the credential stack ever required reading a diagram like this one.

So the decision goes to the engineer. Which would be fine, except that the engineer is optimizing for the component and the leader is accountable for the program, and nobody at the table can connect the two. The leader ratifies. The review minutes record a decision. The organization has transferred accountability to the one person who cannot evaluate what they are accountable for.

This is the state that the certification cascade produces at scale: a layer of people whose job is to make the architecture decisions of a transformation and whose entire professional formation has been about everything except architecture. The program doesn't fail loudly. It drifts. Dates move. Scope narrows. A vendor is engaged. A new framework is adopted. The credentials get a new line.

Multiply the scene by the number of programs in a large bank, and you have the reason enterprise transformation has a reputation for going nowhere. It isn't that the people are unserious. It is that the selection mechanism, running for a decade, has filled the leadership layer with the wrong competence and certified it.

---

## 8. What depth looks like, and how to select for it

If the credential is the wrong signal, the question is what the right one is. It has to be as legible as a badge, or the promotion committee will keep using the badge. It can be.

### 8.1 Depth is an artifact plus a decision

Depth leaves evidence. Not a certificate: a thing that exists because the person made it exist, and a decision the person made about it that could have gone another way.

- A requirements document for a data pipeline that an engineer built from without a clarifying meeting, with the ordering, freshness and failure-handling decisions written down and the reason for each.
- An evaluation set, versioned, with thresholds, that has blocked at least one release.
- A lineage map the person produced, that an auditor used.
- A migration plan with its phases, its gates and the slip that happened, with what the person changed afterward.
- A trade-off memo: latency against consistency, cost against freshness, speed against review capacity, with the choice made and the consequence recorded.
- A one-page executive review that got a decision, not a status.

Each of these is one line on a profile and ten minutes in an interview. Each is impossible to acquire in a two-day course. Together they are a portfolio, and a portfolio is the only credential that correlates with the ability to lead a transformation, because it *is* the ability, recorded.

### 8.2 Five questions that separate depth from the stack

Any interviewer, technical or not, can ask these. The certified-only candidate cannot answer them; the candidate with depth cannot stop answering them.

1. **"Draw the system you transformed. Where did the data come from, where did it go, and what broke?"** Depth draws. The stack describes the program.
2. **"Tell me a technical decision you made that engineering disagreed with. What happened?"** Depth has one and remembers the consequence. The stack has a story about facilitating alignment.
3. **"How did you know the output was right?"** Depth describes a measurement. The stack describes acceptance criteria.
4. **"What slipped, and what did you change in the next gate?"** Depth names the predictor it should have alerted on. The stack names a dependency.
5. **"What would you have done differently if the review queue were half the size?"** Depth re-sequences the capabilities. The stack adds a story to the backlog.

None of these questions is hostile. They are the questions the work asks every week. A leader who cannot answer them in an interview will not be able to answer them in the transformation review either.

### 8.3 What an enterprise should change

- **Remove credentials from promotion criteria above the entry level.** Keep them, if at all, as a shared vocabulary for new joiners. Above that, require a portfolio.
- **Make the portfolio the legible unit.** One page per artifact: what it is, the decision in it, the outcome. Promotion committees can read six pages. They cannot read a transformation.
- **Interview for the diagram.** Every leadership interview for a transformation role includes a real architecture of the system in question and ten minutes of questions about it. Not to test engineering skill; to test whether the candidate can hold the system in their head well enough to make trade-offs about it.
- **Separate the program office from the decision rights.** The people who run cadence and reporting should not be the people who ratify architecture. If they are the same people, the second job will be done by whoever is loudest in the room.
- **Stop funding the cascade.** A learning budget that pays for the fifth credential is a budget that is not paying for the first specified pipeline. Fund artifacts: a quarter to produce one, reviewed by someone with depth.
- **Measure outcomes, not maturity.** Maturity assessments measure adherence to the framework. Outcomes measure whether the system works. A transformation that is "level four" and six months late is a failed transformation with a good score.

---

## 9. The steelman, and why it does not rescue stacking

Fairness requires the strongest case for the credentials, and it exists.

**Shared vocabulary.** In a large organization, a common language for roles and cadences reduces friction. A two-day course is a cheap way to give a thousand people the same words. This is real and it is why the entry-level credential has some value for new joiners.

**Procurement and compliance.** Some contracts and some regulated procurement processes require named credentials. Holding one is then a cost of doing business, not a claim of competence.

**A floor, not a ceiling.** For someone with no exposure to iterative delivery at all, the first credential is a floor. It is better than nothing.

**Signal of initiative.** Acquiring any credential shows a willingness to spend time and money on development, which is weakly informative about conscientiousness.

Every one of these arguments supports holding *one* credential at the *start* of a career. None of them supports holding five at the executive level, and none of them supports using the count as a promotion criterion. The vocabulary argument is exhausted after the first course. The procurement argument applies to the contract, not the leader. The floor argument is about beginners. The initiative argument, applied to the fifth credential, cuts the other way: it suggests time spent on the proxy that was not spent on the thing.

The steelman defends the credential. It does not defend the stack. The stack is what this analysis is about.

---

## 10. Twenty takeaways

1. A credential certifies vocabulary. Transformation requires decisions. The two are not the same, and the exams do not pretend otherwise.
2. The entry-level agile credentials are designed to be passed: two days, fifty questions, two attempts, pass rates near 95 percent, one with no exam at all.
3. A full stack of five costs about $3,000 to $5,000 and ten working days. There is no upper bound and no portfolio review at any level.
4. The credentials cover how to organize work and are silent on the work. The silence is structural: domain independence is what makes them cheap to issue and useless when the domain is the problem.
5. Prestige copies downward. A senior leader's badge column becomes the visible definition of senior, and the organization selects for it.
6. Once a proxy enters promotion criteria, the organization gets more of the proxy and less of the thing, because the proxy is cheaper.
7. The governing bodies and their consultants are the cascade's revenue model. The top credential in the scaling framework licenses the holder to sell the next cohort.
8. The independent evidence finds no relationship between project-management certification and project outcomes, and one study finds a negative one.
9. Only about one in eight non-degree credentials produces a material wage gain. The industry's response to that finding argued pay, not performance.
10. The practices that predict delivery performance are technical: testing, integration, small batches, loose coupling, observability. None is on a Scrum Master exam.
11. The authors of the original manifesto regard the credential economy as a travesty of what they proposed and name the neglect of technical excellence as the core problem.
12. The canonical failure is a leader who can ask when and who, but not whether and why. The first set runs a program; the second set runs a transformation.
13. When the accountable person cannot evaluate the decision, the decision is delegated downward and the accountability stays. That is the structure of a stalled program.
14. Stalled programs do not fail loudly. They drift, narrow, engage a vendor, adopt a new framework, and add a line to the credential column.
15. Depth leaves artifacts: a specified pipeline, an evaluation that blocked a release, a lineage map an auditor used, a trade-off memo, a slip and the gate that changed.
16. A portfolio of those artifacts is as legible as a badge column and is the only credential that correlates with the ability, because it *is* the ability, recorded.
17. Five interview questions separate depth from the stack, and none requires a technical interviewer: draw it, name the disagreement, how did you know it was right, what slipped, what if the queue were half.
18. Enterprises should remove credentials from promotion criteria above entry level, make the portfolio the unit, interview for the diagram, and separate the program office from decision rights.
19. The strongest case for the credentials supports holding one at the start of a career. It does not support holding five at the top, and it does not support counting them.
20. The reputation of enterprise transformation for going nowhere is not a mystery. A selection mechanism running for a decade has filled the leadership layer with the wrong competence and certified it.

---

## 11. Novel insights

These are the observations in this analysis that do not appear in the usual critiques of agile certification.

**1. The cascade is driven by cheapness, not by belief.** Most critiques assume people acquire credentials because they believe in them. The mechanism here needs no belief. It needs only a visible template above, a legible criterion in the middle, and a low price. Belief is optional; the cascade runs on incentives alone.

**2. Domain independence is the defect, not a feature.** The frameworks advertise that they apply to any industry. That property is what makes them scalable as a product and inert as a competence. A credential that could be specific to banking data architecture would be expensive to produce and would actually predict something.

**3. The proxy displaces the thing through time allocation, not through deception.** Nobody is lying. The weekend spent on the exam is simply not spent on the architecture. Aggregate depth declines through ten thousand reasonable individual choices.

**4. The industry's own defense concedes the point.** When challenged on outcomes, the scaling framework's defense was salary. A credential whose best argument is that it is rewarded has told you what it is for.

**5. The failure mode is silent and metric-green.** Program increment metrics, maturity scores and velocity are all process measures. A program can be fully green on all of them while the three architecture decisions that matter sit unmade. The credential economy has supplied its own dashboard, and the dashboard cannot see the problem.

**6. Delegated decision, retained accountability.** The specific structural harm is not that leaders lack depth; it is that the organization continues to hold them accountable for decisions they have, in practice, delegated to whoever in the room could read the diagram. The accountability and the competence have been separated, and the certification is what papered over the separation.

**7. The portfolio is already legible; it has just never been demanded.** The usual objection to replacing credentials is that depth is hard to assess. It is not. One page per artifact, six artifacts, ten minutes each. The committee has never asked because the badge was easier, not because the alternative was impossible.

**8. The right interview questions are not technical.** "Draw it," "what slipped," and "how did you know it was right" can be asked by anyone. They separate depth from the stack because the stack has no answer, not because the interviewer is an expert. Enterprises have been assuming they need engineers to interview for depth. They need the right five questions.

**9. The first credential and the fifth are different objects.** The steelman for credentials is entirely about the first one. The critique is entirely about the fifth. Debates about "whether certifications are worth it" conflate the two and never resolve, because both sides are right about different objects.

**10. Transformation's reputation is a selection effect.** The field's reputation for going nowhere is usually blamed on the difficulty of change. A simpler explanation is available: the people selected to lead it were selected on a proxy that does not measure the ability to lead it, and they have been for a decade.

---

## Sources

- Scrum Alliance, [Global Scrum Alliance Community Surpasses 2 Million Credentials Earned](https://www.streetinsider.com/Press+Releases/Global+Scrum+Alliance+Community+Surpasses+2+Million+Credentials+Earned/26684433.html) and [Annual Report 2025](https://www.scrumalliance.org/about/annual-report-2025)
- Scaled Agile, [Why The WSJ Got It Wrong About Certifications — And Why SAFe Still Delivers](https://scaledagile.com/blog/category/in-the-news/) (September 2, 2025)
- Burning Glass Institute and American Enterprise Institute, [Holding Credentials Accountable to Outcomes](https://www.burningglassinstitute.org/research/holding-credentials-accountable-to-outcomes) and [The Credential Value Index](https://www.burningglassinstitute.org/cvi)
- Martin Fowler, [The State of Agile Software in 2018](https://www.martinfowler.com/articles/agile-aus-2018.html) (Agile Australia keynote)
- Robertson (2019), university study on certification and project outcomes, summarized at [Acquisition Talk](https://acquisitiontalk.com/2019/02/are-certified-managers-associated-with-worse-project-outcomes/)
- [The Effects of Project Management Certification on the Triple Constraint](https://www.igi-global.com/article/the-effects-of-project-management-certification-on-the-triple-constraint/102483) (survey of 93 IT project managers)
- Certification cost, format and pass-bar data: [certdemand.com CSM overview](https://certdemand.com/certs/csm); [PMI-ACP vs CSM vs SAFe Agilist comparison](https://www.4pmti.com/?p=1004468) (training-provider source; figures cross-checked against issuing bodies' published formats)
- Forsgren, Humble and Kim, *Accelerate* (2018), and the DORA State of DevOps research it summarizes
