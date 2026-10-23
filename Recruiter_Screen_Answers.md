# Recruiter Screen: Questions and Best Answers

Cloud Solution Architect (Early in Profession), Microsoft Australia
Call: Monday 26 October 2026, 8:00 PM - 8:15 PM AEDT

---

## How to use this

- Learn the **beats**, not the words. Say it your own way each time so it sounds like you talking.
- Behavioural questions ("tell me about a time...") use **STAR plus Reflection**: Situation, Task, Action, Result, Reflection. Microsoft interviewers look for the reflection, so don't skip it.
- Other questions (intro, why Microsoft, logistics) use short beats. STAR doesn't fit them.
- Every answer should land on **customers or outcomes**, not just on what you get. That is the main theme of the JD.
- Anything in **[brackets]** is a fact to confirm before Monday. Only say what is true.

### Time budget for a 15-minute call

| Answer | Target |
|---|---|
| Tell me about yourself | about 50 seconds |
| Why CSA / why Microsoft | about 40 seconds |
| AWS to Azure | about 35 seconds |
| Customer story | about 70 seconds |
| Work rights and start date | about 25 seconds |
| Salary | about 20 seconds |
| Other interviews | about 20 seconds |
| Your questions | 2 to 3 questions |

---

## What the JD is looking for (and where you prove it)

| JD asks for | Your proof |
|---|---|
| 2 to 4 years in cloud, IT support or software | About 3 years: DNEG (1), AWS (2) |
| Translate technical concepts into customer outcomes | AWS escalations: plain-language updates to customer stakeholders. Customer pipeline story |
| Customer and business outcome mindset | Customer pipeline story. Cost and performance reviews at AWS that cut compute spend |
| Curiosity about AI, willingness to learn | Master of AI. Focus Bear internship. Halo Voice live |
| Cloud fundamentals, Azure certs or hands-on | AWS SA Associate. AWS and Azure pipelines at AWS. AZ-900 path [started / finished] |
| Build or automate simple solutions | Python and Bash diagnostic tooling at AWS. Foodbiz payroll automation. n8n workflows |
| Modern apps and APIs | Music app deployed three ways. Halo Voice on Cloudflare Workers |
| Security, governance, data protection | Halo Voice: API key never reaches the browser, short-lived tokens, rate limits. Least-privilege IAM, private S3 with pre-signed URLs |
| Proof of concept, MVPs, rapid prototypes to show ROI | Music app: same backend three ways, compared cost and effort, recommended serverless |
| SQL, Power BI, Python | SQL and Python yes. Dashboards in QuickSight and Grafana. Power BI: be honest, it's new to you |
| Growth mindset, learning agility | Learned AWS on the job and got certified. Data leakage catch. LiveKit rebuild |
| Clear communication and collaboration | Knowledge-base articles and internal training at AWS. Working with TAMs and service teams |

---

## 1. "Tell me about yourself."

**Beats**
1. Master's in AI at RMIT, finishing in December
2. About three years of work: DNEG, then AWS, customer-facing
3. What you're doing now with AI
4. Why this role

**Answer**

> "I'm in my final semester of a Master of AI at RMIT, finishing in December. Before that I spent about three years working. First at DNEG, building Python automation for VFX pipelines, and then two years at AWS as a Cloud Support Engineer. At AWS I worked directly with enterprise customers on production issues, and I built data pipelines alongside Solutions Architects. I'm also AWS certified.
>
> Right now I'm an ML engineering intern at Focus Bear, and I've built and launched my own AI voice receptionist.
>
> The part of AWS I enjoyed most was working with customers on how their setup should actually work, not just fixing it when it broke. That's why the CSA role really appeals to me."

**Don't**
- Say "entry point" or "a good team". It undersells you and sounds generic.
- Leave out Focus Bear and Halo Voice. Without them it sounds like you've only been studying since 2024.

---

## 2. "Why this role, and why Microsoft?"

**Beats**
1. You liked the customer side at AWS. CSA is that as the whole job.
2. Microsoft is where enterprise AI adoption is happening, which fits your AI plus cloud background.
3. The program lets you learn from experienced architects.

**Answer**

> "At AWS, the part I enjoyed most was working directly with customers, understanding what they actually needed and helping them get their setup right. The CSA role is basically that as the whole job, so it's a natural next step for me.
>
> Why Microsoft: a lot of enterprise customers are adopting AI right now through Azure OpenAI and Copilot, and Microsoft is right in the middle of that. With my Master's in AI and my cloud background, that's exactly where I want to be. And this being an Early in Profession program means I'd be learning from experienced architects while working with real customers, which is the best way for me to grow into the role."

**Don't**
- Flatter them ("the best teams", "the most intelligent minds").
- Make it all about what you get. Say what you bring to customers.
- Mention the long-term goal of starting your own company.

---

## 3. "Your background is mostly AWS. How comfortable are you with Azure?"

**Beats**
1. Honest: mostly AWS, but not starting from zero
2. Real Azure exposure: pipelines across AWS and Azure
3. Show the mapping with two or three examples
4. Admit real differences, say what you're doing about them
5. Proof you learn fast: learned AWS on the job and got certified

**Answer**

> "Honestly, most of my hands-on work is AWS, but I'm not starting from zero. At AWS I worked on customer data pipelines that ran across both AWS and Azure. And a lot of the core ideas carry straight across: networking, identity, security, cost. VPC maps to VNet, IAM to Entra ID, Lambda to Azure Functions. There are real differences too, especially around identity and governance, so I've [started / finished] the AZ-900 path on Microsoft Learn. I learned AWS on the job and got certified, so I'm confident I can do the same with Azure."

**Don't**
- Say "it's only the service names that differ". The interviewers are Azure people.
- Say you've finished AZ-900 if you haven't.

**Handy mapping if they probe**

| AWS | Azure |
|---|---|
| VPC | Virtual Network (VNet) |
| IAM | Microsoft Entra ID (plus Azure RBAC) |
| Lambda | Azure Functions |
| EC2 | Azure Virtual Machines |
| S3 | Azure Blob Storage |
| Redshift | Azure Synapse Analytics |
| CloudWatch | Azure Monitor |
| KMS / Secrets Manager | Azure Key Vault |
| VPC endpoint (PrivateLink) | Private Endpoint |

---

## 4. "Tell me about a time you worked with a customer on a difficult technical problem."

This is your most important story. It hits "customer outcome", "own the blocker" and "seamless customer experience" from the JD.

**STAR plus Reflection**

- **Situation:** At AWS, a customer was building a cross-account pipeline. Data in an S3 bucket encrypted with KMS in one account. Redshift in a private VPC in another account. They'd followed the docs but kept hitting Access Denied errors.
- **Task:** Get their pipeline working. The problem crossed IAM, S3 and networking, and my team only covered analytics services.
- **Action:** Got on a call first to understand it properly. Sent a written summary so we were aligned. Instead of passing it between three teams, I owned it. Researched internal articles and past cases, found the cross-account IAM role and the network rules were misconfigured. Sent the fix and stayed on a call while they applied it.
- **Result:** The pipeline came up and they were unblocked. [If you know how long they'd been stuck or what it unblocked for them, add it. Don't make up a number.]
- **Reflection:** Customers don't care which team owns a problem. They just want someone to own it.

**Answer (about 70 seconds)**

> "At AWS, a customer was building a cross-account pipeline. Their data sat in an S3 bucket encrypted with KMS in one account, and they needed to load it into a Redshift cluster in a private VPC in another account. They'd followed the docs but kept hitting Access Denied errors.
>
> I got on a call with them first to properly understand it, then sent a written summary so we were on the same page. The tricky part was that it crossed IAM, S3 and networking, and my team only covered analytics services. Normally that gets passed between three teams. Instead I dug through internal articles and past cases and found the cross-account IAM role and the network rules weren't set up properly.
>
> I sent them the fix and stayed on a call while they applied it, so we could deal with anything new straight away. The pipeline came up and they were unblocked.
>
> What I took from it: customers don't care which team owns the problem. They just want someone to own it."

**Technical notes (for the technical round, if they dig in)**
- A Redshift cluster in a **private** VPC does not use an internet gateway. With Enhanced VPC Routing it reaches S3 through an **S3 gateway VPC endpoint** (or a NAT gateway). Network pieces: the endpoint, its policy, the route table, and outbound security group rules.
- Cross-account access to SSE-KMS data needs all three:
  - **S3 bucket policy** in the data account allows the Redshift account's role
  - **KMS key policy** in the data account allows that role `kms:Decrypt`
  - **IAM role** on Redshift has permissions for both the bucket and the key
- It only works with a **customer managed key**, not the default `aws/s3` key.
- Say "the network rules" unless you're sure which piece it was. Only mention KMS or the endpoint if that was really part of the fix.

---

## 5. "What are your work rights, and when can you start?"

**Beats**
1. Start date first (it's inside their window)
2. Current visa, then the 485
3. Bridging visa, so there's no gap
4. Staying long-term

**Answer**

> "I can start full-time from 16 November, so that lines up well with your intake. I'm on a student visa right now. Once my exams finish I'll apply for the Temporary Graduate visa, the 485. That gives me full work rights for [two / three] years, and I'm covered by a bridging visa with full work rights while it's processed. Longer term I'm planning to stay in Australia and go for PR."

**If asked "Will you need sponsorship?"**

> "Not for the next few years. The 485 gives me full work rights, and I'm working toward PR."

**Confirm before Monday**
- [2 or 3 years on the 485.] Standard for a coursework Master's is 2 years. Some nationalities get longer. Check Home Affairs.
- [Full-time from 16 November] matches your student visa conditions after the course ends.

---

## 6. "What are your salary expectations?"

**First, ask for their band**

> "I'm open on that. For me the bigger factors are the team and the chance to grow in this role. Could you share the band for this level and what the overall package looks like? Then I can give you a proper answer."

**Only if they push for a number**

> "From what I've seen for similar roles, something around $105 to $115k base plus super feels right. But I'm flexible depending on the full package."

**Rules**
- Always say **"plus super"**.
- Quote **base**, never total compensation.
- Ask about bonus and stock separately. Don't add them into your number.
- If they share a band, use that over your research.

**Research behind the range**
- Glassdoor: CSA with 1 to 3 years, about $100-110k base.
- Levels.fyi, Microsoft Solution Architect I, Australia, base only: fresh hires $104k (0 years) and $111k (1 year). Internal staff $109k to $119k. Bonus roughly $15-27k plus some stock on top. Small sample, 2020 to 2024.

**Don't**
- Say "I don't have a figure in mind" and stop there. It anchors you low.
- Call this an "entry point". You have about three years of experience.

---

## 7. "Are you interviewing anywhere else?"

**Answer**

> "Yes, I'm in the early stages with a couple of companies for Cloud Engineer and Cloud Ops roles. But this one is my first choice. It's the customer-facing side that I enjoyed most at AWS, and those roles don't have that. If anything moves quickly elsewhere, I'll let you know."

**Don't**
- Overstate it. Most are applications or early screens.
- Name companies unless asked.
- Make it sound like pressure.

---

## 8. "Do you have any questions for me?"

Ask two or three. In this order:

1. **Which team?**
   > "The JD mentions multiple positions across Australia. Do you know which solution area or team I'd be in, like infrastructure, data, apps, or security?"

   The most useful question. The answer changes what you study for the technical round.

2. **Next steps and timeline**
   > "What are the next steps in the process, and roughly what timeline are you looking at?"

3. **Advice for the next round**
   > "Is there anything you'd suggest I focus on to prepare for the next round?"

**Backups if there's time**
- "What does the Early in Profession program look like in the first few months, in terms of training or mentoring?"
- "What do the people who do really well in this program have in common?"

**Avoid:** more questions about pay, leave or perks. Anything you could find on Microsoft's website.

---

## Extra questions that could come up

Not covered in the first mock, but these come straight from the JD and your CV. Same rules: learn the beats.

### 9. "Why did you leave AWS?"

Very likely, because there's a gap between AWS (ended 2024) and now.

**Beats**
1. The honest reason [you need to fill this in: for example, to do the Master of AI full-time]
2. Positive, not negative about AWS
3. Link to now: AI plus cloud is exactly what this role needs

**Answer shape**

> "I left to [your real reason, for example: do my Master of AI full-time]. I could see AI becoming a big part of what cloud customers were asking for, and I wanted proper depth in it, not just surface knowledge. Now I've got both the cloud background and the AI side, which is exactly what this role is about."

Fill in your real reason. Never criticise AWS.

### 10. "Tell me about your AI experience." / "How do you show curiosity about AI?"

**STAR plus Reflection: Halo Voice**

- **Situation:** Small businesses miss calls. I wanted to build an AI receptionist that actually works in production.
- **Task:** Build it, make it secure, and keep it cheap and fast.
- **Action:** Built it on Cloudflare Workers and the OpenAI Realtime API, with browser-to-model audio. Made sure the API key never reaches the browser (short-lived session tokens), and added rate limits and call time limits. The first version used LiveKit, but I realised it carried media-routing infrastructure a two-person call didn't need, so I rebuilt it without it.
- **Result:** It's live. The rebuild cut latency and running cost.
- **Reflection:** Design for what the customer actually needs, not the biggest setup you can build.

> "I built and launched my own AI voice receptionist for small businesses. It runs on Cloudflare Workers and the OpenAI Realtime API. I made sure the API key never reaches the browser by using short-lived session tokens, plus rate limits and call time limits. My first version used LiveKit, but I realised it was carrying infrastructure a simple two-person call didn't need, so I rebuilt it without it. That cut latency and cost. The lesson for me was to design for what's actually needed, not the biggest setup you can build."

**Honesty:** if asked how you built it, say you used AI coding assistance heavily. That's fine, and it shows you know how to use the tools.

### 11. "Tell me about a mistake or something you learned from." / Growth mindset

**STAR plus Reflection: data leakage catch**

- **Situation:** Deep learning assignment at RMIT. PyTorch classifier for drone hand signals.
- **Task:** Build a model that genuinely works on new people, not just the test set.
- **Action:** The results looked too good, so I checked instead of celebrating. Found data leakage: the same people were in both train and test. Moved to person-independent grouped cross-validation.
- **Result:** An honest evaluation of how it would perform on new people.
- **Reflection:** When results look too good, question them. Being right matters more than looking good.

> "In my deep learning course I built a classifier for drone hand signals, and the results came back looking too good. Instead of just taking them, I dug in and found data leakage. The same people were in both the training and test sets, so the model was partly recognising people, not gestures. I switched to person-independent cross-validation so the results were honest. The lesson: when something looks too good, question it."

**Don't** quote any accuracy numbers. The assignment isn't finished.

### 12. "How do you explain technical things to non-technical people?"

**STAR plus Reflection: high-severity escalations**

- **Situation:** High-severity escalations at AWS, with customer stakeholders who weren't technical.
- **Task:** Keep them informed and confident while systems were down.
- **Action:** Regular plain-language updates: what's broken, what we're doing, what happens next. Worked alongside TAMs and service teams. Kept clear running notes for handover.
- **Result:** Stakeholders stayed informed until systems were back up. Also wrote knowledge-base articles and ran internal training that shortened diagnosis time for the team.
- **Reflection:** People don't need every detail. They need to know what it means for them and what happens next.

> "At AWS I handled high-severity escalations where the people waiting on updates often weren't technical. I'd give them short updates in plain language: what's broken, what we're doing, and what happens next. They didn't need the detail, they needed to know what it meant for them. I also wrote knowledge-base articles and ran internal training, which helped the team diagnose issues faster."

### 13. "Do you have experience with SQL, Power BI or Python?"

> "Python yes. I've used it for automation at DNEG, diagnostic tooling at AWS, and my AI projects. SQL yes, for data work and pipelines. For dashboards I've used QuickSight and Grafana. Power BI itself is new to me, but it's the same idea, and I've [started a Microsoft Learn Power BI module]."

Only say the Power BI module part if you've actually started one.

### 14. "Tell me about a time you built or automated something simple."

> "At Foodbiz I automated the weekly payroll calculation in Excel, which removed a recurring source of errors. At AWS I wrote Python and Bash tooling to automate repetitive diagnostic checks. I like spotting something done by hand every week and just fixing it."

### 15. "Tell me about a time you compared options and made a recommendation."

Maps to the JD's "proof of concept" and "ROI".

**STAR plus Reflection: music subscription app**

- **Situation:** RMIT cloud project, team of four.
- **Task:** Decide how to deploy the backend.
- **Action:** Deployed the same Python backend three ways: API Gateway with Lambda, Flask on EC2, and Docker on ECS Fargate. Compared cost, scaling and effort.
- **Result:** Recommended serverless.
- **Reflection:** Build small and compare before committing. Data beats opinions.

> "In a cloud project at RMIT, instead of guessing how to deploy our backend, we deployed it three ways: Lambda with API Gateway, Flask on EC2, and Docker on ECS Fargate. We compared cost, scaling and effort, and I recommended serverless. That's how I like to make decisions: try small, compare, then commit."

---

## Things you must NOT claim

- Power BI, React or TypeScript experience
- Any Azure certification
- A RAG project
- Accuracy numbers for the gesture classifier
- Bedrock, Textract, Amazon Q, Kendra, EMR, EKS, CloudFormation or Jenkins experience
- Detail about Focus Bear work you haven't confirmed

---

## Before Monday checklist

- [ ] Confirm AZ-900: started or finished
- [ ] Confirm 485 length: 2 or 3 years
- [ ] Confirm full-time from 16 November is allowed on your student visa
- [ ] Fill in your real reason for leaving AWS (question 9)
- [ ] Optional: start a Microsoft Learn Power BI module
- [ ] Check the spelling of the recruiter's name (Khow) on LinkedIn
- [ ] Practise questions 1, 2 and 4 out loud with a timer
- [ ] Do one practice run Monday morning, not after the exam
- [ ] Phone charged, quiet room, CV and JD open
