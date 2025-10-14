---
layout: post
title: AI Customer Stories
gh-repo: Shllomi/AI-Customer-Stories
gh-badge: [star, follow]
tags: [AI stories]
comments: true
mathjax: true
author: Shllomi Ezra
---
This repository provides various public stories on how organizations approach and implement AI. If you have a story to share, please create a  [pull request](https://github.com/Shllomi/AI-Customer-Stories)!

---

_**Financial Services & Capital Markets**_
------------------------ 

**Itaú Unibanco**    
Pix on WhatsApp is one of the first solutions connected to Inteligência Itaú and uses generative AI to interact with clients through WhatsApp and make day-to-day transfers in an automated and instant way.  
[Learn-More](https://www.itau.com.br/relacoes-com-investidores/noticias/inteligencia-itau-banco-lanca-nova-experiencia-para-clientes-com-ia-generativa/?lang=en)   

**S&P Global Market Intelligence, part of S&P Global**  
The credit analysts at S&P Global Market Intelligence are asked to answer questions and provide secondary analysis of industries and countries. Responses and analysis require synthesis of broad context from long documents (not just short snippets). The analysts need to prioritize retrieving and synthesizing the most relevant information among multiple relevant documents with similar titles (e.g. XX Industry Outlook). Furthermore, none of the "off the shelf" solutions were able to address the specific challenges of commentary articles, so S&P Global Market Intelligence needed a custom solution. AWS scientists built a custom Retrieval Augmented Generation (#RAG) solution powered by Amazon #Bedrock and Anthropic Claude Haiku to achieve the desired outcome. First, PDF documents were converted to markdown format using Amazon Textract with Layout mode. Documents were then chunked according to markdown section delimiters, to construct chunks with broad and complete context. Chunks were vectorized with #Titanv2 embeddings, and Amazon #OpenSearch queries weighted documents by semantic relevance and date to favor the latest commentaries. The custom pipeline achieved % top 10 accuracy in document retrieval, effectively generative comprehensive answers to broad research questions using the latest insights. The solution took days and weeks of manual document search, review, and synthesis down to minutes and seconds, saving valuable time for analysts.  
[Learn-More](https://www.youtube.com/watch?v=wY8M0uCYxL4)

 **Banco de Occidente**  
Banco de Occidente needed to improve the validation process of responses to the PQR (Preguntas, Quejas y Reclamos or in English: Questions, complains and claims) of its clients. The legacy workflow included a validation by sampling after communications were sent (vs. a complete analysis prior to sending every communication). The existing process was cumbersome, lengthy, and was driving down Net Promoter Score (NPS) due to response times and accuracy of responses. Banco de Occidente built an AI-powered assist for their level 2 support team. The intelligent tool empowers employees by validating responses, offering context-aware suggestions, and streamlining the complaint handling process. Powered by Amazon Bedrock leveraging Anthropic Claude Sonnet 3.5, the architecture employs a chain pattern that calls an LLM multiple times to evaluate the proposed response, generate corrections, and provide feedback to the collaborator on how to improve their proposed response based on internal communication rules evaluation. Furthermore, the solution is multi-modal as it validates the correct use of logos, handwritten signatures, social media, bank colors all associated with communication rules. Using the new GenAI powered solution, the evaluation process became 17.3x faster than the previous system, dramatically reducing response times and streamlining complaint handling workflows. Additionally, the solution provided high fidelity responses, demonstrating an 86% precision rate in response validation, while significantly reducing the need for manual reviews. Finally, it improved the overall user customer experience, as the GenAI powered solution guarantees much clearer grammar and writing, without spelling errors, maintaining an appropriate conceptual tone and facilitating customer understanding while maintaining appropriate security controls. See more of AWS GenAI services in Financial services [here](https://aws.amazon.com/financial-services/generative-ai/)   

**Thomson Reuters**  
Thomson Reuters modernized over 1.5 million lines of legacy .NET code per month using AWS Transform the first agentic AI experience for .NET modernization at scale. The solution leverages agentic AI to automate asset discovery, codebase analysis, planning, refactoring, and execution. AWS Transform enables parallel modernization jobs via both web and IDE interfaces, includes re-authentication checkpoints for long-running jobs, and adapts workflows in real-time. Teams seamlessly moved from Windows to Linux, cutting costs by 30% and reducing transformation timelines from months to two-week sprints. Technical debt was slashed by 50%. AWS Transform also proactively uncovers and remediates security vulnerabilities tied to outdated language versions and platforms.  
[Learn-More](https://aws.amazon.com/solutions/case-studies/thomson-reuters-case-study)

**Rocket Companies**  
Rocket Companies utilizes Amazon Bedrock and agentic generative AI to solve critical homeownership workflow challenges. Their solution, including the Rocket Assist tool, leverages over 10 petabytes of operational data and automates time-consuming administrative tasks. By using Amazon Bedrock’s multi-agent capabilities, they deliver solutions that achieved 68% faster query resolution and tripled loan closure rates. Bedrock agents orchestrate backend logic, data lookups, and conversational flows helping Rocket automate service and resource intensive business processes throughout the homeownership journey.  
[Learn-More](https://www.youtube.com/watch?v=Egc77PutWEo&list=PL2yQDdvlhXf89LPUVrnqUAO9SulA_op40&index=10)

**London Stock Exchange Group (LSEG)**  
Built a post-trade client services agent assistant with Amazon Q Business for rapid, AI-driven client support.  
[Learn-More](https://aws.amazon.com/blogs/machine-learning/london-stock-exchange-group-uses-amazon-q-business-to-enhance-post-trade-client-services/)

**TP ICAP**  
Migrated 50% of IT to AWS and uses generative AI (Amazon Bedrock) for market data, analytics, and green/sustainable business initiatives.  
[Learn-More](https://aws.amazon.com/solutions/case-studies/innovators/tp-icap/?did=cr_card&trk=cr_card)

---

 _**Healthcare & Life Sciences**_
------------------------
**Experity**    
Experity Launches Care Agent: The First Clinical Intelligence Solution for Urgent Care. Experity developed an AI-powered "Care Agent" using Amazon Bedrock. The solution leverages multiple LLMs, including Amazon Nova, to create conversational interface for patients. The system uses a multi-agent architecture for various tasks (e.g. authentication, document delivery, etc.) with built in guardrails to ensure reliable and compliant interactions. The solution provides a dual-channel communication approach and ultimately allows patients to use mobile message (SMS/RCS) for smart registration, and secure web chat throughout the entire patient journey including triage assessments, discharge notes, payment collections, and care reminders. And, all while remaining secure and compliant with HIPAA, protecting patients' private personal data.  
[Learn-More](https://www.experityhealth.com/news/experity-launches-care-agent-the-first-clinical-intelligence-solution-for-urgent-care/)   

**Bayer Crop Science**  
The solution: Bayer Crop Science built the Decision Science Ecosystem (DSE), a next-generation machine learning operations (MLOps) solution that accelerates data-driven decision making for science teams at scale across the organization. This solution helps the data scientist at every step, from ideation to model output, including the entire business decision record made using DSE.
How does it work? DSE integrates cohesively with Amazon SageMaker, a fully managed service that lets data scientists quickly build, train, and deploy machine learning (ML) models for different use cases so they can make data-informed decisions quickly, instead of having to construct and engineer the resource itself. Furthermore, the solution uses webhook-triggered code documentation generation powered by Amazon Q to automatically create high-quality code documentation and also to maintain and improve existing code documentation.  
[Learn-More](https://aws.amazon.com/blogs/machine-learning/accelerating-data-science-innovation-how-bayer-crop-science-used-aws-ai-ml-services-to-build-their-next-generation-mlops-service/)   

**Cornell Richard P. Riney Canine Health Center (RCHC) at the Cornell University College of Veterinary Medicine**    
 Big Red Bark Chat, a generative AI-powered chatbot that enables pet owners to get on-demand access to canine health information curated by RCHC faculty. The tool allows owners to evaluate symptoms, understand potential next steps, and decode veterinary medical reports while reinforcing that it does not replace a veterinarian. The solution is built on Amazon Bedrock, using Anthropic's Claude Sonnet 4 as its primary foundation model, and leverages Amazon Bedrock KnowledgeBases to ingest and index Cornell’s extensive collection of canine health articles, research papers, and educational materials, making sure responses are grounded in accurate veterinary information.  
[Learn-More](https://https://aws.amazon.com/blogs/publicsector/using-generative-ai-to-help-dog-owners-make-smarter-health-decisions/)   

**Sidekick**    
Sidekick is an Icelandic company with a mission to empower people to take control of their health by combining clinical and technical innovation to develop engaging and effective digital health products. Sidekick Health to developed a secure, cloud-native architecture for Archimedes, their dynamic solution which delivers personalized, real-time outreach and care coordination across digital health programs.
How does it work? The cloud-native architecture enables modular workflows, dynamic user profile orchestration, and automated validation of conversational outputs. A centralized control layer governs how user inputs are routed through specialized safety and accuracy checkpoints, each designed to enforce clinical validity, regulatory compliance, and interaction quality. The architecture leverages Amazon Bedrock and multiple Amazon Nova foundation models (Micro, Light, and Pro), ensures traceability of all outputs, and enables continuous performance optimization through structured testing and prompt evaluation. Healthcare providers can now access insights and treat patients more efficiently, while maintaining data privacy, security and complying with strict regulatory standards (GDPR, HIPAA, DiGA). 
The architecture enables evidence-based, traceable interactions - helping advance digital healthcare solutions for everyone. See more from Sidekick [here](https://www.sidekickhealth.com/) 

**Availity**  
Availity integrated Amazon Q Business, Amazon Q Developer, and Amazon Q in QuickSight to streamline operations and enhance productivity. Q Business powers conversational assistants for team-wide knowledge access and policy inquiries. Q Developer assists software teams by automating coding, code review, and troubleshooting, resulting in 33% of new code authored with Q Developer’s help. Q in QuickSight enables rapid natural language analytics for a two trillion-row dataset, centralizing insight generation and visualization for business decision making. Automation of code review, release management, and reporting with Amazon Q cut release-management meeting time by 75% and doubled data analysis speed. All solutions are built with high-security standards native to AWS services.  
[Learn-More](https://aws.amazon.com/solutions/case-studies/availity-case-study/)

---

_**Insurance**_
------------------------
**Travelers**    
Foundation model(FM)-based classifier through prompt engineering: Travelers receives millions of emails a year with agent or customer requests to service policies. The system Travelers built uses the predictive capabilities of FMs to classify complex, and sometimes ambiguous, service request emails into several categories. This FM classifier powers the automation system that can save tens of thousands of hours of manual processing and redirect that time toward more complex tasks. With Anthropic’s Claude models on Amazon Bedrock, we formulated the problem as a classification task, and through prompt engineering and partnership with the business subject matter experts, we achieved 91% classification accuracy.  
[Learn-More](https://aws.amazon.com/blogs/machine-learning/how-travelers-insurance-classified-emails-with-amazon-bedrock-and-prompt-engineering/)   

---
_**Retail**_
------------------------
**Booking.com**  
Booking.com was migrating their data-driven operations to the cloud, including more than 3,500 complex data processing workflows. A manual conversation process of these workflows could take years, draining valuable resources, impacting operational efficiency, and lengthening time-to-market for new services, all resulting in a negative user experience. Booking.com collaborated with AWS to design and develop a solution that automated and accelerated the migration process. Using Amazon Bedrock, Amazon SageMaker Studio, and Amazon S3, the solution focused on the following tasks: 1/ Oozie XML to YAML conversion, 2/ YAML validation, revision, and accuracy calculation, 3/ HiveQL to DBT SQL conversion, and 4/ On-prem pyspark to BDX pyspark conversion. The results speak to the power of innovation: 40% reduction in development time, enhanced workflow quality, and improved resource allocation. This enabled Booking.com to focus on what matters most - delivering exceptional travel experiences for their customers while building a more resilient, scalable infrastructure.  
[Learn-More](https://aws.amazon.com/solutions/case-studies/innovators/booking/)   

**Cars Commerce (Cars.com)**    
Cars.com was looking to improve the search experience for customers. The traditional legacy search filters worked for basic searches, but limited the vehicle discovery experience, as a query like "family-friendly SUV under $30K with good gas mileage" wasn't interpreted by the legacy system, leading to abandoned searches and an incomplete user experience. Cars.com built an innovative search solution that transforms how users discover vehicles through natural language queries. Built using Amazon Bedrock and Amazon Open Search, and powered by multiple foundation models, the solution implements low latency text-to-query for real-time search, and includes intelligent query parsing that converts conversational requirements into technical specifications and contextual enrichment through Cars.com's proprietary article database. This seamless translation process delivers highly relevant vehicle options that truly match what customers are seeking. Try-it-out-[here](https://www.cars.com/)   

**CJ ENM Global**  
CJ ENM Global is a South Korean conglomerate that operates as a leading entertainment and retail company, known for producing and distributing a wide range of content, including films, dramas, K-Pop, and animation. One of the businesses is ONSTYLE, a mobile commerce platform, where staff previously manually responded to customer questions during live commerce shows. The manual process created significant challenges as staff needed extensive product knowledge across multiple categories while managing high volumes of real-time inquiries about products, shipping, and payments. With only 20% of customer questions being answered due to these operational constraints, CJ ENM decided to implement an AI system to automate responses and improve service coverage. CJ ENM built an Agentic AI system that automates the entire Q&A response process for live commerce shows. Built on Amazon Bedrock, the solution combines Amazon Nova Pro and  Anthropic Claude Sonnet 3.7 with specialized agents to understand product images, extract relevant information, and generate accurate responses automatically. The system achieves 85-95% consistency ratio with human responses and reduces response time to under 10 seconds. But most importantly, the solution improved inquiry coverage rate from 20% to 91.5%. This solution demonstrates how Agentic AI is transforming customer experiences, in this case, shopping, by intelligently extracting product insights from visual content, automating personalized customer responses, and delivering enhanced customer experiences.  
[Learn-More](https://www.etnews.com/20250915000185)   

---


_**Independent Software Vendors (ISV)**_
------------------------
**Adobe**  
Adobe launched Adobe Unified Support, with the goal of helping thousands of the company's developers get immediate answers to questions from a centralized system.
Unified Support leverages Amazon Bedrock Knowledge Bases and the Vector Engine for Amazon OpenSearch Serverless to enhance document retrieval in a scalable, automated fashion. Amazon Bedrock Knowledge Bases is the backbone of the system, which indexes data through data ingestion, chunking, vectorization, and storage. When a user poses a question, the system vectorizes the query, retrieves most relevant chunks of data, and scores the relevant chunks so that the top ranked information is presented to the user. Metadata filtering was also added to provide developers with the option to retrieve data that is semantically relevant and spans multiple domains based on specific criteria.  
[Learn-More](https://aws.amazon.com/blogs/machine-learning/adobe-enhances-developer-productivity-using-amazon-bedrock-knowledge-bases/)  

**Intuit**  
During AWS Summit NYC 2025, Intuit demoed GenOS: their proprietary generative AI operating system—running on AWS (SageMaker, Bedrock, Aurora, MSK, and more).  
- **GenOS** powers agentic experiences: customer, finance, payments, and accounting agents, all integrated via an orchestration stack called GenRuntime (built for tool orchestration, context/memory, and guardrails).
- **AI & data**: Over 95PB of enterprise data, 60B predictions per day, and over half a million attributes per customer run through GenOS and AWS.
- **Workflow**: The platform features event buses, a data lake, and real-time vector databases—all built on and scaled by AWS cloud infrastructure.
- **User experience**: Small business owners interact with agents for customer engagement, cash flow monitoring, invoice drafting, and accounting. Human experts always remain in the loop, with GenUX providing a unified user interface.  
[Source: AWS Summit NYC 2025 Keynote (YouTube, Intuit section: 0:09:44–0:13:00)](https://youtu.be/W0hZY-sdxVE)

**DTEX Systems**    
DTEX is using GenAI to help analyst teams respond faster, understand the intention of end users, and interpret human behavior in ways that weren't possible previously. Support from the GenAIIC unlocked this potential for DTEX by providing best practices for adoption of Claude models via Amazon Bedrock to better fit the needs of the use case, and co-developing DTEX's proprietary capabilities for vector embedding and semantic analysis on their data set. Further support from the Amazon Open Search team has enabled DTEX to be efficient and follow best practices for architecture design, implementation, and production of their solutions.  
[Learn-More](https://www.youtube.com/watch?v=m9MWN9XpX5Y)   

**Druva**    
Druva built multi-agent system that can understand and respond to customer questions in everyday language. Using Amazon Bedrock, AgentCore, and Strands Agents, the solution uses multiple AI agents that work together to dynamically choose the right tool from hundreds of options, to proactively secure, recover, and manage customer data. The system consists of a supervisor agent and sub-agents, including: 1/ Data Agents that surface key signals and trends from telemetry, risk indicators, and history, 2/ Help agent that guide users by troubleshooting problems, investigating incidents, and recommending next steps, and 3/ Action agents that carry out specific tasks, such as recovering workloads, creating protection policies, or adjusting retention to optimize cost. When customers ask a question or need help, the system figures out what they need and handles the technical work "behind the scenes," making it much easier for customers to get things done without needing to understand the technical processes.  
[Learn-More](https://www.druva.com/about/press-releases/druva-introduces-ai-agents-to-simplify-cyber-resilience)  

---

_**Media & Sports**_
------------------------ 

**Formula 1®**  
Formula 1 partnered with AWS to build a root cause analysis (RCA) assistant using Amazon Bedrock, Bedrock Agents, and Bedrock Knowledge Bases. The solution ingests raw logs into Amazon S3, processes data via EventBridge and AWS Glue ETL pipelines, and feeds structured logs into Bedrock Knowledge Bases backed by OpenSearch vectors. Bedrock Agents query internal (SQL, CloudWatch, EC2) and external systems (Jira, Datadog), providing real-time, actionable troubleshooting via a Streamlit based chat UI. Anthropic Claude 3 models orchestrate the agent flow, ensuring accuracy and relevance. Strict API and SQL access controls are implemented for security. Triage time was reduced from days to 20 minutes; overall resolution time dropped by 86%. The RCA agent also autonomously routes problems to relevant teams, letting engineers focus more on innovation and less on manual investigation.  
[Learn-More](https://aws.amazon.com/blogs/machine-learning/how-formula-1-uses-generative-ai-to-accelerate-race-day-issue-resolution/)

---

_**Digital Transformation**_
------------------------
**Pitney Bowes**    
Pitney Bowes developed Agentic AI Beacon with Live Agent Handover, which was launched in PitneyShip. PitneyShip is a cloud-based shipping and mailing software that helps businesses streamline their shipping processes by offering discounted rates from multiple carriers (like USPS and UPS), printing postage, tracking packages, and providing reporting features. Built using Amazon Bedrock, the solution leverages multi-agent orchestration using specialized agents plus a "master" agent for routing, and an enterprise-tuned RAG using Bedrock Knowledge Bases to optimize the groundedness of responses. Other technical highlights include built-in governance (e.g. APIs, observability, compliance guardrails), and evaluation harnesses, enabling fully automated customer simulation before rollout.  
[Learn-More](https://www.pitneybowes.com/content/dam/campaign/bpx-pitneybowes-whitepaper3-aishipping-041025-v3.pdf?cid=email_us_sts_pitneyshipper_growth_marketing_june24_2025_link2_ai_powered_shipping_whitepaper)   

**LG Electronics (LGE)**    
LGE and GenAIIC built a YouTube analytics solution for market competitiveness analysis. The automated system uses a multi-model approach with Anthropic Claude 3.7 and
Amazon Nova Pro on Amazon Bedrock, extracting 24 structured fields from video transcripts and comments, including sentiment analysis, product features, and multi-format summaries with real time Q&A capabilities. The solution implements LLM-based evaluation using consistency, alignment, and coverage metrics to ensure measurable extraction quality. It is integrated with an in-house social media portal where business professionals can easily (and timely) gain insights.  
[Learn-More (Korean)](https://aws.amazon.com/ko/blogs/tech/lg-social-media-analysis-with-amazon-bedrock/)  

**POSCO HOLDINGS DX**   
POSCO was looking to automate the manual, time consuming process for their hardware engineers, the creation of PLC card drawings with AutoCAD. The legacy process required highly skilled engineers to understand complex Excel structures across multiple worksheets to identify appropriate PLC cards for specific sensors, handle AutoCAD files, manipulate Excel data, and adapt to various input formats from multiple suppliers. Thry built an AgenticAI to automate the entire PLC card drawing generation process. The solution combines AI-based and rule-based pure Python-coding approaches to understand semi-structured Excel documents, extract relevant information, and generate AutoCAD files automatically. The solution is powered by Amazon Bedrock, using autoplanning and coordinating from a plain prompt as well as visual understanding of semi-structured Excel documents and images with Anthropic's Claude Sonnet 3.7 Large Language Model (LLM) and Vision Language Model (VLM). The result? Instead of days to produce a single PLC card, the process is automated to 6 minutes with 99% accuracy.  
[Learn-More](https://www.mk.co.kr/en/it/11366537)  

_**Qlik & Qlik Customers**_
------------------------
**TouchPoint Support Services**  
Deployed Qlik Answers, an AWS-native generative AI solution, for 15,000 healthcare staff to instantly access thousands of complex policy documents. Powered by Amazon Bedrock and SageMaker, Qlik Answers offers a conversational, agentic interface so employees can simply ask a question to find the relevant policy or procedure. By integrating with Qlik Cloud and leveraging AWS as the data backbone, TouchPoint’s deployment saw huge adoption and time savings, transforming end-user experience for front-line workers.  
[Learn-More](https://www.qlik.com/us/solutions/customers/customer-stories/touchpoint-support-services)

**Lintech International**  
Lintech’s sales teams use Qlik Answers (agentic AI powered by Amazon Bedrock and AWS infrastructure) to instantly search over 17,000 technical and regulatory documents—reclaiming 7 hours per week per manager and achieving 75% faster customer response times. This system is fully integrated into Lintech’s data landscape on AWS, ensuring secure and accurate retrieval while modernizing workflow.  
[Learn-More](https://www.qlik.com/us/solutions/customers/customer-stories/lintech-international)

**Bystronic Group**  
Bystronic, a global manufacturing leader, transformed operations using Qlik Answers (agentic generative AI on AWS) to turn vast and messy unstructured data—spanning thousands of manufacturing machines—into concise, actionable answers. Their solution, built on Qlik Cloud and AWS services (such as Bedrock and analytics backbone), scaled insights and agentic knowledge to global teams across the manufacturing chain.  
[Learn-More](https://www.qlik.com/us/solutions/customers/customer-stories/bystronic-group)

---

_**Airline**_
------------------------
**Ryanair**  
Ryanair operates over 3,600 flights daily and has a goal of doubling passenger capacity by 2034. To help provide front line staff with crucial operational information, Ryanair developed a new cabin crew application built risk management and trusted AI controls into the app. Using our automated risk assessment framework powered by Amazon Bedrock, the application provides an automated risk assessment for the cabin crew, and addresses notable Responsible AI dimensions such as security, data privacy, explainability and controllability. How does it work? Leveraging an LLM-as-a-judge approach, the framework checks a set of 250 controls (based on international standards like ISO controls, NIST600 and OWASP frameworks) on top of different artifacts including prompts, source code, and technical documentation. It also directly connects to Ryanair’s API to perform pen-tests and jailbreaking attempts. The solution provides continuous monitoring capabilities and a single pane of glass to drive timely actions and can monitor hundreds of GenAI applications in production.Ryanair and AWS delivered meaningful impact by enhancing risk visibility and automating risk management. The solution established a transparent, data-driven assessment of AI risks in the cabin crew app, providing clear insights where previously risks were difficult to quantify. Furthermore, the solution transformed manual, time-intensive risk evaluations into an automated monitoring solution – a first for Ryanair’s GenAI applications. The solution helps protect both passenger and operational data while enabling Ryanair's ambitious growth plans. By incorporating security and privacy controls from the start, the airline can confidently scale their AI innovations, demonstrating how organizations can embrace generative AI's potential while maintaining robust security practices.
Learn more about Ryanair’s work on AWS [Here](https://aws.amazon.com/solutions/case-studies/innovators/ryanair/?trk=4b29643c-e00f-4ab6-ab9c-b1fb47aa1708&sc_channel=podcast)

_**Agriculture**_
------------------------ 

**Syngenta**  
Syngenta’s Cropwise AI, built in collaboration with AWS, empowers seed sales reps and farmers with generative AI tools for seed selection and recommendation. The solution uses Amazon Bedrock Agents to build a multi-agent orchestration layer, integrating user queries, backend agronomic models, and metadata from DynamoDB and S3. AWS Lambda provides serverless function execution, AppSync manages real-time data exchange, and Cognito secures user authentication and access control. Cropwise AI’s agent layer selects between multiple foundation models (Meta, Claude 3.5, Llama, etc.) as needed. Document ingestion and text extraction are automated with S3, Textract, and Step Functions. Bedrock Knowledge Bases enable intelligent retrieval from large agronomic datasets using OpenSearch vectors. Sales reps deliver tailored, data-driven seed recommendations 5x faster; farmers get contextual decision support accessible via a conversational mobile interface. The agent tracks outcomes to personalize recommendations and drive continuous system improvement.  
[Learn-More](https://aws.amazon.com/blogs/machine-learning/syngenta-develops-a-generative-ai-assistant-to-support-sales-representatives-using-amazon-bedrock-agents/)

---


_**Public Sector**_
------------------------
**US Navy COMSUBFOR (Commander, Submarine Force)**    
COMSUBFOR developed an agentic Retrieval-Augmented Generation (RAG) solution with a complex Amazon Open Search architecture, providing separate indexes for each submarine to accommodate their unique technical specifications. Powered by Amazon Bedrock Agents on Amazon Bedrock, the solution implements an AI-driven system and creates an agentic architecture that consults vector databases, searches the COMSUBFOR website for information, and generates specific Navy Official Forms.  
[Learn-More](https://aws.amazon.com/government-education/)   

**US Environmental Protection Agency (EPA)**    
Intelligent document processing solution: The team built intelligent document processing solutions, powered by Anthropic models on AmazonBedrock to address labor intensive processes of assessing chemical risk and review and regulate pesticides in the U.S. Both solutions leverage intelligent document processing using Amazon Simple Storage Service and Amazon Textract, as well as incorporating knowledge bases and criteria from EPAs own data stores. Most importantly, the heavy lifting of assessing, comparing, evaluating is done by generative AI, but the humans remain in the loop and in control, accepting or modifying the AI generated evaluations before finalizing decisions.  
[Learn-More](https://aws.amazon.com/blogs/publicsector/accelerating-workflows-with-generative-ai-epas-document-processing-journey/)   

**Buenos Aires City Government**    
The Buenos Aires City Government upgraded its popular WhatsApp AI assistant, Boti, using LangGraph and Amazon Bedrock. This enhancement introduced an agentic AI solution to help citizens navigate the city's 1,300 complex government procedures.
The system features an input guardrail that uses a custom LLM classifier to approve or block user requests based on content. Approved queries are then handled by a government procedure agent, which retrieves the relevant information and generates a response. The assistant maintains Boti's characteristic style, delivering short, helpful messages in Argentina's Rioplatense Spanish dialect.  
[Learn-More](https://aws.amazon.com/blogs/machine-learning/meet-boti-the-ai-assistant-transforming-how-the-citizens-of-buenos-aires-access-government-information-with-amazon-bedrock/) (More on Boti [here](https://lnkd.in/eWXD3rCM))

---

_**Education**_
------------------------
**The University of Texas at Austin**    
UT Sage: A virtual instructional designer and AI Tutor designed by UT Austin experts to support the responsible use of generative AI in teaching and learning, Built on
AmazonBedrock and powered by Anthropic Claude models.  
[Learn-More](https://provost.utexas.edu/the-office/academic-affairs/office-of-academic-technology/ut-sage/)   

---

_**Education Tech (EdTech)**_
------------------------
**Renaissance**    
Renaissance Learning and AWS collaborated to build a solution that automatically analyzes and categorizes educational content, mapping items to relevant state standards using natural language processing. Built on Amazon Bedrock and leveraging Amazon OpenSearch for information retrieval, AWS Lambda for serverless processing, the solution intelligently maps content and learns from existing mapped content to improve accuracy. The solution also provides confidence scores for mapped relationships.  
[Learn-More](https://aws.amazon.com/blogs/publicsector/renaissance-uses-generative-ai-on-aws-to-accelerate-personalized-learning-at-scale/)   

---

_**Legal Tech**_
------------------------
**Robin AI**    
LLM-as-a-jury: Robin AI accelerates contract work for legal professionals using AI-powered tools combined with expert legal knowledge. Their legal assistant traditionally relied on human experts to assess AI-generated legal answers, a process they have now begun to automate and scale through a partnership with the AWS Generative AI Innovation Center. Robin AI employed an LLM-as-a-judge approach using Amazon #Bedrock with Amazon #Nova Pro and Anthropic's #Claude 3 Haiku to serve as an LLM "jury." These foundation models were fine-tuned on data from over 500 contracts across nine types and guided by expert feedback to evaluate and improve the quality of AI-generated legal responses, incorporating prompt optimization, data augmentation, and iterative model training for enhanced accuracy and reliability.  
[Learn-More](https://robinai.com/platform/)   
