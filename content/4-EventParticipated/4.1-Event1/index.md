---
title: "AWS Vietnam Community Day - May 2026"
date: 2026-05-23
weight: 1
chapter: false
draft: false
pre: "<b>4.1.</b> "
---

# Reflection Report on “AWS Vietnam Community Day – May 2026”

## Event Information

- **Event name:** *AWS Vietnam Community Day – May 2026*
- **Date attended:** *May 23, 2026*
- **Location:** *26th Floor, Bitexco Financial Tower*
- **Organizer:** *FCAJ - First Cloud AI Journey*
- **Attendance format:** *In person*

## Purpose of the Event

- To provide updates on emerging trends in **Generative AI, Agentic AI, and application architecture on AWS**.
- To share practical experience in designing, deploying, and operating AI systems in enterprise environments.
- To introduce methods for optimizing **performance, cost, security, and reliability** for applications through Amazon CloudFront.
- To help attendees understand the roles of **context engineering**, multi-agent systems, guardrails, and techniques for managing the non-deterministic behavior of large language models.
- To create opportunities to learn from real-world projects, hackathons, and product development experiences under time constraints.
- To connect students, engineers, and members of the AWS technology community in Vietnam.

## List of Speakers

- **Tinh Truong** - Platform Engineer, GoTymeX
- **Pham Ng Hai Anh** - G-AsiaPacific Vietnam, AWS Community Builder
- **Nguyen Tuan Thinh** - DevOps Engineer, First Cloud AI Journey
- **Team VIB** - Presentation on the UTMorpho project at LotusHacks 2026
- **Dao Duc** - Solution Architect, Cloud Kinetics
- **Cat Vy** - Senior Business Systems Analyst, VPBank

## Key Highlights

### 1. Context Is Everything – The Importance of Context When Working with AI

The presentation emphasized that modern AI models are already highly capable, but the quality of their results still depends greatly on how users provide **context**. Answers that go in the wrong direction, are overly verbose, or overlook important requirements are not always caused by weak models. In many cases, the input does not clearly describe the goals and constraints.

Good context should include:

- **Goal:** The final result that needs to be achieved.
- **Situation:** Whether the user is a student, a beginner, or a member of a real-world project.
- **Constraints:** Technology, budget, timeline, style, and output format.
- **Relevant information:** Code, documents, examples, requirements, and supporting evidence.

The presentation also identified three common mistakes:

- Providing all documents, images, and notes at once, causing important information to be buried under irrelevant data.
- Repeating information that the AI can already identify from the provided materials without explaining what needs to be changed or solved.
- Giving overly general requests without clear criteria for evaluating the result.

The key message was that **context quality is more important than context quantity**. AI usage is evolving from single prompts toward systems that can store and retrieve context and retain useful information over time. A simple workflow can be described as: **Store → Retrieve → Generate → Learn**.

### 2. Friendly AI Assistant With Amazon Quick

This session introduced the use of Amazon Quick Suite to support business users in completing their daily tasks. Common difficulties include gathering information from multiple sources, relying on experts to analyze specialized data, and repeatedly performing time-consuming manual tasks.

Amazon Quick Suite was presented as a unified environment that combines:

- Internal company data, user-uploaded files, databases, and data warehouses.
- External knowledge, web search, and models available through Amazon Bedrock.
- Multiple data connectors and actions integrated with third-party applications.
- Dashboards, chat, research, insights, and automation flows.
- Governance mechanisms such as access control, guardrails, data security, and regulatory compliance.

The demonstrated use case was a **PM Assistant** that could automatically create meeting minutes, send emails to stakeholders, and schedule the next meeting. This showed that AI can do more than answer questions; it can also directly participate in business workflows and perform actions according to predefined processes.

### 3. From Edge to Origin – CloudFront as Your Foundation

The presentation showed that Amazon CloudFront is not only a CDN service but can also serve as a foundational layer in front of an application to optimize **cost, security, reliability, and performance**.

#### Cost Optimization and Control

The session introduced a flat-rate pricing model that helps customers predict costs more easily than a fully usage-based pricing model. These plans can combine multiple components, including CDN, WAF, DDoS protection, DNS, logging, and storage benefits.

CloudFront also reduces origin load through caching, request collapsing, and compression. When fewer requests reach the origin, the system can reduce resource usage across Load Balancers, EC2 instances, and databases.

#### System Security

The security capabilities discussed included:

- Distributing DDoS protection across edge locations and blocking unwanted traffic close to its source.
- Integrating AWS Shield and AWS WAF.
- Using HTTPS, TLS, and mutual TLS for use cases that require two-way authentication.
- Hiding origins by using VPC Origin, Origin Access Control, or firewall rules that only allow traffic from CloudFront.
- Adding a secret custom header to reduce direct access to the origin.
- Controlling access based on geographic location.
- Protecting content with Signed URLs or Signed Cookies.

#### Improved Reliability

CloudFront can continue serving cached content when the origin temporarily becomes unavailable, use origin failover to route traffic to a backup origin, and provide custom error pages to maintain a user-friendly experience.

#### Improved Performance

The techniques introduced included multi-layer caching architecture, HTTP/3, compression, persistent connections to origins, and edge logic processing through CloudFront Functions or Lambda@Edge. These mechanisms help reduce latency, decrease the number of connections to the origin, and improve application response times.

### 4. UTMorpho – Building an AI Product in 36 Hours

This session shared the journey of building **UTMorpho** within 36 hours at LotusHacks 2026. The idea came from a practical problem: many AI tools can generate user interfaces, but whenever users need to modify a specific detail, they must enter another prompt. Re-prompting can unexpectedly change colors, spacing, layouts, and increase token consumption.

UTMorpho was developed with the following goals:

- Generate a functional UI component from a prompt instead of only producing a static mockup.
- Allow users to directly edit text, colors, spacing, and layout on the canvas.
- Change only the selected component and minimize design drift.
- Use smart diffing so that small changes consume only a corresponding number of tokens.
- Support exporting the result to React.

The development process was divided into several stages: setting up the repository and AWS access, building the initial backend, integrating AI, developing the inline editor, synchronizing state, resolving errors, cutting unnecessary features, completing the demo, and rehearsing the pitch.

The key lessons included:

- Strong ideas often come from problems that the development team has personally experienced.
- Under time constraints, it is important to protect the main demo flow instead of trying to complete too many features.
- Trust and effective teamwork can be more important than building a complicated process.
- Token usage and AI costs should be treated as product design constraints.
- AI can be viewed as a supporting team member rather than simply a library called through an API.

### 5. Non-Determinism of “Deterministic” LLM Settings

This session explained how large language models generate results one token at a time through logits, softmax, and parameters such as **Temperature, Top-P, and Top-K**.

In theory, when `temperature = 0`, the model selects the token with the highest probability and is expected to produce the same result for the same prompt. However, in real deployment environments, this configuration does not guarantee that the system will be completely deterministic.

The main causes discussed included:

- Floating-point operations on GPUs can produce very small differences depending on the parallel execution order.
- Small differences in logits can change the selected token.
- Providers often combine requests from multiple users into batches to optimize GPU usage.
- Batch composition and inference optimization techniques can cause results to vary between runs.

This affects applications that require structured output, regression testing, prompt evaluation, benchmarking, and other high-risk systems.

Several mitigation strategies were introduced:

- Run the same request multiple times and use majority voting.
- Restrict the output space by using JSON mode, function calling, schemas, or grammars.
- Validate the output before passing it to the next processing step.
- Design systems with the assumption that AI output is probabilistic.
- Self-host models when deeper control over the inference infrastructure is required.
- Perform repeated testing across different scenarios and datasets.

The key lesson was that `temperature = 0` only removes part of the randomness in the sampling process; it does not eliminate every source of output variation.

### 6. Enterprise-Grade Multi-Agent System – Startup Credit Scoring

This presentation used startup credit scoring as a use case to illustrate the differences between single-agent and multi-agent systems.

Traditional credit scoring systems often rely on long financial histories, collateral assets, predictable revenue, and standardized reporting formats. Startups, however, usually have short operating histories, no established credit records, and assets that are mainly based on intellectual property, teams, and growth potential. Their data is also distributed across several domains, including finance, market conditions, team quality, and traction.

A single agent may face several limitations:

- Excessively large context.
- Diluted domain expertise.
- No mechanism for cross-checking and challenging assumptions.
- A single point of failure.

The proposed solution was a **virtual credit committee** consisting of multiple specialized agents:

- **Manager Agent:** Coordinates the entire workflow.
- **Financial Analyst:** Analyzes cash flow, burn rate, and unit economics.
- **Market Analyst:** Evaluates the market, competition, and timing.
- **Team Evaluator:** Assesses founders, team composition, and experience.
- **Risk Assessor:** Analyzes risks and mitigation measures.
- **Compliance Agent:** Verifies policies and regulatory requirements.

The agents can run in parallel, challenge one another's results, and produce outputs such as credit scores, risk ratings, confidence levels, and audit trails.

To move from a proof of concept to an enterprise-grade system, the presentation proposed six groups of considerations:

- **Security:** Authentication, encryption, and secrets management.
- **Data Governance:** PII handling, data residency, and audit logging.
- **Network:** VPC isolation, private endpoints, and zero-trust principles.
- **Operations:** Monitoring, incident response, and disaster recovery.
- **Human Factors:** Training, runbooks, and knowledge transfer.
- **Compliance:** Industry regulations, internal policies, and certifications.

Guardrails should be implemented throughout the system:

- **Input guardrails:** Content filtering, PII detection, prompt injection prevention, and rate limiting.
- **Processing guardrails:** Token budgets, timeouts, model selection, and tool permissions.
- **Output guardrails:** Validation, hallucination detection, bias checking, and compliance verification.

The reference deployment flow used containers, Amazon ECR, Amazon Bedrock, API Gateway, VPC, IAM, AWS Secrets Manager, CloudWatch, X-Ray, and Infrastructure as Code. The implementation should be divided into foundation, integration, pilot, and scale phases.

## What I Learned

### Working Effectively with AI

- A good prompt should clearly define the goal, context, constraints, and success criteria.
- Not all available data should be passed to the model; only the most relevant information should be retrieved.
- Memory and retrieval help AI systems maintain context more effectively across multiple interactions.
- LLM output should be treated as probabilistic and must go through validation.

### Designing AI Systems

- A single agent is suitable for linear workflows and narrow domains of expertise.
- Multi-agent systems are more suitable when a problem involves multiple knowledge domains, requires cross-checking, and needs auditability.
- Guardrails should be designed for the input, processing, and output stages.
- Security, governance, observability, and compliance should be considered from the beginning.
- Token usage, latency, and inference costs are important architectural constraints.

### AWS Architecture and Operations

- CloudFront can be used as a protection and optimization layer in front of an application.
- Caching, request collapsing, and edge computing help reduce origin load.
- OAC, VPC Origin, WAF, Shield, TLS, and Signed URLs support a layered security architecture.
- Monitoring, audit trails, IAM least privilege, and Infrastructure as Code are essential components of a production system.

### Product Development and Teamwork

- Projects should begin with a real problem instead of trying to create an overly ambitious idea.
- Under time constraints, teams should prioritize the MVP and the most important demo flow.
- Team synchronization and clear task allocation help accelerate implementation.
- Teams should be prepared to remove features to ensure that the core product remains stable.

## Application to the AI AWS Architecture Reviewer Project

### Improving Context for the Analysis Process

- Add metadata to architecture images, such as workload type, system goals, deployment environment, and priority requirements.
- Send only the documents and rules relevant to the architecture being reviewed to Amazon Bedrock.
- Clearly define an output schema that includes detected services, Well-Architected findings, security risks, cost estimates, and recommendations.
- Store useful information for each `reviewId` to support retrieval and history tracking.

### Expanding Toward a Multi-Agent Architecture

In an extended version, the system could be divided into specialized agents:

- An agent for detecting AWS services in the diagram.
- An agent for assessing the AWS Well-Architected Framework.
- An agent for analyzing security and compliance.
- An agent for estimating and optimizing costs.
- An agent for consolidating results and generating the final report.

A manager agent could coordinate the agents, validate their results, and handle cases where different agents produce conflicting assessments.

### Improving Website Security and Performance

- Place CloudFront in front of the S3 frontend and the appropriate APIs.
- Use OAC to restrict direct access to the S3 bucket.
- Combine AWS WAF with rate limiting to filter abnormal requests.
- Enable HTTPS, compression, and HTTP/3 where appropriate.
- Consider using Signed URLs for reports that should only be downloadable within a limited time.
- Monitor access logs, WAF logs, and CloudWatch metrics to detect incidents.

## Experience at the Event

Attending **AWS Vietnam Community Day – May 2026** allowed me to explore different perspectives, ranging from communicating effectively with AI to designing cloud architecture and introducing AI systems into enterprise environments.

### Highly Connected Knowledge

Although the sessions covered different topics, they were clearly connected. A strong AI system must begin with accurate context, manage model non-determinism, use an appropriate agent architecture, and be protected by security, governance, and monitoring layers.

### Multiple Real-World Use Cases

The case studies on the PM Assistant, UTMorpho, and startup credit scoring helped me understand how technical knowledge can be transformed into valuable products. The sessions did not only introduce AWS services; they also discussed the problems, architectural decisions, limitations, and practical implementation approaches.

### A New Perspective on AI

I realized that AI is not a component that can operate reliably with only a single prompt. Building a trustworthy AI application requires context management, output validation, guardrails, logging, testing, and mechanisms for handling changing results.

### Lessons for Project Development

The experience of building UTMorpho in 36 hours showed that identifying the right problem and focusing on the main workflow are more important than the number of features. This is a valuable lesson for group projects, especially during the final demo preparation and presentation stages.

> Overall, the event provided me with technical knowledge, product development experience, and a practical mindset for deploying AI systems. The topics of context engineering, CloudFront, LLM non-determinism, multi-agent architecture, and enterprise guardrails can be directly applied to the completion of the AI AWS Architecture Reviewer project.
