Based on Nina-client-briefs.md

Case 1 – Retail Customer Emotion Analysis
Client Summary

A large retail chain wants to use existing in-store CCTV cameras to analyze customers' facial expressions and body language in real time. The AI estimates shoppers' emotional state and identifies individuals who may be susceptible to impulse purchases. When this occurs, personalized discounts are immediately displayed on nearby screens without customer awareness or human intervention.

First-pass Classification

Prohibited AI (Article 5)

Why

The proposed system combines emotion recognition with behavioral manipulation. It infers customers' emotional state and uses that information to influence purchasing behavior without transparency or meaningful human oversight. This raises concerns under the AI Act's prohibited practices relating to emotion recognition, manipulative AI, and exploitation of individuals' psychological vulnerabilities.

Proposed Architecture
Component	Description
Business trigger	Customer enters the retail store.
AI behaviour	Analyzes facial expressions and body posture to infer emotional state and purchasing susceptibility.
Inputs	Live CCTV video streams.
Human review	None before promotional content is displayed.
Output	Immediate personalized discount displayed on digital signage.
Role Map
Role	Entity
Provider	AI software vendor developing the emotion recognition platform.
Deployer	Retail chain operating the stores.
Third-party vendor	Cloud infrastructure and computer vision providers (if applicable).
Compliance Implications

Because the proposed functionality falls within prohibited AI practices, there is no compliance pathway under the AI Act.

Consulting Decision

-> Deny and Redesign

The proposed solution should not be deployed in its current form, as it falls within prohibited AI practices under the EU AI Act. There is no compliance pathway that would make this use lawful through additional documentation or governance alone. Instead, the client should redesign the solution to remove emotion recognition and manipulative behavioral targeting. A compliant alternative would be to use anonymized or aggregated analytics—such as store traffic, purchase history, or contextual promotions—to improve customer experience without inferring emotional states or exploiting psychological vulnerabilities.

Case 2 – AI Resume Screening
Client Summary

A recruitment company wants an AI system to rank job applicants based on resume content, years of experience, and relevant keywords. Recruiters review only the ten highest-ranked candidates, while all remaining applicants receive an automatic rejection without further human review.

First-pass Classification

High-risk AI (Annex III – Employment)

Why

The AI directly influences recruitment decisions within the employment domain, an Annex III high-risk area. Although a recruiter reviews the top-ranked applicants, candidates excluded by the AI receive no meaningful human assessment, making the AI's output determinative for employment opportunities.

Proposed Architecture
Component	Description
Business trigger	Job application submitted.
AI behaviour	Scores and ranks resumes using structured and unstructured candidate information.
Inputs	CVs, work experience, education, keywords.
Human review	Limited to the highest-ranked applicants only.
Output	Candidate ranking and automatic rejection of lower-ranked applicants.
Role Map
Role	Entity
Provider	Recruitment AI platform provider.
Deployer	Recruitment company using the platform.
Third-party vendor	LLM or ML infrastructure provider (if applicable).
Compliance Implications

The system would require the full set of applicable high-risk obligations, including risk management, technical documentation, logging, transparency, human oversight, and post-market monitoring. The current level of oversight appears insufficient because rejected candidates are never reviewed by a human.

Consulting Decision

-> Approve with Controls

The proposed system may proceed only if the client implements the governance and compliance controls required for high-risk AI systems. These include establishing a documented risk management process, maintaining technical documentation and system logs, ensuring training and testing data are appropriately governed and assessed for bias, and implementing meaningful human oversight so that hiring decisions are not based solely on AI rankings. The organization should also prepare conformity documentation, define post-market monitoring procedures, and ensure recruiters can review and override AI recommendations before any employment decision is finalized. Deployment should only occur once these controls are operational and documented.

Case 3 – Customer Service Chatbot
Client Summary

An electronics retailer wants to deploy an AI chatbot on its website and mobile application to answer routine customer service questions. Conversations that exceed the chatbot's capabilities are transferred to a human support agent.

First-pass Classification

Limited Risk – Transparency Obligations

Why

The chatbot interacts directly with customers and generates conversational responses. Users must be informed that they are communicating with an AI system, and escalation to human support should remain available.

Proposed Architecture
Component	Description
Business trigger	Customer initiates support conversation.
AI behaviour	Answers routine support questions and determines whether escalation is required.
Inputs	Customer chat messages and order information.
Human review	Human agent takes over complex conversations.
Output	AI-generated customer support responses.
Role Map
Role	Entity
Provider	Chatbot software provider.
Deployer	Electronics retailer.
Third-party vendor	LLM provider and hosting platform.
Compliance Implications

The retailer should ensure customers are clearly informed that they are interacting with AI and maintain appropriate escalation paths to human support.

Consulting Decision

-> Approve with Conditions

The project may proceed provided that transparency requirements are implemented and users are clearly informed when interacting with the AI system. The retailer should ensure that AI-generated responses are clearly distinguishable from human communications and maintain an effective escalation process so customers can easily reach a human agent whenever necessary. Regular monitoring of chatbot performance and clear user guidance will help ensure safe and compliant deployment.

Case 4 – Bakery Demand Forecasting
Client Summary

A bakery chain wants to use AI to forecast daily production quantities based on historical sales data. Managers remain responsible for deciding how much inventory to produce and may modify the AI's recommendations before placing orders.

First-pass Classification

Minimal Risk

Why

The AI supports internal operational planning and inventory optimization. It does not make decisions affecting individuals' rights or access to services, and managers retain full authority over production decisions.

Proposed Architecture
Component	Description
Business trigger	Daily production planning.
AI behaviour	Forecasts product demand based on historical sales patterns.
Inputs	Historical sales data and seasonal trends.
Human review	Store manager reviews and adjusts recommendations.
Output	Suggested production quantities.
Role Map
Role	Entity
Provider	Forecasting software provider.
Deployer	Bakery chain.
Third-party vendor	Cloud analytics provider (if applicable).
Compliance Implications

No specific AI Act obligations apply. However, the bakery should continue to comply with any applicable GDPR or commercial obligations if personal or customer data is processed.

Consulting Decision

-> Approve

The proposed system represents a low-risk internal decision-support tool that assists operational planning without producing decisions that have legal or similarly significant effects on individuals. The bakery may proceed with deployment while maintaining standard governance practices, appropriate data management, and periodic performance reviews to ensure forecast quality and business reliability.
