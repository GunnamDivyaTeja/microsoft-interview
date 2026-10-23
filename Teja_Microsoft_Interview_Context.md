# Teja Gunnam: Context for Microsoft Interview Prep

Last updated: 23 October 2026 (after first mock recruiter screen)

This file holds everything needed to help Teja prepare for his Microsoft Cloud Solution Architect (Early in Profession) interview process. Read it fully before helping.

---

## 1. How to work with me

• No em dashes or en dashes anywhere. Use plain hyphens (-) only.
• Use round bullet points (•) for lists.
• Keep it concise. Simple, plain English. No elaborate or "AI-sounding" phrasing.
• Lead with the verdict or answer first, then the detail.
• Give honest assessments, not encouraging ones. Tell me when an answer is weak.
• Never put aspirational or forward-looking skills on my CV or claim things I have not done. If I have not used something, say so and suggest an honest way to frame it.
• Answers I give in interviews must sound like a real person talking, not a script.

---

## 2. Who I am

• Name: Divya Teja Gunnam (goes by Teja)
• Location: Truganina / Werribee area, Melbourne, VIC
• Phone: +61 481 576 074
• Email: gunnamdivyateja@gmail.com
• LinkedIn: linkedin.com/in/teja-gunnam-2a92a415a
• Study: Final semester, Master of Artificial Intelligence, RMIT University. Graduating December 2026. Final exams in late October 2026 (one on Monday 26 Oct afternoon).
• Undergrad: Bachelor of Technology, Electronics and Communication Engineering, Bennett University (2021)
• Certification: AWS Certified Solutions Architect - Associate
• Visa: Student visa (subclass 500) now, with limited work hours during study. Will apply for the Temporary Graduate visa (subclass 485) as soon as exams finish, which gives full work rights (Bridging Visa A with full work rights while it is processed). Plan is to apply for PR after that.
• 485 length: standard Post-Higher Education Work stream for a coursework Master's is 2 years. Some nationalities get longer. CONFIRM 2 or 3 years on Home Affairs before saying a number.
• Available to start full time: 16 November 2026 (fits Microsoft's November to December target start). CONFIRM this matches student visa conditions after the course ends.
• Long-term goal: AI engineering career, and eventually building my own AI company.

---

## 3. Work experience (facts only, safe to use)

### Cloud Support Engineer, Amazon Web Services (2022 - 2024)
• Diagnosed and fixed production issues for enterprise customers across EC2, ECS, Lambda, Redshift and VPC under SLA, using logs, metrics and network traces.
• Part of the analytics services team covering Redshift, QuickSight and managed Grafana and Prometheus.
• Handled high-severity escalations with Technical Account Managers and service teams, keeping customer stakeholders updated in plain language. Kept clear running notes for handover.
• Built data pipelines with Solutions Architects across AWS and Azure, moving customer data from S3 through Glue and Athena into Redshift for reporting and dashboards.
• Reviewed customer environments for cost and performance and recommended changes that cut compute spend without hurting performance.
• Key story: a customer pipeline kept failing. It sat outside my service area. I traced it to a cross-account VPC networking issue (including IAM access) and fixed it end to end instead of letting it bounce between three teams.
• Wrote Python and Bash tooling to automate repetitive diagnostic checks. Debugged customer Terraform deployments broken by provider changes.
• Wrote knowledge-base articles and ran internal training that shortened diagnosis time for the team.

### Machine Learning Engineer Intern, Focus Bear (Sep 2026 - present)
• Remote, part-time, distributed team across timezones.
• Working on AI-based distraction blocking features for the Focus Bear productivity app. (I have not yet given detailed specifics of what I built. Ask me before adding detail.)

### Pipeline Assistant Technical Director, DNEG (2021 - 2022)
• Built Python automation for VFX pipelines on Dune and Tenet (credited on Dune), working directly with the artists who used it.
• Triaged production-blocking faults through Jira under hard deadlines.

### Part-time roles (2025 - present)
• Shiperoo (e-commerce fulfilment, pick and pack and inbound, now permanent part-time), Spotlight (inbound, about 5 months), Foodbiz (wholesale food distribution, Administration Officer). At Foodbiz I automated the weekly payroll calculation in Excel, removing a recurring source of errors.

---

## 4. Projects (facts only)

### Halo Voice: AI voice receptionist (personal, live)
• Live at halo-voice.divyatejagunnam.workers.dev
• AI receptionist for small businesses on Cloudflare Workers and the OpenAI Realtime API, with browser-to-model WebRTC audio.
• Security: short-lived session tokens so the API key never reaches the browser, per-IP rate limiting, call time limits.
• First version used LiveKit. I rebuilt it after realising it carried media-routing infrastructure a two-person call did not need, cutting latency and running cost.
• Bug story: the agent started inventing business names. I added event logging, found a request that was quietly overwriting the session config, and fixed it by deleting code.
• Deploy story: deploys kept failing. I traced it to a mismatch between two hosting products, fixed it in config, and wrote the exact error in the commit message for the next person.
• Note: built with heavy AI coding assistance (Claude Code). Be honest about this if asked.

### Cloud-Native Music Subscription App (RMIT course project, team of four)
• Deployed the same Python backend three ways: API Gateway with Lambda, Flask on EC2, and Docker on ECS Fargate via ECR. Compared cost, scaling and effort, and recommended serverless.
• Designed the DynamoDB schema (composite key, local and global secondary indexes so searches are Queries, not Scans).
• Artwork in a private S3 bucket behind pre-signed URLs. IAM roles scoped per service.

### Automated Curriculum Processing Engine (RMIT capstone, in progress)
• Cloud and deployment lead in a five-person team building an LLM-based document processing tool for an education client (Spectrum Tuition).
• Own hosting, deployment and workflow automation across AWS, Supabase, PostgreSQL, Vercel and n8n, with Claude and Gemini APIs.

### UAV Gesture Classifier (RMIT Deep Learning)
• PyTorch classifier for drone marshalling hand signals, ImageNet-pretrained MobileNetV2 with transfer learning, trained on AWS SageMaker.
• Noticed results looked too good, traced it to data leakage (same people in train and test), moved to person-independent grouped cross-validation.
• Do NOT quote any accuracy numbers. The assignment is not finished.

### Multi-Agent Workflow System (personal)
• AI agents on LangGraph and n8n that handle stages of a business process, with human approval before anything goes out.

---

## 5. Things I must NOT claim

• No clinical coding project (not started).
• No C++ port (not started).
• No RAG project. I have not built one.
• No accuracy numbers for the gesture classifier.
• No Power BI, React or TypeScript.
• No Azure certifications. Azure experience is limited to data pipeline work at AWS.
• No Bedrock, Textract, Amazon Q, Kendra, EMR, EKS, CloudFormation or Jenkins experience.

---

## 6. The Microsoft role

• Title: Cloud Solution Architect (Early in Profession)
• Link: https://apply.careers.microsoft.com/careers/job/1970393556997801?domain=microsoft.com&hl=en
• Full JD saved in this repo: "Job Description - CSA Early in Profession.pdf"
• Job number 200055607. Posted 24 Sep 2026. Profession: Customer Success. Individual contributor, full time.
• Locations: Sydney, Melbourne, Brisbane, Canberra or Perth. 3 days a week in office. Travel under 25%.
• Target start date: November to December 2026. Applications reviewed on a rolling basis, process expected to move quickly.
• JD wants 2 to 4 years of experience. Mine: about 3 years (DNEG 1 year, AWS 2 years).
• JD phrases to hit: "translate technical concepts into customer outcomes", "customer and business outcome mindset", "curiosity about AI", "growth mindset and learning agility", "build or automate simple solutions", "security, resilience and AI", proof of concept / MVP / rapid prototypes to show ROI, Copilot and AI scenarios.
• Power BI is a named skill I do not have. Honest framing: dashboards in QuickSight and Grafana, SQL and Python for data work, Power BI is new to me but the same idea.
• Applied through the Microsoft careers portal and was shortlisted for a screening call.
• Program: designed to work alongside experienced architects and technical specialists.

### Responsibilities (summary)
• Listen actively, respectfully challenge customers and partners, build trust.
• Map architecture and digital transformation solutions to customer business outcomes.
• Support delivery through Value-Based Deliverables (VBDs), training, technical validation and advisory.
• Help with change management, deployments and long-term adoption.
• Guide customers toward secure, resilient, AI-enabled, cost- and performance-optimised architectures.
• Manage business and technical risk, escalate and remove blockers.
• Build relationships with Technical Decision Makers (TDMs).
• Support partners with proofs of concept, pre-sales and offerings.
• Contribute to presentations, IP and events (Tech Connect, Build, Ignite).
• Build readiness in security, resilience and AI.

### Required qualifications
• Bachelor's or Master's in Computer Science, Engineering, IT or related, plus 2+ years (or 2-4 years) related experience in cloud/infrastructure, IT consulting/support, systems admin, software development/support or architecture.

### Preferred
• Curiosity about AI, SQL, Power BI and Python basics, cloud fundamentals (Azure certs or hands-on), building or automating simple solutions, modern apps and APIs, security and governance awareness, problem solving, customer focus, clear communication, growth mindset.

### Microsoft culture keywords
• Growth mindset ("learn-it-all, not know-it-all"), customer obsessed, One Microsoft, diversity and inclusion, making a difference.

---

## 7. The screening call

• When: Monday 26 October 2026, 8:00 PM - 8:15 PM Sydney/Melbourne time (AEDT)
• Who: Khow, recruiter (check exact spelling of her name)
• Format: 15-minute recruiter screen. Not technical. Checks background, motivation, communication and logistics.
• I have a final exam the same afternoon.
• Message sent / planned to Khow on LinkedIn:
  Subject: Cloud Solution Architect (Early in Profession) - Teja Gunnam, 26 Oct
  "Hi Khow, Thank you for shortlisting me for the Cloud Solution Architect (Early in Profession) role. I'm really looking forward to our chat. I appreciate you making time for the evening slot. I have a final exam on Monday afternoon, so it works much better for me. Talk to you soon. Kind regards, Teja Gunnam"

### Plan for a 15-minute call
• Tell me about yourself: 45-60 seconds.
• Other answers: 30-60 seconds each.
• Questions at the end (2 to 3): which solution area / team, next steps and timeline, any advice for the next round.

### Polished answers
Full polished answers from the first mock are in "Recruiter_Screen_Answers.md" in this repo. Short version below.

### Answers drafted so far
• Tell me about yourself (4 beats, about 50 seconds): Master's at RMIT finishing December. About three years of work: DNEG Python automation, then two years at AWS working directly with enterprise customers and building data pipelines with Solutions Architects. AWS certified. Now ML engineering intern at Focus Bear and built my own live AI voice receptionist. Enjoyed the customer side at AWS most, which is why CSA appeals. Do NOT say "entry point" or "a good team".
• Why Microsoft / why CSA (3 beats): liked the customer side at AWS and CSA is that as the whole job. Microsoft is where enterprise AI adoption is happening (Azure OpenAI, Copilot), which fits my AI plus cloud background. The Early in Profession program means learning from experienced architects with real customers. Avoid flattery like "the most intelligent minds".
• AWS to Azure: most hands-on work is AWS, but not starting from zero. Worked on customer pipelines across AWS and Azure at AWS. Core ideas carry across: VPC to VNet, IAM to Entra ID, Lambda to Azure Functions. Real differences in identity and governance. AZ-900 path on Microsoft Learn (CONFIRM: started or finished, say only what is true). Learned AWS on the job and got certified. Do not say "only the names differ".
• Customer story (STAR plus reflection, about 70 seconds): cross-account pipeline. S3 data encrypted with KMS in one account, Redshift in a private VPC in another account, Access Denied errors. Got on a call, sent a written summary, owned it across IAM, S3 and networking even though my team only covered analytics, found the cross-account IAM role and network rules were misconfigured, stayed on a call while they applied the fix, pipeline unblocked. Reflection: customers don't care which team owns a problem. Technical notes: a private VPC uses an S3 gateway VPC endpoint or NAT, NOT an internet gateway. Cross-account SSE-KMS needs bucket policy, KMS key policy (kms:Decrypt) and the IAM role, with a customer managed key. Only mention KMS or the endpoint if that was really part of the fix.
• Explaining technical things simply: plain-language updates during high-severity escalations, knowledge-base articles, internal training.
• AI: Halo Voice live in production, and the LiveKit rebuild showing I design for what the customer actually needs.
• Mistake / learning: the data leakage catch. Use "growth mindset" naturally.
• Start date and work rights (lead with the date): "I can start full-time from 16 November, so that lines up with your intake. I'm on a student visa now, and once exams finish I'll apply for the 485, which gives full work rights for [2 or 3] years, with a bridging visa with full work rights while it's processed. Longer term I'm planning to stay in Australia and go for PR." If asked about sponsorship: "Not for the next few years. The 485 gives me full work rights, and I'm working toward PR."
• Salary: ask for their band and the full package first (base, super, bonus, stock). Fallback only if pushed: "around $105 to $115k base plus super, but flexible depending on the full package." Always say "plus super". Never quote total comp.
• Salary research: Glassdoor says about $100-110k base for CSA with 1-3 years. Levels.fyi Microsoft Solution Architect I in Australia, base only: fresh hires $104k (0 yrs) and $111k (1 yr), internal people $109k to $119k, bonus roughly $15-27k plus some stock on top. Small, older sample.
• Other interviews: "Yes, early stages with a couple of companies for Cloud Engineer and Cloud Ops roles. But this one is my first choice because of the customer-facing side. If anything moves quickly elsewhere, I'll let you know." Don't name companies unless asked. Don't overstate.

### Mock 1 verdict (23 Oct)
• Likely to pass the screen. Background fits the JD. Sound honest and natural.
• Fix 1: lead with the point and land every answer on customers or outcomes, not on what I get.
• Fix 2: get facts exact (Azure course status, 485 length, 16 Nov start, salary range).
• Fix 3: practise out loud with a timer from beats, not a script. Intro about 50 seconds, customer story about 70 seconds.

---

## 8. The CV I submitted to Microsoft (exact text)

File: Teja_Gunnam_CV_Microsoft_CSA.docx / .pdf

```
Divya Teja Gunnam
Cloud Engineer | AWS Certified Solutions Architect | Master of AI
Melbourne, VIC • +61 481 576 074 • gunnamdivyateja@gmail.com • linkedin.com/in/teja-gunnam-2a92a415a

SUMMARY
Cloud engineer with two years at Amazon Web Services helping enterprise customers fix production problems and get more
from their cloud setup. Now finishing a Master of AI at RMIT and building AI applications of my own. I enjoy working out what
a customer actually needs, then helping design something secure, reliable and sensibly priced to get them there.

EXPERIENCE
Cloud Support Engineer, Amazon Web Services                                                     2022 - 2024
 • Worked with enterprise customers to diagnose and fix production issues across EC2, ECS, Lambda, Redshift and VPC, within
   agreed response times.
 • Handled high-severity escalations alongside Technical Account Managers and service teams, keeping customer
   stakeholders updated in plain language until systems were back up.
 • Reviewed customer environments for cost and performance, and recommended changes that cut compute spend without
   hurting performance.
 • Built data pipelines with Solutions Architects across AWS and Azure, moving customer data into Redshift for reporting and
   dashboards.
 • Fixed a broken customer pipeline outside my own service area by tracing it to a cross-account VPC networking issue, and
   resolved it end to end instead of passing it across three teams.
 • Wrote knowledge-base articles and ran internal training that shortened diagnosis time for the wider team.
Machine Learning Engineer Intern, Focus Bear                                                    Sep 2026 - Present
 • Machine learning work on a live productivity app, working remotely with a distributed team across timezones.
Pipeline Assistant Technical Director, DNEG                                                     2021 - 2022
 • Built Python automation for visual effects pipelines on Dune and Tenet (credited on Dune), working directly with the artists
   who used it.
Part-time roles, Shiperoo, Spotlight and Foodbiz                                                2025 - Present
 • Warehouse and administration work alongside full-time study. At Foodbiz I automated the weekly payroll calculation,
   removing a recurring source of errors.

SELECTED PROJECTS
Automated Curriculum Processing Engine, RMIT capstone with industry partner                     In progress
 • Cloud and deployment lead for a five-person team building an LLM-based curriculum processing tool for an education
   client. I own hosting, deployment and workflow automation across AWS, Supabase, Vercel and n8n.
Cloud-Native Music Subscription App, RMIT course project
 • Deployed the same backend three ways (Lambda with API Gateway, Flask on EC2, Docker on ECS Fargate), compared cost,
   scaling and effort, and recommended serverless. Designed the DynamoDB schema and kept artwork in a private S3 bucket
   behind pre-signed URLs.
Halo Voice, AI phone receptionist, live
 • AI receptionist for small businesses running on Cloudflare Workers and the OpenAI Realtime API. Built so the API key never
   reaches the browser, using short-lived session tokens, rate limits and call time limits.
UAV Gesture Classifier, RMIT Deep Learning
 • PyTorch classifier for drone hand signals. Caught a data leakage problem in the evaluation that was inflating the results,
   and fixed the testing method.

EDUCATION AND CERTIFICATION
Master of Artificial Intelligence, RMIT University, Melbourne                                   Expected Dec 2026
Bachelor of Technology, Electronics and Communication Engineering, Bennett University           2021
AWS Certified Solutions Architect - Associate, Amazon Web Services

SKILLS
Cloud: AWS (EC2, ECS, Fargate, Lambda, API Gateway, S3, DynamoDB, VPC, IAM, Redshift), Microsoft Azure, Cloudflare Workers, Docker, Terraform
AI: LLM applications (OpenAI, Anthropic and Gemini APIs), LangGraph, n8n, PyTorch, machine learning
Data and development: Python, SQL, REST APIs, Flask, PostgreSQL, dashboards (QuickSight, Grafana), Git, Linux
Security: IAM and least-privilege access, private storage with pre-signed URLs, short-lived credentials, network troubleshooting
Working with customers: Stakeholder communication, escalation management, technical documentation, training
```

Note: interviewers will ask about anything on this CV. The Microsoft Azure skill line refers only to the Azure data pipeline work at AWS.

---

## 9. Wider job search (current status)

Target roles: AI/ML engineering, cloud engineering, SRE and graduate roles in Melbourne. Salary positions used so far: $80-90k base for grad/consulting roles, $90-105k including super for associate cloud roles, $100-120k for mid-level AWS operations roles.

• Microsoft - Cloud Solution Architect (Early in Profession): shortlisted, recruiter screen 26 Oct, 8:00 PM AEDT.
• WSN (recruitment agency) - AWS Platform Operations Engineer, $100-120k, hybrid Melbourne, hiring starts Dec 2026: had a screening call with recruiter Bailey Wright. Good rapport. She will call in December. I will update her when my 485 visa is granted.
• REA Group - Associate Machine Learning Engineer (Richmond): an ML Team Lead at REA encouraged me to apply and said the role is engineering focused (coding, Python, software). I asked about referral / mentioning his name. CV tailored.
• Medibank - Cloud Engineer, AI & Data (Docklands): CV and cover letter tailored. Reaching out on LinkedIn to Ashwin K V (Cloud Tech Lead) and Indraneel Chavan (Engineering Manager).
• IMDEX - Cloud Engineer (senior-level role, long shot): applied, messaged recruiter Charlotte, she replied "Thank you, Teja".
• Insignia Financial - Associate Cloud Engineer: CV and cover letter tailored, application questions answered.
• Culture Amp - Associate Site Reliability Engineer: CV and cover letter tailored.
• BLOOMTECH (Japan, fully remote) - AI Engineer: CV tailored, messaging recruiter Yamada-san to check if Australia-based candidates are accepted and if Japanese is required.
• Others with tailored CVs earlier: Publicis Sapient (Early Careers Consultant, Data & AI), Maincode (Graduate Software Engineer), Deloitte (Engineering EOI, Forward Deployed Engineer), Adaptovate (Forward Deployed AI Consultant), KPMG, EY, HESTA, Shiperoo (IT side), Shield AI, CareGP, DiDi, Pluralis, Orica, Fusion5, Focus Bear.

---

## 10. What I want from this session

Help me prepare for the Microsoft process, starting with the 15-minute recruiter screen on 26 October, then the later interview rounds if I get through. This includes mock interviews, tightening my answers, Azure and CSA knowledge I need, and follow-up messages after each round.
