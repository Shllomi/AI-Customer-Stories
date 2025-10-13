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

_**Financial Services**_
------------------------ 
**Itaú Unibanco**    
Pix on WhatsApp is one of the first solutions connected to Inteligência Itaú and uses generative AI to interact with clients through WhatsApp and make day-to-day transfers in an automated and instant way. [Learn-More](https://www.itau.com.br/relacoes-com-investidores/noticias/inteligencia-itau-banco-lanca-nova-experiencia-para-clientes-com-ia-generativa/?lang=en)   

_**Digital Transformation**_
------------------------
**Pitney Bowes**    
Pitney Bowes developed Agentic AI Beacon with Live Agent Handover, which was launched in PitneyShip. PitneyShip is a cloud-based shipping and mailing software that helps businesses streamline their shipping processes by offering discounted rates from multiple carriers (like USPS and UPS), printing postage, tracking packages, and providing reporting features. Built using Amazon Bedrock, the solution leverages multi-agent orchestration using specialized agents plus a "master" agent for routing, and an enterprise-tuned RAG using Bedrock Knowledge Bases to optimize the groundedness of responses. Other technical highlights include built-in governance (e.g. APIs, observability, compliance guardrails), and evaluation harnesses, enabling fully automated customer simulation before rollout. [Learn-More](https://www.pitneybowes.com/content/dam/campaign/bpx-pitneybowes-whitepaper3-aishipping-041025-v3.pdf?cid=email_us_sts_pitneyshipper_growth_marketing_june24_2025_link2_ai_powered_shipping_whitepaper)   

**LG Electronics (LGE)**    
LGE and GenAIIC built a YouTube analytics solution for market competitiveness analysis. The automated system uses a multi-model approach with Anthropic Claude 3.7 and
Amazon Nova Pro on Amazon Bedrock, extracting 24 structured fields from video transcripts and comments, including sentiment analysis, product features, and multi-format summaries with real time Q&A capabilities. The solution implements LLM-based evaluation using consistency, alignment, and coverage metrics to ensure measurable extraction quality. It is integrated with an in-house social media portal where business professionals can easily (and timely) gain insights.
 [Learn-More (Korean)](https://aws.amazon.com/ko/blogs/tech/lg-social-media-analysis-with-amazon-bedrock/)  
 
 _**Healthcare**_
------------------------
**Experity**    
Experity Launches Care Agent: The First Clinical Intelligence Solution for Urgent Care. Experity developed an AI-powered "Care Agent" using Amazon Bedrock. The solution leverages multiple LLMs, including Amazon Nova, to create conversational interface for patients. The system uses a multi-agent architecture for various tasks (e.g. authentication, document delivery, etc.) with built in guardrails to ensure reliable and compliant interactions. The solution provides a dual-channel communication approach and ultimately allows patients to use mobile message (SMS/RCS) for smart registration, and secure web chat throughout the entire patient journey including triage assessments, discharge notes, payment collections, and care reminders. And, all while remaining secure and compliant with HIPAA, protecting patients' private personal data. [Learn-More](https://www.experityhealth.com/news/experity-launches-care-agent-the-first-clinical-intelligence-solution-for-urgent-care/)   

**Cornell Richard P. Riney Canine Health Center (RCHC) at the Cornell University College of Veterinary Medicine**    
 Big Red Bark Chat, a generative AI-powered chatbot that enables pet owners to get on-demand access to canine health information curated by RCHC faculty. The tool allows owners to evaluate symptoms, understand potential next steps, and decode veterinary medical reports—while reinforcing that it does not replace a veterinarian. The solution is built on Amazon Bedrock, using Anthropic's Claude Sonnet 4 as its primary foundation model, and leverages Amazon Bedrock KnowledgeBases to ingest and index Cornell’s extensive collection of canine health articles, research papers, and educational materials, making sure responses are grounded in accurate veterinary information. [Learn-More](https://https://aws.amazon.com/blogs/publicsector/using-generative-ai-to-help-dog-owners-make-smarter-health-decisions/)   

_**Insurance**_
------------------------
**Travelers**    
Foundation model(FM)-based classifier through prompt engineering: Travelers receives millions of emails a year with agent or customer requests to service policies. The system Travelers built uses the predictive capabilities of FMs to classify complex, and sometimes ambiguous, service request emails into several categories. This FM classifier powers the automation system that can save tens of thousands of hours of manual processing and redirect that time toward more complex tasks. With Anthropic’s Claude models on Amazon Bedrock, we formulated the problem as a classification task, and through prompt engineering and partnership with the business subject matter experts, we achieved 91% classification accuracy. [Learn-More](https://aws.amazon.com/blogs/machine-learning/how-travelers-insurance-classified-emails-with-amazon-bedrock-and-prompt-engineering/)   

_**Public Sector**_
------------------------
**US Navy COMSUBFOR (Commander, Submarine Force)**    
COMSUBFOR developed an agentic Retrieval-Augmented Generation (RAG) solution with a complex Amazon Open Search architecture, providing separate indexes for each submarine to accommodate their unique technical specifications. Powered by Amazon Bedrock Agents on Amazon Bedrock, the solution implements an AI-driven system and creates an agentic architecture that consults vector databases, searches the COMSUBFOR website for information, and generates specific Navy Official Forms. [Learn-More](https://aws.amazon.com/government-education/)   

**US Environmental Protection Agency (EPA)**    
Intelligent document processing solution: The team built intelligent document processing solutions, powered by Anthropic models on AmazonBedrock to address labor intensive processes of assessing chemical risk and review and regulate pesticides in the U.S. Both solutions leverage intelligent document processing using Amazon Simple Storage Service and Amazon Textract, as well as incorporating knowledge bases and criteria from EPAs own data stores. Most importantly, the heavy lifting of assessing, comparing, evaluating is done by generative AI, but the humans remain in the loop and in control, accepting or modifying the AI generated evaluations before finalizing decisions.[Learn-More](https://aws.amazon.com/blogs/publicsector/accelerating-workflows-with-generative-ai-epas-document-processing-journey/)   

**Buenos Aires City Government**    
The Buenos Aires City Government upgraded its popular WhatsApp AI assistant, Boti, using LangGraph and Amazon Bedrock. This enhancement introduced an agentic AI solution to help citizens navigate the city's 1,300 complex government procedures.
The system features an input guardrail that uses a custom LLM classifier to approve or block user requests based on content. Approved queries are then handled by a government procedure agent, which retrieves the relevant information and generates a response. The assistant maintains Boti's characteristic style, delivering short, helpful messages in Argentina's Rioplatense Spanish dialect. [Learn-More](https://aws.amazon.com/blogs/machine-learning/meet-boti-the-ai-assistant-transforming-how-the-citizens-of-buenos-aires-access-government-information-with-amazon-bedrock/) (More on Boti [here](https://lnkd.in/eWXD3rCM))

_**Independent Software Vendors (ISV)**_
------------------------
**DTEX Systems**    
DTEX is using GenAI to help analyst teams respond faster, understand the intention of end users, and interpret human behavior in ways that weren't possible previously. Support from the GenAIIC unlocked this potential for DTEX by providing best practices for adoption of Claude models via Amazon Bedrock to better fit the needs of the use case, and co-developing DTEX's proprietary capabilities for vector embedding and semantic analysis on their data set. Further support from the Amazon Open Search team has enabled DTEX to be efficient and follow best practices for architecture design, implementation, and production of their solutions. [Learn-More](https://www.youtube.com/watch?v=m9MWN9XpX5Y)   

_**Education**_
------------------------
**The University of Texas at Austin**    
UT Sage: A virtual instructional designer and AI Tutor designed by UT Austin experts to support the responsible use of generative AI in teaching and learning, Built on
AmazonBedrock and powered by Anthropic Claude models. [Learn-More](https://provost.utexas.edu/the-office/academic-affairs/office-of-academic-technology/ut-sage/)   

_**Education Tech (EdTech)**_
------------------------
**Renaissance**    
Renaissance Learning and AWS collaborated to build a solution that automatically analyzes and categorizes educational content, mapping items to relevant state standards using natural language processing. Built on Amazon Bedrock and leveraging Amazon OpenSearch for information retrieval, AWS Lambda for serverless processing, the solution intelligently maps content and learns from existing mapped content to improve accuracy. The solution also provides confidence scores for mapped relationships. [Learn-More](https://aws.amazon.com/blogs/publicsector/renaissance-uses-generative-ai-on-aws-to-accelerate-personalized-learning-at-scale/)   

_**Legal Tech**_
------------------------
**Robin AI**    
LLM-as-a-jury: Robin AI accelerates contract work for legal professionals using AI-powered tools combined with expert legal knowledge. Their legal assistant traditionally relied on human experts to assess AI-generated legal answers, a process they have now begun to automate and scale through a partnership with the AWS Generative AI Innovation Center. Robin AI employed an LLM-as-a-judge approach using Amazon #Bedrock with Amazon #Nova Pro and Anthropic's #Claude 3 Haiku to serve as an LLM "jury." These foundation models were fine-tuned on data from over 500 contracts across nine types and guided by expert feedback to evaluate and improve the quality of AI-generated legal responses, incorporating prompt optimization, data augmentation, and iterative model training for enhanced accuracy and reliability. [Learn-More](https://robinai.com/platform/)   

**Example 1**    
Example [Learn-More](https://example.com)  
