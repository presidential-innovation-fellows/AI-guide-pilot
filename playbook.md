# THE ARTIFICIAL INTELLIGENCE GUIDE ON GETTING TO PILOT

_Last Updated: January 27th, 2020_


This guide is a product of [10x](http://10x.gsa.gov) investments, made in collaboration with the [CIO Council](http://cio.gov), and the [Presential Innovation Fellows](http://pif.gov).

## Table of contents

- [Introduction](#introduction)
	- [Who should use this guide, and how and why they should use it](#who-should-use-this-guide-and-how-and-why-they-should-use-it)
- [Identifying your problem and evaluating the approach](#identifying-your-problem-and-evaluating-the-approach)
	- [Identify the problem](#identify-the-problem)
	- [Evaluate whether the problem is a fit for AI/ML](#evaluate-whether-the-problem-is-a-fit-for-aiml)
	- [Bring diverse, experienced teams in-house](#bring-diverse-experienced-teams-in-house)
	- [Know your data](#know-your-data)
	- [Continuously test and evaluate prototypes](#continuously-test-and-evaluate-prototypes)
- [Culture and Education](#culture-and-education)
	- [Identify key risks, including resistance](#identify-key-risks-including-resistance)
	- [Assess and manage ethical concerns](#assess-and-manage-ethical-concerns)
	- [Build support and educate senior stakeholders](#build-support-and-educate-senior-stakeholders)
- [Run your pilot](#run-your-pilot)
	- [Have a clear plan](#have-a-clear-plan)
	- [Create standards for measuring the performance of models](#create-standards-for-measuring-the-performance-of-models)
	- [Know and follow the relevant laws to your project](#know-and-follow-the-relevant-laws-to-your-project)
- [Post pilot: Now what?](#post-pilot-now-what)
	- [Consider the long-term investment strategy](#consider-the-long-term-investment-strategy)
	- [Lay the seeds for future experimentation](#lay-the-seeds-for-future-experimentation)
- [Case Study: Census Bureau](#case-study-census-bureau)
- [Appendix I: Definition of Terms](#appendix-I-definition-of-terms)
- [Appendix II: Additional Resources](#appendix-II-additional-resources)

## Introduction


[Artificial Intelligence](https://science.sciencemag.org/content/357/6346/19) (AI) has the potential to help many federal government agencies deliver on the services that the American public counts on. This guide provides a set of recommendations and best practices for how federal agencies can begin piloting AI solutions to assist with service delivery.

While there are several different categories of AI, this guide is mostly relates to machine learning (ML), where algorithms find patterns in data without explicit instruction. AI and ML can help agencies automate manual, labor intensive tasks, as well as assist in informing decision-making. Searching databases, understanding language, labeling text and images, and identifying patterns in large amounts of data are very common problems that AI can help with.

Pilots evaluate whether an AI project is ready for broader use. Here is a rough diagram of what an AI project build from design to scale might look like.

Pilot projects can have a broad definition and set of criteria across the U.S. federal government. With respect to this guide, an AI pilot should meet the following criteria:

- AI models are running, learning from data, and helping to make decisions
- There is a framework in place to evaluate the effectiveness of the AI models
- A selection of the public can interact with the service and provide feedback
- Evidence is gathered as to whether the service meets user needs

### Who should use this guide, and how and why they should use it

This guide is for:

- Government leaders considering machine learning as a solution in a pilot project
- CIOs, CTOs, and CDOs providing technical leadership for an AI pilot project
- Program staff and managers trying to learn more about AI
- Agency staff managing a pilot software project where AI is a capability

Readers of this guide will learn how to manage many of the key risks inherent to an AI pilot project including:

- Identifying whether the problem really is a fit for AI
- Hiring the right people
- How to run an AI pilot
- Cultural risks
- What to consider post-pilot

These plays were derived from studying lessons learned from interviews of dozens of Federal employees involved in developing and driving agency AI projects. Additionally, experts from the [Technology Transformation Services](https://www.gsa.gov/about-us/organization/federal-acquisition-service/technology-transformation-services), [United States Digital Services](http://usds.gov), [The CIO Council](http://cio.gov), [The Presidential Innovation Fellows](http://pif.gov), [Network Information Technology Research and Development Program AI Interagency Working Group](http://https://www.nitrd.gov/nitrdgroups/index.php?title=AI), and the [American Council for Technology and Information Advocacy Council](http://https://www.actiac.org/) (ACT-IAC) were key to its development. 

These 13 best practices are ordered roughly in sequence. However, a project team should revisit many of them during the course of an AI project. Each play contains a short description, with key checklist items and questions to be answered at each step. 

This guide is not:

- A set of linear steps
- The entire overview of an AI lifecycle
- A complete primer on laws and ethics, data governance, user-centered design, or software development
- A review of data science or machine learning

This guide is meant to be a living document. Every month, new research and guidance on AI for governments is released. As the technological sophistication of AI solutions advances, this set of plays, checklists, and questions should be updated to remain relevant and useful to federal community. 


# Identifying your problem and evaluating the approach

AI is not an all-purpose solution; it is another tool to help agencies meet their missions. For designing any service, always begin with user needs.

## Identify the problem

It is important for agencies to take the time to understand the problem they are trying to solve with AI. Rather than beginning with AI as a solution, first identify the problem to be solved.

[Begin by understanding what people need](https://playbook.cio.gov/#play1). An algorithm is only a small part of a solution, and part of an overall service. What needs should that service solve for? To find out, involve users in the design process from the beginning. Users might be the public or internal agency employees. There are many [methods](https://methods.18f.gov/) to understanding these needs, but pretty much all of them involve speaking to users directly.

You should interview individuals impacted by the technology to understand and address potential concerns. For example, a tool that helps to adjudicate benefits decisions may have an internal agency user-base, but also external stakeholder groups like individuals applying for benefits whose views are crucial to factor into design decisions.

A template for a clear problem statement might look like the following:

> We have observed that _product/service/organization_ isn’t meeting _these goals/needs_, which is causing _this adverse effect_. How might we improve so that our product/service/team/organization is more successful based on _these measurable criteria?_
       

##### Checklist

- [ ] Create a list of specific user needs that the solution will need to address 
- [ ] Understand how the solution fits within the user’s journey or workflow
- [ ] Read the [Digital Services playbook](http://https://playbook.cio.gov/) 
- [ ] Work with senior leadership to understand how the problem statement fits within their priorities or mission
- [ ] As you uncover new unmet needs, document these and share them with the team and agency leadership
- [ ] Test prototypes of solutions with real people, in the field if possible
- [ ] Identify key metrics and outcomes for solving the problem, rather than metrics for the technical solution
- [ ] Understand previous attempts to solve this problem and those projects’ outcomes

##### Key Questions

- How quickly can you begin speaking to users to learn more about the problem and unaddressed needs?
- What goals or needs aren’t being met? What measurable criteria would indicate progress toward those goals?
- Are you at a point where you are hearing the same challenge described over and over again?
- Do you have a document describing the history of this problem and the various connected issues?
- Can you articulate in plain language the problem to be solved?

## Evaluate whether the problem is a fit for AI/ML

AI, and ML are methodologies for solving a problem. Oftentimes, simpler solutions like Robotic Process Automation (RPA), rule-based software, or analytics can be more effective and less costly. However, there are problems in agencies where AI and machine learning is the most effective approach from a business and cost- savings standpoint.

AI is not:
- An all-purpose solution
- Capable of making judgements the way humans can 

AI can help when:
- There are large amounts of high-quality data
- The problem to be solved is repetitive
- The problem is narrowly scoped (for example, differentiating a kind of object/sound/image from something else)
- The problem is too expensive to be solved at scale with human resources
- The problem can be ethically solved with a machine, and a mistake by that machine would not pose a serious risk
to users
- An engineer can effectively program a machine to learn the task
- The solution involves labeling (or scoring) something

When evaluating use cases for AI it can be helpful to think about outputs of a repetitive task, and then work backwards. Even if there is a better solution than AI, the use-case could still be handed to an engineer and developed into a solution.

For example:

|Benefits |Steering Wheel|Product Description|Bridge |Data Center Cooling System|Image|Transaction|
|:---|:---|:---|:---|:---|:---|:---|
|Eligible or Ineligible?| Left or Right?| Correct or Not?|Send maintenance crew or not?| Warmer or cooler?| Fake or real?| Fraudulent or real?|

If your agency doesn’t have the talent to evaluate whether the problem is a fit for AI, the agency should consider contacting the [AI Center of Excellence](mailto:connectcoe@gsa.gov) at the Technology Transformation Service. When issuing a Request for Proposal (RFP), in most situations an agency should not describe the solution as AI unless there is strong reason to believe so. Even then, the agency should be open to alternative technical solutions. Instead, focus on delivering a clear problem statement.

The UK Office of Artificial Intelligence and the World Economic Forum have [released guidance on procuring AI solutions](https://www.weforum.org/whitepapers/ai-government-procurement-guidelines) that can be helpful to review when planning your purchasing strategy.

##### Checklist

- [ ] Fill out an AI Agency Self-Assessment Checklist for AI 
- [ ] Assess whether AI is an appropriate solution by consulting with a data analyst or data scientist
- [ ] Consult with a domain expert who understands the set of issues that will impact the deployment of the solution was consulted
- [ ] You have or can procure a large amount of high quality data for training machine learning models
- [ ] You have many labelled examples of what “right” looks like for the models to learn from
- [ ] Identify whether you have a healthy budget for hiring, building and long-term maintenance of an AI solution
- [ ] Determine whether AI application will produce better ROI over simpler and cheaper analytics

##### Key questions

- Can you express what the right action is for a machine?
- Do you have enough data for a model to learn from?
- Have you asked a statistician or data scientist how much data you will need to solve your problem with AI?


### Bring diverse, experienced teams in-house

You will need to draw on the skills of a data scientist or data analyst for at least a short period of time to validate that AI is indeed a viable solution for your problem. Testing and evaluation before committing to a given path should always happen before advancing further with a pilot.

If you don’t have experts who understand your data and the relationship to your use-case in-house already, bringing in someone in-house to do this has several advantages over outsourcing to a vendor.

- Generally speaking, in-house data scientists have fewer barriers to speaking with data owners, and getting access to data
- It may be cheaper than hiring a vendor, as an in-house data scientist can quickly create experiments and build models to test the viability of AI
- It may be faster than hiring a vendor
- That employee can oversee a vendor if a contract is awarded, especially if there isn’t the technical expertise on
staff to work with the vendor
- Such experts, combined with domain data experts, can interact and evaluate various company tools and ideas via
AI tech sprints

Integrating these algorithms into a software application will probably involve more than a data scientist. You will likely need a diverse team including at least a designer, engineer, and possibly a product manager to work with the product owner on your team. They should be familiar with user-centered design and agile methods.

##### Checklist

- [ ] Consider working with 18F acquisitions specialists to help with procurement for the project
- [ ] Ensure that the team building the solution and the agency team that knows the data are working closely with one another
- [ ] Work with a data scientist to validate that AI is a sensible approach to solving a problem
- [ ] Integrate vendor teams closely with your agency’s teams so that there are good communication practices, a responsive culture, and a clear understanding of the problem to be solved
- [ ] Work with government fellowships like the Presidential Innovation Fellows, AAAS Fellows, the Civic Digital Fellows, and Presidential Management STEM Fellows, as well as academic institutions in computer science, to bring hard-to-find skill sets in statistics, computer science, and AI into your agency
- [ ] Consider using hackathons or [data science challenges](http://https://www.cdc.gov/flu/news/predict-flu-challenge.htm) (such as [Kaggle](http://https://www.kaggle.com/)) as means to engage industry on building tools, evaluating tools, and exchanging ideas/perspectives around open datasets and/or datasets that only need simple data use agreements.
- [ ] Recruit at least one designer, and possibly a front-end and back-end engineer to develop prototypes and ultimately build software that can meet user needs for a pilot.

##### Key Questions

- What is your justification for using AI to solve this problem, versus robotic process automation (RPA), or another tool?
- Have you asked your team to see if anyone has the requisite data skills? 
- Do you have an experienced person on your hiring team to evaluate whether the people you are hiring have the appropriate skills?
- Does the team have experience working in the government?
- Is the hired team really agile?


### Know your data

You will need a large volume of data to train machine learning models. Sometimes you may need to look for data outside your agency, if the data you have is not sufficient for the problem you are trying to solve.

AI does not reason like a human. AI algorithms ingest a set of inputs in the form of data and can only return an output. For this reason, knowing your data is not just about knowing the size of your databases or whether you have the right kind of data, but also involves the quality of your data:

- Data provenance
- Accuracy
- Laws governing that data
- Validity
- Reliability
- Completeness
- Uniqueness
- Timeliness
- Consistency
- Overall value to the organization

Developing a strong understanding of your data is the first step to laying the groundwork for an effective data management strategy -- and eventually better software, including AI. You will need to have access to a data scientist to do this, and you may want to bring them in-house.

For a pilot, you may be able to use synthetic data (or artificially created data) to test the viability of an AI solution meeting a user’s needs. If you find new data within your agency, you should document it in accordance with the [Federal Data Strategy](https://strategy.data.gov/), and if non-sensitive, make it available in a machine readable format for data discovery (for example, on [data.gov](http://data.gov]).

##### Checklist

- [ ] Work closely with data owners, data scientists, statisticians, and subject matter experts within your agency to understand the state of your data, including accuracy, validity, reliability, completeness, and more 
- [ ] Consider where you might identify other sources of data to meet your short-term and long-term requirements. Can you buy the data, artificially create it, collect it from other places that haven’t surfaced yet, or add new means of collecting data like sensors? 
- [ ] Know where your data is physically located and who are the points of contact for accessing the data
- [ ] Be sure data has links to provenance information to facilitate quality checks, reproducibility, and interpretability
- [ ] Keep your data clean and well-structured as you collect and store it
- [ ] Understand data standards, ontologies, and terminologies that may be applicable to your data

##### Key Questions

- Have you identified data experts within your agency and paired them with a data scientist to ensure that the data scientist can learn about the data quickly? 
- Has the data scientist shared with you:
	- the types of variables you have?
	- the kinds of data analysis methods and models that could be used?
	- metrics for the data?
	- information on how to best curate the data?
	- information about missing data, erroneous data, and duplicative data?
	- information about potential bias in the dataset?
	- options as to how to go about solving issues in the data?
- Can you reach out to experts within the federal community, like the [Networking and Information Technology Research and Development Working Group on AI](https://www.nitrd.gov/nitrdgroups/index.php?title=AI?)

### Continuously test and evaluate prototypes

Developing AI solutions is an iterative process. Data scientists will run through a machine learning process, which includes creating training data, evaluating algorithm performance using test data, and trying different approaches and parameters to get the most accurate and usable output. Additionally, diverse teams will need to test and evaluate prototypes - and typically many iterations before you have working software that can be piloted with a group of users.\

Remember that a prototype may still be ready to be integrated into a service even if it doesn’t perform perfectly for all cases, so long as it performs really well for one case. For example, part of the job of the data scientist is to identify bias in the data or algorithm and communicate proactively with the agency project lead about how their work may favor one group over another.

Look for the team to describe iterations based on user-provided feedback and findings. These iterations integrate the data being used for training AI, the AI models applied, and the user experience. During the iteration and prototyping process, the team should be demonstrating their software on a regular cadence to leadership and the agency product owner. This will assist in getting to real software that can be piloted.

##### Checklist

- [ ] Use experts for identifying good training and testing data
- [ ] Collaborate with training data owners and model developers in order to understand the scope and suitability for the specific application
- [ ] Require the team to follow practices like the [Digital Services Playbook](https://playbook.cio.gov/), and the [Defense Innovation Board’s Detecting Agile BS Guide](https://media.defense.gov/2019/May/02/2002127286/-1/-1/0/DIBGUIDEDETECTINGAGILEBS.PDF)
- [ ] Ensure that the team is well integrated with the problem and data experts so that there is regular, efficient communication without requiring additional oversight or layers of access
- [ ] Ensure that the team can interview end-users without running into barriers like the [Paperwork Reduction Act](https://pra.digital.gov/)

##### Questions

- Does the team have access to the original training data owners and model developers?
- What would outputs of the AI model be compared against (e.g. non-AI process), and what are the proper accuracy metrics to use for such comparisons?
- What is the accuracy of the algorithm and is it sufficient given the user’s needs?
- How is user feedback factoring into the prototypes being developed by the team?
- Is the team demoing working software on a regular cadence?
- Does the machine learning model perform really well for at least one use-case?

## Culture and Education

AI involves different risks than just normal software. While many typical software development risks apply to AI projects, there are also a variety of different issues related to agency culture that can pose a risk. Education is key to addressing these risks.

### Identify key risks, including resistance

Every software project has a certain amount of inherent risk. We use agile as project management philosophy because we can’t predict the future. Here are some risks that are especially important to AI:

- Legacy infrastructure where sharing data is not technically easy
- Data that involve special handling, such as rules for the protection of personally identifiable information (PII)
- Data that require a substantial review period before any individual can access it
- Ambiguity and uncertainty about the quality of the data
- Biased data or algorithm processing
- No clear data owner, or person responsible for the quality of the dataset
- The data owner being unaware of the project
- Fear, uncertainty, and doubt over how an AI will fit with an existing workflow
- No communications plan with users about the impact of AI
- No communications plan with senior leadership about the purpose of the AI

The majority of these risks include culture change and work process change management elements. As such, good and timely communication is important, especially with the users affected by an AI tool, data owners, and leadership.

##### Checklist

- [ ] Work with a product manager to identify the risks associated with your project
- [ ] Proactively communicate with your projects’ stakeholders regarding risk
- [ ] Communicate regularly and proactively with users, senior leaders, data owners, and more
- [ ] Work with data owners and data scientists to understand the quality of data

##### Key Questions

- What will you need and from whom?
- What are the most likely reasons this effort would fail? 
- Have you identified everything you need to make this pilot a success?
- What is the minimum level of success this pilot needs? 
- Who are the most important people to communicate with?

### Assess and manage ethical concerns

The automation of government processes should not create a negative experience for citizens. This might include:

- Putting some groups at an unfair disadvantage over others
- Making it harder to find or access important information
- Breaching the privacy of citizens
- Creating feelings of discomfort or a sense that citizens are being monitored

ML approaches in AI are reliant on data to build predictive models. These models become part of decision-making pipelines which in turn become part of the software application with which users interact. If the data itself is biased, the software will reflect those biases.

Biased software can mean that vulnerable populations are discriminated against, as vulnerable populations are oftentimes statistically under- or over-represented in data. Bias may also occur outside of the domain of classical discrimination categories with which we are familiar as citizens. Bias can also occur when underlying variables take on mathematical significance or weight in an algorithm. This kind of bias could systematically skew decision-making related results of algorithms in ways that are hard to detect. Being cognizant of this possibility is important in order to test for and mitigate bias.

Ethical issues in a project should be identified as early as possible and considered throughout a project life-cycle; not just at the very end of a project or as a one-time event.

##### Checklist

- [ ] Understand where your data comes from. Know the ramifications on how trustworthy and unbiased the dataset itself is by talking with individuals responsible for its collection and management
- [ ] Fill out an [Algorithmic Impact Assessment](https://ainowinstitute.org/aiareport2018.pdf)(AIA) to determine the potential algorithmic risk for citizen harm (for example: [The Government of Canada’s AIA](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/responsible-use-ai/algorithmic-impact-assessment.html)). Revisit and update based on the problem being solved and throughout the lifecycle of the project
- [ ] Identify indicators of citizen harm and construct a plan to measure and report on those indicators regularly
- [ ] Work with data scientists to understand what your model’s error rate means for your software’s performance and the ramifications it could have on citizens
- [ ] Conduct user interviews with citizens to understand how current services work or don’t work for them, paying special attention to vulnerable populations. Use this information to better understand what your data for building a model might be leaving out
- [ ] Involve your agency’s privacy office in conversations around your plans for developing a new service. Work with them to identify privacy issues and have plans to mitigate them
- [ ] Be aware of the potential for the identification of citizens private information from the sharing of machine learning models, and consider partial sharing of code only

##### Key Questions

- Do you understand that your system, even if well- engineered, will make mistakes?
- From an ethics point of view, are you prepared for the occasional error by an AI system?
- Is the data scientist regularly communicating to the agency project team the implications of their work on the service?
- Does providing the service favor one group or another?
- Is a person on the team very knowledgeable about the data and the subject matter?
- Where does this data come from?
- How reliable are the reporting and collection methods?
- What are the current experiences of vulnerable populations interacting with the program, and how would this new service impact them?
- Is there appropriate human oversight and control of the system?
- Did you implement appropriate strategies to enhance privacy, such as training models on non-sensitive data, using encryption, etc.?
- Can a non-technical person on your team explain what your algorithm is doing?
- Did you take users’ preferences into account for accessing information, and ensuring that you have non-digital means to access the same information?

### Build support and educate senior stakeholders

AI is very much a new technology in the federal government. Senior leaders are often unaware of the technical details of implementation. Furthermore, your leadership in legal, finance, operations, security and more may be unfamiliar with AI. Beginning a project with a strong cadence of communication with these leaders establishes trust and begins to set expectations on what the pilot will look like.

Culture change is a team sport, and no pilot can accomplish this on its own. But, by showing what is possible with AI and setting expectations, you can increase the organization’s chance of a good experience. This means that the second project will be more likely to succeed.


##### Checklist

- [ ] Know what data you need and get the data owners bought in early
- [ ] Map agency mission to AI/ML resource requirements in a way that meets leadership accountability mandates 
- [ ] Be aware of trends in the market or academia where similar processes to your own have been advanced through new technology and use those as signposts for the future and to gain buy-in.
- [ ] Win over leadership to do a pilot, and build the pilot to demonstrate alignment and to win over leadership Share business problem findings with team and agency leadership

##### Key Questions

- Is the AI pilot structured to demonstrate unambiguously alignment with agency mission and data structures? 
- How is leadership invested in the AI pilot?
- Is the risk-of-loss tolerable to the agency should the AI prototype and/or pilot fail? 

## Run your pilot

Pilots take working software and typically test it with a substantial user segment. This gives development teams and leadership insight into how well the software works as a solution.

A pilot of AI should also involve live data, where the algorithm and the software are both integrated into a user’s workflow. During a pilot phase, evaluate the success of the model to ensure that the outputs are understood by the users. Collect user feedback and ensure that the feedback is relayed to the entire team and used in the next iteration of the software.

### Have a clear plan

Before actually running the pilot, have a clear plan. Running a pilot that yields results that are not actionable could be a tremendous waste of resources and time. Decide beforehand what the important metrics are for evaluating the software and algorithm you are piloting. Refer back to the original business problem and user needs you identified.

Also, it’s important to consider how you’ve set up your system to collect feedback. For example, you may wish to conduct user interviews during the pilot to continuously collect user needs and new user stories. You should look carefully at employing monitoring analytics to collect quantitative measures of user actions. Finally, it is important to measure model results with test dataset and accuracy metrics.

##### Checklist

- Know your important metrics for success, both technical (things like performance) and non-technical (the user needs)
- Have a clear plan in place for monitoring the performance of the algorithm and the usability of its outputs
- Document the results of the pilot for further learning and evaluation by the software team
- Continue to collect user needs and turn them into user stories during the pilot phase

##### Questions

- What are the hypotheses being tested in this pilot?
- What are the key metrics?
- How are key stakeholders being involved and informed of the pilot?
- What is the plan for documenting and sharing the results of this pilot?
- How will the pilot results inform future iterations?

### Create standards for measuring the performance of models

The approach used for training and testing should be designed for the AI from the beginning of the piloting process. This typically involves a gold-standard dataset, often annotated by experts or via crowdsourcing, that can serve as basis for measuring model performance. It is essential to evaluate your AI algorithm using a testing dataset that is different from the training set used to build the AI model. This ensures that the AI model can be readily applied to other situations with similar accuracy. It can involve obtaining models from external organizations and testing them for accuracy on previously unseen data. To ensure adequate testing, agencies and/or trusted third parties may play a role to ensure trusted independent testing is performed. Having a common platform and metrics for testing also ensures that accuracy results are trustworthy and comparable across various solutions being compared. Either way, the key is to have some data kept for testing that is not used in the training process.

Working with industry is useful to understand broader sets of use cases, and challenges/sprints can enable comparisons of different models to be tried and tested for different types of applications. Sometimes, data is located on different servers and cannot be combined into a central database due to privacy or other concerns. In such cases, federated approaches may be useful, whereby computing is done on local servers and then resulting analysis is shared with others. This can enable AI results to be combined from data across sites in ways that protect access of the individual server’s data by outside users (e.g. for privacy).

##### Checklist

- [ ] Develop a model evaluation plan at the beginning of the design process
- [ ] Consider creating a gold-standard dataset annotated by experts that can serve as basis for measuring model performance
- [ ] Release only a subset of a gold-standard dataset for training purposes by external parties/vendors, keeping some for testing of model performance. Alternatively, if the training data is readily available, consider saving the gold-standard dataset for training and use it only for testing purposes to evaluate the accuracy of the tools created
- [ ] For testing models, compare model-predicted results with results from gold-standard datasets
- [ ] Define accuracy metrics used in the evaluation process
- [ ] Iterate on algorithms using human input to tweak performance on training datasets (while keeping testing data separate)
- [ ] Evaluate the relative weight of various features of the model for a quick sanity check and explore explain- ability to see if follows human intuition
- [ ] Do sensitivity analysis to understand how data variations can affect predictions

##### Key Questions

- Unless you are doing unsupervised learning, do you have enough labeled outputs for the model to learn from?
- Can you pay someone to repeat the manual task over and over to generate the outputs?
- Are there standard training/testing datasets already available in the agency or externally?
- Can a third party do independent model testing (in which case gold-standard test data would be given to a third party)?
- Is the model explainable?
- What accuracy metrics best represent user needs?

### Know and follow the relevant laws to your project

An AI algorithm is software code that processes data. AI and other types of automation (including RPA) are not entities or agents that have the rights of a human being. Agencies should expect to comply with all existing laws and policies with respect to data and software. Whether an agency may be constrained in the use of AI algorithms may depend on the consent and privacy laws governing the use of the data that was collected.

##### Checklist

- [ ] Understand what data protection questions need to be answered before implementing a machine learning algorithm or building a dataset. For example, building a training set by extracting data programmatically from websites (a legally grey area)
- [ ] Identify any laws and policies that would be impacted by implementing an algorithm
- [ ] Consult early with Legal and Privacy Officers, and bring data owners to these early conversations in order to discuss protections around the information being collected and used
- [ ] Remember that the appropriate privacy, civil liberties, and/or legal advisors for the department or agency are part of your stakeholder ecosystem

##### Key Questions

- What are the roles and responsibilities for the pilot?
- What are the laws and policies that impact this algorithm?
- What are the key privacy issues?
- What information protection questions need to be answered?

## Post pilot: Now what?

You’ve run your pilot. You’ve collected valuable user feedback on how useful your tool is. Your tool is using live data. What do you do now?

### Consider the long-term investment strategy

In the short-term, a pilot needs to test the foundational ideas and hypotheses discovered in the user research, as well as get a better sense of the technical feasibility of the path.

However, long-term considerations are a bit different. Long-term, you will need to:

- Have a sound plan for managing the data used by the AI model
- Have a plan for updating the software
- Ensure the quality of the AI outputs
- Develop a strategy for AI procurement
- Address the integration of AI into your workflow long term with training and education

You may also need alternative infrastructure and services, like a specialized chip-based (Graphics Processing Unit) or cloud-based environments for processing data and running the models. AI takes significantly more computing power than traditional software applications because the amount of the data being modelled continuously and at high speeds. Consider infrastructure needs based on the quantity of data that must be processed and stored, and the speed of access/transfer required. For computations, understand the computational complexity and ability for parallelization of the algorithms/models to determine the speed and quantity of processors needed as well as memory requirements.

AI may not be a possible solution if the infrastructure within which you are deploying it can’t keep up with the requirements needed to provide a good user experience. Other investments in talent and education may also be needed.

##### Checklist

- [ ] Determine whether AI can be supported on your current infrastructure
- [ ] Understand if there will be resources for this project after the pilot ends if it is successful
- [ ] Roughly scope out the various needs (technical, data, human) if your pilot is successful

##### Questions

- What kind of resources can this project expect if the pilot is successful?
- How is your infrastructure suited for AI?
- What are you seeking to optimize in your long-term strategy- cost, building in-house technical capacity, agility to quickly implement new projects, performance on single large projects?
- Do you have a sustainable business model?

### Lay the seeds for future experimentation

In order to steward artificial intelligence in the government, we need professional data scientists. However, we also need a trained non-data science workforce that is capable of identifying opportunities within their own workflow for automation or data pattern recognition, who can think ahead to the future, evaluate vendors, and manage teams that may include data scientists and software engineers.

Developing in-house talent is about recognizing that automation, data, and software are changing the way government does its work. To be proactive, thoughtful, and effective stewards of this work, it is important that agencies look at how it can [grow these skills within their own walls](https://strategy.data.gov/action-plan/#action-14-identify-opportunities-to-increase-staff-data-skills). AI is a discipline that includes statistics, computer science, and software engineering. Technical staff with a background in at least statistics are often capable of learning more computational approaches.

##### Checklist

- [ ] Identify individuals with experience conducting web analytics, doing statistical analyses or economic analyses using statistical processing methods, managing major databases, and working as data architects
- [ ] Give talented technical experts a few hours each week to explore problems that interest them outside their day-to- day tasks. Ask them how they might solve those problems, and consider how you might provide them resources if they present a compelling business case
- [ ] Encourage technical experts to take online training courses like Coursera, MIT Opencourseware, Edx, and others to enhance their existing skill sets with new ones. Encourage the use of open source packages and libraries like R, Python, Keras, Pytorch, and sci-kit learn to promote literacy in industry-standard tools, avoid black-box tools where it is difficult to de-engineer how a given software tool made a decision, and get to prototype faster than traditional procurement
- [ ] Consider how internal classes taught by more experienced technical staff can enhance the skills of less experienced staff and promote greater data and AI literacy and understanding
- [ ] Explore whether budgetary set-asides are permitted to fund innovation, experiments, and prototype development

##### Key Questions

- What skills do you have in your agency currently in statistics, informatics, analytics, mathematics, computer science, and software engineering?
- Have you given your talented technical people time to experiment with new tools and grow?
- Have you considered setting up data science guilds, classes, or workgroups taught by more experienced internal staff?
- Have you considered internal hackathons or data science challenges to give technical staff time to identify their own problems and solve them?
- Does your agency culture prioritize internal innovation or is it focused on acquiring market-driven solutions?

### Case Study: Census Bureau

#### Classifying free-text product descriptions using machine learning

The Commodity Flow Survey (CFS), a joint effort between the Bureau of Transportation Statistics and the Census Bureau, produces estimates of shipment activity and the flow of goods nationwide. In 2018, CFS implemented a machine learning process to improve data quality as well as reduce operational costs and respondent burden. In particular, CFS has implemented a machine-learning based "autocoder" to classify free-text product descriptions provided by respondents. Using this autocoder, CFS has successfully labeled or relabeled codes for approximately 200,000 records from the 2017 CFS. This has improved production data quality and the resulting estimates, while simultaneously reducing respondent burden and costs.

##### Assessing impact of changes

One important facet of implementing any AI/ML process is understanding the potential bias and “downstream impact” of introducing a new methodology. In the case of CFS, the team wondered how potentially reclassifying product types might affect estimates of product movement throughout the country. An early version of the model was particularly good at classifying products in food-related product categories, and less good at classifying into other categories (e.g. machinery or electronics). The team wondered if this would bias final estimates toward food-related shipment activity. However, upon further investigation, the team found that when predicting food categories, the ML exhibited both high precision and high-recall; in other words, it was capturing the "universe" of food-related product shipments and therefore helping correctly apportion food-related shipments vs. other shipment activity.

###### Going to production early

At first, the CFS team saw potentially concerning accuracy numbers: around 50%. However, upon leveraging the model's measure of its confidence in the prediction, the team found that highly confident predictions were far more accurate -- around 90%. By limiting predictions / updates to just this subset of highly confident predictions, the CFS team found that it both had a deployable "production-ready" model and a path forward to improve the model by working to increase the proportion of high-confidence predictions. Practitioners, especially those with research backgrounds, can often become focused on developing a "perfect" model before going to production, even when something production-grade may exist under the right constraints without deeper research.
                

### Appendix I: Definition of Terms

**Artificial intelligence** (AI): The field of computer science that deals with the simulation of intelligent behavior in computers or the capability of a machine to imitate intelligent human behavior. It is used broadly to refer to any algorithms, methods, or technologies that make a system act and/or behave like a human and includes machine learning, computer vision, natural language processing, cognitive, robotics, and related topics.
 
**Machine learning** (ML): A technique within the field of artificial intelligence which uses algorithms that automatically improve with experience or “learn” without being explicitly programmed. Machine learning is the application of AI techniques using statistical methods that enable machines to improve correlations as more data is used in the model, and for models to change over time as new data is correlated. Machine learning evolved from the connectionist theory of human cognition, pattern recognition, and computational learning theory. Approaches include neural networks and deep learning. 
 
**Algorithm**: A set of mathematical rules, that if followed, will give a prescribed result. Some of the common algorithms used in AI/ML include Bayesian networks, clustering, decision tree learning, reinforcement learning, and representation learning. 
 
**Model**: A set of instructions or recipe that a computer uses to turn data into a decision or output (i.e., is this picture a fake or real?).
 
**Pilot**: Pilot projects can have a broad definition and set of criteria across the U.S. federal government. With respect to this guide, an AI pilot should meet the following criteria: 
- AI models are running, learning from data, and helping to make decisions
- There is a framework in place to evaluate the effectiveness of the AI models
- A selection of the public can interact with the service and provide feedback
- Evidence is gathered as to whether the service meets user needs
 
**AI lifecycle**: A set of phases in which a ML model is integrated into the organization’s software development process. For more on the AI lifecycle, read this blog post by Google on [Making the Machine: The Machine Learning Lifecycle](https://cloud.google.com/blog/products/ai-machine-learning/making-the-machine-the-machine-learning-lifecycle).
 
**Data science**: A process by which raw data is turned into business insights. This includes data cleaning, debugging, and “munging,” data mining, and finally delivering actionable insights. 
 
**User journey**: The major interactions shaping a user’s experience of a product or service.
 
**Agile**: A way of thinking and attacking problems that embraces iteration, failing quickly, and learning. Agile typically involves practices like standups, retrospectives, sprints, sprint planning, backlog grooming, transparency of information,  self-organizing teams and more. Agile is not a checklist though. A team can have all these practices and not be agile. Good signs include valuable software being shipped at the end of every sprint and the team receiving continuous user feedback. For more read the [Defense Innovation Board’s Guide: Detecting Agile BS](https://media.defense.gov/2019/May/02/2002127286/-1/-1/0/DIBGUIDEDETECTINGAGILEBS.PDF).
 
**Gold-standard dataset**: A dataset that is highly curated, often by experts to evaluate machine learning models that have been fully trained. As opposed to the training data, this data the model never sees. In a competitive award process, agencies can use gold-standard datasets to evaluate the performance of different vendors to decide a winner. 
 
**Data provenance**: The record trail and historical context for a piece of data. A measure of data quality.
 
**Data accuracy**: Whether the data itself is correct. A measure of data quality.
 
**Data validity**: The extent that the data reflects the real world. A measure of data quality.
 
**Data uniqueness**: The extent that the data does not contain any duplicates. A measure of data quality.
 
**Data completeness**: A measure of how much critical data is available relative to all of the data available for a given a business case.
 
**Synthetic data**: Data that is generated by computer code. Usually used in place of real data for model training if that data has special protections or is difficult to come by. 
 
**Robotic Process Automation** (RPA): Robotic Process Automation (RPA): A technology platform that enables a software robot to interact with applications. RPA software can be easily programmed to do basic tasks across applications just as human workers do. The software robot can be taught a workflow with multiple steps and applications such as taking received forms, sending a receipt message, and checking the form for completeness. RPA software is designed to reduce the burden of repetitive, simple tasks on employees. RPA technology can automate many common data entry activities that can include invoice entry, human resources personnel action entry, and data verification.
 
**Supervised Machine Learning**: In supervised machine learning, a model is given data that is labeled in an organized fashion by a subject matter expert. Once enough structured and labeled data is provided, the AI model built can recognize and respond to patterns in data without explicit instructions. The output and the accuracy of supervised learning algorithms are easy to measure. Supervised learning is a common method of machine learning today.
 
**Unsupervised Machine Learning**: A model is given data that are not labeled in an organized fashion. For example, one might provide pictures of animals (cats, dogs, etc.) without any labels. The model organizes items into logical groupings based on patterns recognized by the model. This method is used to identify underlying patterns from previously unstructured data. The expectation is not to derive the right output but to explore datasets and draw inferences. Unsupervised learning is often applied to cases where the researcher or user does not already know the significant structures or relationships among the data.

### Appendix II: Additional Resources

#### Identifying the problem and evaluating the approach

- [Digital Services Playbook] (https://playbook.cio.gov/)
- [18F Method Cards] (https://methods.18f.gov/)
- [AI Self Assessment Checklist] 
- [What Great Data Analysts Do -- And Why Every Organization Needs Them](https://hbr.org/2018/12/what-great-data-analysts-do-and-why-every-organization-needs-them)
- [De-risking Custom Technology Projects](https://github.com/18F/technology-budgeting/blob/master/handbook.md#footnote-2)
- [A Guide to Using Artificial Intelligence in the Public Sector](https://www.gov.uk/government/collections/a-guide-to-using-artificial-intelligence-in-the-public-sector)
- [DIB Guide: Detecting Agile BS](https://media.defense.gov/2019/May/02/2002127286/-1/-1/0/DIBGUIDEDETECTINGAGILEBS.PDF)

#### Culture and Education

- [Scientific American AI Glossary](https://science.sciencemag.org/content/357/6346/19)
- [Understanding artificial intelligence ethics and safety](https://www.gov.uk/guidance/understanding-artificial-intelligence-ethics-and-safety)
- [OECD AI Principles](oecd.org/going-digital/ai/principles/)
- [Algorithmic Impact Assessments: A practical framework for public agency accountability](https://ainowinstitute.org/aiareport2018.pdf)
- [Government of Canada Algorithmic Impact Assessment](https://ainowinstitute.org/aiareport2018.pdf)
- [AI Principles: Recommendations on the Ethical Use of Artificial Intelligence by the Department of Defense](https://media.defense.gov/2019/Oct/31/2002204459/-1/-1/0/DIB_AI_PRINCIPLES_SUPPORTING_DOCUMENT.PDF)

#### Run Your Pilot

- [Planning and preparing for artificial intelligence implementation](https://www.gov.uk/guidance/planning-and-preparing-for-artificial-intelligence-implementation)
- [Managing your artificial intelligence project](https://www.gov.uk/guidance/managing-your-artificial-intelligence-project)
- [ACT-IAC AI/ML Primer](https://www.actiac.org/system/files/Artificial%20Intelligence%20Machine%20Learning%20Primer.pdf)
- [Making the machine: the machine learning lifecycle](https://cloud.google.com/blog/products/ai-machine-learning/making-the-machine-the-machine-learning-lifecycle)

#### Post - pilot: Now what?

- [Guidelines for AI Procurement, World Economic Forum 2019](https://www.weforum.org/whitepapers/ai-government-procurement-guidelines)
- [U.S. Federal Data Strategy: Action 14](https://strategy.data.gov/action-plan/#action-14-identify-opportunities-to-increase-staff-data-skills)
- [ACT-IAC AI Playbook](https://www.actiac.org/act-iac-white-paper-artificial-intelligence-playbook)

