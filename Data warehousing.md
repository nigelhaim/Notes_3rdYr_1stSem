2023-08-14

Prof.  Jessie James P. Suarez

Lab and lecture are switch 

Grading system 

20 prelim 
20 Finals
20 Lab
10 quiz activities 
30 project
- Final project would be tackling a machines learning problem and analyzing the results of the model 
- the expected output is code and paper detailing the method experiments and results 

One of the main issues in handling data
- Many source
- Messy data 

## Data warehouse
- central repository off integrated data
	- AVOID Stored in different file types (Excel, SVG, txt)
	- single source of truth
- backbone for reporting, data analytics, decision support
	- Reporting
		- Helps in decision making
		- Mostly in the form of dashboards
		- Example 
			- Netflix on genres
	- Data analytics
		- Gathering insight from the reported data
		- Interpretation of data 
		- Examples 
			- Number of active users
	- Decision support 
		- Decision making of the organization/company

### "One of the most important assets of any organization is its information. "

#### Why is Data warehouse important?
- Ensure consistency
	- Standardize data from different sources
	- reduces the risk of error
	- Application of uniform format 
- Make better decisions 
	- improving the speed and efficiency of accessing different data sets 
- Improve their bottom line 
	- Quickly access their organizations historical structures and evaluate initiatives that have been successful or unsuccessful in the past. 
	- Does the promo work in the past?

Themes
- "We collect tons of data, but we can't access it."
- "We need to slice and dice the data in every which way."
- "Business people need to get the data easily"
	- Easy interpretation of data even the ones who cannot understand the technicality behind.
- "Just show me what is important"
- "We spend entire meetings arguing about who has the right number rather than making decisions."
- "We want people to use information to support more fact-based decision making."


Data must make the information easily accessible 
- Understandable 
- Obvious 
- To anyone 

Data must presented information consistently 
- Credible 
- easily manipulated 
- cleansed
- quality assured 

Data must adapt to change
- Since data are all subject to change......data is needed to be 
- Handle inevitable chance gracefully
- Does not invalidate existing data or applications

Data must present information in timely way 
- Raw data needed to be converted into actionable information within a specific amount of time 

Data must be secure bastion that protects the information assets 
- crown jewels are stored in the data warehouse 

Data must serve as the authoritative and trustworthy foundation for improved decision making 
- right to support decision making 
- decisions that are based on the analytic evidence presented 

Data must be accepted by the business community to deem it successful 
- built an elegant solution using best-of-breed products and platforms. 

By definition 

Databases
- Online  transactional processing 
	- Delete, insert, replace and update 
Data Warehouses 
- Online analytical processing 
	- Analyze massive volumes of data rapidly 
	- Look at your data from different points of view

Cloud Tools 
- Amazon redshift
- Azure 
- Google BigQuery 

Databases
- PostgreSQL 
- IBM DB2
- MySQL

Tools insertion, extraction, and moving of data 


Topics
- Concepts and architecture for data warehouses
- data modelling life cycle 
- Dimensional modelling life cycle Dimensional data modelling 
- Extraction, Transformation, and load
- Visualization and descriptive analytics 
- Emerging technologies

2023-09-07

## Data models and Data Warehouse Architectures 

### Data Modeling 
- Creates a visual representation either a whole information system or parts of it to present connections between data points and structures. 
- The importance of entities and attributes 
Different types of data models? 
	- **Conceptual**
		- Defines what the system contains 
		- Domain models
		- Offer a big-picture view of what the system will contain and how it will be organized
		- Usually created as parts of the process of gathering initial project requirements
		- The high-level parts of the database without it there is no system
		- The objective of the system
			- A user is able to do an event 
			- A model in the system can interact through events 
			- What problem are you trying to solve? 
		- Usually developed or created by Business Stakeholders or Data Architects in the organization
	- **Logical** 
		- This type of data model defines how the system should be implemented regardless of the **Database Management system**
		- They are **less abstract** and provide greater detail about the concepts and relationships in the domain under consideration 
		- **Indicates** data attributes, such as data types and their corresponding lengths, and show the relationships among entities.
		- Typically developed and created by Data Architects and Business Analysts in the organization
		- Information that represents the data model 
		- Can be changed through events
		- Get the necessary information of the model before an event happens
		- Can be obtained through data gathering (interviews)
	- **Physical**
		- Defines how the system should be implemented with a specific Database Management System 
		- Provide a schema for how the data will be physically stored within a database. As such they are the least abstract of all
		- These data models can include database management system (DBMS) - specific properties, including performance tuning 
		- Typically created by Database Administrators and Developers 
		- The different syntaxes, definitions and limitations 
		- Respect to the Hardware from implementing the software 
		- The data is complete 
### Data Architecture 
- Describes how data is managed from collection through to **transformation, distribution, and consumption.** It sets the blueprint for data and the way it flows through systems. 
- **Transformation** - Is there any transformation we are trying to do in the system? 

| Dimensions | Data Model  | Data Architecture |
| --- | --- | --- | 
| **General Definition** | Activity within data architecture | Broader; Encomapsses data management | 
| **Focus Area(s)** | Focus on detailed data representation | Focus on data collection, storage, governance | 
| **Role in Data management** | Ensures precise data design and integrity | Responsible for data infrastructure setup | 
| **Roles and Responsibilities** | Collaboration of data architects and admins | Collaborating of both data teams and stakeholders | 
| **Abstraction** | Lower level of abstraction; more specific | Higher level of abstraction | 
| **End Goal** | Implements data architecture effectively | Provides data strategy and framework | 

### Different Datawarehouse Architecture
- Method of defining the overall architecture of data communication processing and presentation that exist for end-clients computing within the enterprise.
- **Inmon** Architecture (1922) 
  **Kimball** Architecture (1996)
  **Data Vault** (2013)
- How to show data on the dashboard 
#### Inmon (Corporate Information Factory )
- "A data warehouse is a subject-oriented, integrated, time-variant and non-volatile collection of data in support of management's decision-making process"
	- Bill Inmon
- ##### Necessary Attributes of a Data Warehouse
	- **Subject oriented **
		- Data collected relates to a particular subject rather than a particular action 
		- The warehouse has respect to the subject
	- **Non-Volatile **
		- Once information is saved in a Data Warehouse, it should stay there 
		- It should be secured 
		- We should not delete anything or at all 
	- **Integrated**
		- Data is standardized no matter how it stored in the source system 
		- What is reflected in the where house is also reflected in the system 
	- **Time-Variant**
		- Data collected and stored  in the Data Warehouse changes with time
		- Big data must be stored and processed in time despite of the high traffic 
- **Inmon's Approach**
	- Start with the corporate data model. Identify all the different sources of available to the enterprise 
	- From the data and understanding of business needs, identify the key entities and their mutual relationships
		- What does the business need and what are the key entities? 
		- Information about everyone that could be included in the operation 
	- Use the entity structure to build a detailed logical model. The is should captured in create detail all need information 
	- Build the physical model. Use ETL (Extract Transform Load) processes. The Normalized data model (3NF) is the core 
		- How do we use a specific language to communicate in the database and show the data 
	- Build data marts for specific departments. The Data warehouse acts as a single source of truth
		- **Data marts** - Smaller warehouse for the specific department not everything is shown in the database...

### Recap 
- 1NF: Each table cell should contain a single value, and each column should have a unique name 
- 2NF: Each column should be directly related to the primary key, and not other columns 
- **3NF: This means that each column should not be related to any other columns in the same table**

| Advantages | Disadvantages |
| --- |---|
|**Flexibility** - It is because of the ETL process design that leads to normalized data| **Cost and Setup** - Normalized schemas exhibit greater complexity in design and maintenance | 
| **Less Prone to Errors** - Normalization avoids data redundancy | **Skills Needed**- The approach necessitates highly skilled engineers |
|**Completeness** - This approach covers all enterprise data so all  | **More ETL Required** - Because of separating the Data marts from Data Warehouse |

#### Kimball (Dimensional Modelling)
- The latest for data warehouses mostly used for the past few years
- Kimball focuses on the purpose of a Data Warehouse: "a copy of transaction data specifically structured for query and analysis"
	- Ralph Kimball
##### The purpose of a Data Warehouse
- **Collection**
- **Transformation**
- **Load**
- **Knowledge**

**Kimball's approach**
- Understand and document the business processes, business needs, and business questions being asked. 
- Document all data sources available throughout the enterprise 
- Build ETL pipelines that extract, transform, and load data into a denormalized data model 
- The dimensional model is usually built around and within dimensional data marts for specific departments 

|Advantages|Disadvantages|
|---|---|
|**Simplicity & Speed** - The architecture is much simpler and faster to design and set up|**Data Redundancy** - Because data is loaded into a dimensional model it is not normalized |
|**Understandable & Relevance** - Easy to understand and gears answer organization needs |**No single source of truth** - The warehouse is designed and organized around data marts|
|**Skills needed** - Requires less number of highly skilled engineers and less technical knowledge |**Less Flexible and incomplete** - Due to "as-needed" paradigm and is specific to needs |

2023-11-09

#### Dan Linstedt (Data Vault)

"A **detail-oriented** , **historical tracking**, and **uniquely linked set** of normalized tables that support functional areas of the business. It is **hybrid approach** of 3NF and Star Schemas" - Dan Listedt

##### The pillars of a Data Vault:
- **Methodology** - Emphasis on Agile principles and practices. Involves incremental delivery, continuous integration and adaptability to changes.
	- Incremental - Waterfall
	- Continuous integration - Git is the best example. 
	- Adaptability to changes - Do not plan the entire scenario
- **Architecture** - Focuses on the systems and structures that handle and store data it combines **best of 3NF and start schema techniques**

**Lundstedt's Approach**
- Identify the **Core Business Concept**. Need to select a grain of abstraction that the organization is using 
- Create a **Raw Vault** by identifying the core concepts for the architecture which are Hubs, Links, and Satellites 
- ETL to first add Hubs for defining business IDs, followed by Links, and then additional data through satellites

Encrypt Necessary IDs as dedicated from maintaining security and privacy 
Data Marts are used as

| Advantages  | Disadvantages|
|---|---|
|**Incremental Builds** - since the architecure adapts an Agile approach, it is more adaptable to change |**Added Overhead** - Because of the added complexity, for fewer data sources, it is not idea|
|**Data Lineage** - through the core concepts, the vault keeps track of the historical data | **Explosion of tables** | 
| ||
|||


## Kimball Lifecycle and Dimensional Modelling

**Program/Project Planning**
- Ano gusto sa life 
**Business Requirements Definition**
- If you do not use the right tools to solve the problem it is useless
- Ano plano mo gawin in life
**Top Track/**
- Implement in life
**Middle Track/Data Track**
- Enough ba si python/java...?
**Bottom Track/Bi Application Track**
- Dashboards, admin page 
- Ano itsura ng front end 
**Deployment**
- Production ready software 
- Tested, WIdthstand mutliple request, and bugs 
**Growth**
- As the business gets bigger, the data too
**Maintenance**
- How you solve problems along the way

#### Program/Project Planning and Management 

**What is a lifecycle**
- **Customer Expectations**
- **Completion within times**
	- Fishbone 
	- Requirements 
	- Why in this certain amount of time? 
		- Too late for the competitors? 
- **Cost estimates**
	- The cost to make a project
		- Devleopers, Maintenance

**The DW/BI initiative begins with a series of program and project planning activities**
- Asses Readiness
	- Business Sponsor 
		- A backer for the project 
		- Makes the project worth it 
		- Someone from the top that backs the developer
	- Business motivation
		- What is the return? 
		- What is it for me? 
		- Something compelling to gain support 
	- Feasibility 
		- Resources needed
		- If data is not feasible there is no sense of data warehousing 
- Scoping and Justification 
	- The limitations and kung ano lang kaya gawin ng developers 
	- Justification
		- The cost
		- Benefits 
		- The time to develop 
	- Impact
		- The cost of life 
- Staffing 
	- Who are involved? 
	- Opportunities for newly Grads 
	- Business Roles 
		- Business Sponsor - Form the top
		- Business Driver - the henchmen 
		- Business Lead - the leader of  the business
		- Business Users - customer 
	- IT 
		- Business Analyst - translates busniess to technical 
		- Data Steward 
		- 
- Developoment and matintaining the plan 
	- The project manager does not makes the estimates
	- Are we actually accomplishing something? 
	- Scope creep - A small bump on the scope making it bigger to satisfy the business requirements
	- Zero-sum - What should I stop doing it? Gaining control on the scope agreement

#### Business requirments definition

**Collaborating with business users to understand their requirments and ensure their buy-in**
- Requirements planning 
	- **Choose the Forum**
		- Ask the right person on the requirements 
	- **Identify the Req. Team**
		- Should be accompanied with the same language 
	- **Select, Schedule, Prep. Business representatives**
		- Prepare for the impact for the business
		- Make sure everyone is on the same page 
	- Don't waste your/someone's time 
- Collect Business Reaquirements
	- **Launch**
		- Someone needs to talk about the primary talking point
		- Someone at the beginning to states the purpose
	- **Interview flow**
		- The flow of the conversation
		- Flow vs time restraint
	- **Wrap up**
		- The final minutes of the meeting 
		- Saying everything what has been agreed during the meeting 
		- Success criteria 
- Documenting Requirements
	- Describe why needs the users 
	- What features
	- List down everything 
- Prioritize requirements 
	- Least effort more impact first 

##### Technical Architecture Design
- I need an app for this 

##### Product Selection and Installation
- Approvals
- Buy products for organization 
- 