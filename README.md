# Threat-Modeling-Risk-Assessment-for-a-SaaS-Product
This repository contains the DFD and Risk Register of Halisans Technology SaaS Product

Student Login Portal | Threat Modeling & Risk Assessment

Analyst: Funmilola Folarin · Status: Production security audit
# Executive summary
This repository documents a security assessment of a proposed Student Login Portal. Students can register, log in, and view their own academic profiles. The assessment uses an OWASP Threat Dragon data flow diagram (DFD), STRIDE threat identification, a risk register, security control mapping, and a risk treatment plan.

# Application scope
•	External entity: Student using a web browser


•	Three application processes: Student Registration, Student Login, View Student Profile


•	Data store: Student Database containing student accounts, password hashes, and academic profile records


•	Known communication: Student/browser ↔ application via HTTPS/TLS


•	To confirm with developers: backend-to-database protocol, database hosting, session mechanism, and authorization enforcement


•	Out of scope: administrator functions, profile data import, penetration testing, and live production systems

# Objectives
1.	Translate the developer brief into a Level 1 DFD with exactly three application processes.
2.	Label data flows and known protocols, and document.
3.	Identify and justify the trust boundaries.
4.	Apply STRIDE to identify plausible threats.
5.	Score likelihood and impact (1–5), then document controls and treatment actions.
   
# Assessment workflow
Developer brief → Threat Dragon DFD → STRIDE findings → Risk register → Control mapping → Risk treatment plan
Stage	
## What I did	Evidence
Model	Created DFD and labeled data flows / boundaries	[threat-model/](threat-model/)


Threats	Identified threats using STRIDE	Threat Dragon report in threat-model/


Risk	Scored each threat and recorded justification	[risk-assessment/](risk-assessment/)


Controls	Mapped mitigations to applicable controls	[control-mapping/](control-mapping/)


Treatment	Assigned proposed actions, owners, and verification criteria	[risk-treatment/](risk-treatment/)


Findings summary — complete after assessment


ID	STRIDE category	Threat summary	Risk score	Proposed action
T-01	[Category]	[Finding]	[1–25]	[Action]


T-02	[Category]	[Finding]	[1–25]	[Action]


T-03	[Category]	[Finding]	[1–25]	[Action]


Risk scoring: Likelihood (1–5) × Impact (1–5). Explain both ratings in the risk register. Scores are scenario judgments, not measured exploit probabilities.


# Deliverables
1.	OWASP Threat Dragon report and model — add exported report PDF and model JSON to threat-model/.
2.	Threat Risk Register — complete risk-assessment/threat-risk-register.csv.
3.	Control Mapping — complete control-mapping/control-mapping.csv using verified control references.
4.	Risk Treatment Plan — complete risk-treatment/risk-treatment-plan.csv.
