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
- **Ensure consistency**
	- Data warehouses are programmed to apply a uniform format to all collected data. Standardizing data from different sources also reduces the risk of error in interpretation 
	- Standardize data from different sources
	- reduces the risk of error
	- Application of uniform format
- **Make better decisions**
	- Successful leaders develop data-driven strategies and rarely make decisions without consulting the facts. Data Warehousing improves the speed and efficiency of accessing different data sets
	- improving the speed and efficiency of accessing different data sets
- **Improve their bottom line**
	- Data warehouses allow leaders to quickly access their organization's historical activities and evaluate initiatives that have been successful or unsuccessful in the past. 
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

#### Goals and objectives of a data warehouse 
**Data must make the information easily accessible**
- The contents of the DW/BI system must be understandable. The data must be intuitive and obvious to the business user, not merely the developer.
	- Understandable 
	- Obvious 
	- To anyone 

**Data must presented information consistently**
- The data in the DW/BI system must be credible. Data must be carefully assembled from a variety of sources, cleansed, quality assured, and released only when it is fit for user consumption.
	- Credible 
	- easily manipulated 
	- cleansed
	- quality assured 

**Data must adapt to change**
-  User needs, business conditions, data, and technology are all subject to change. The DW/BI system must be designed to handle this inevitable change gracefully so that it doesn’t invalidate existing data or applications
	- Since data are all subject to change......data is needed to be 
	- Handle inevitable chance gracefully
	- Does not invalidate existing data or applications

**Data must present information in timely way**
- As the DW/ BI system is used more  
intensively for operational decisions, raw data may need to be converted into actionable information within  
hours, minutes, or even seconds.
- Raw data needed to be converted into actionable information within a specific amount of time 

**Data must be secure bastion that protects the information assets**
- An organization’s informational crown jewels are stored in the data warehouse.
- crown jewels are stored in the data warehouse 

**Data must serve as the authoritative and trustworthy foundation for improved decision making** 
- The data warehouse must have the right data to support decision making. The most important outputs from a DW are the decisions that are made based on the analytic evidence presented
- right to support decision making 
- decisions that are based on the analytic evidence presented 

**Data must be accepted by the business community to deem it successful**
- It doesn’t matter that you built an elegant solution using best-of-breed products and platforms.
- built an elegant solution using best-of-breed products and platforms. 

**By definition **

Databases
- Online  transactional processing 
	- Delete, insert, replace and update 
Data Warehouses 
- Online analytical processing 
	- Analyze massive volumes of data rapidly 
	- Look at your data from different points of view

| Area of comparison | OLTP | Data warehousing | 
| --- | --- | --- | 
| System Purpose | Support operational processes | Support strategic analysis, performance, and exception reporting | 
| Data usage | Capture and maintain the data | Exploit the data | 
| Data validation | Data verification occurs upon entry | Data verification occurs after the fact | 
| Update frequently | Data is updated when business transactions occur (e.g., client uses debit card, web order is placed)| Data is updated by periodic, scheduled processes | 
| Historical data requirement | Current data | Multiple years of history | 
| Data integration and balancing | Data is balanced within the scope of this one system | Data must be integrated and balanced in multiple systems | 


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

![[Pasted image 20230912142358.png]]
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
- **Modelling**- Emphasized on the represetnation of data. Enusres that the data remains **consistent**, **resilient**, and **accessible**, even in complex environment 
**Lundstedt's Approach**
- Identify the **Core Business Concept**. Need to select a grain of abstraction that the organization is using 
- Create a **Raw Vault** by identifying the core concepts for the architecture which are Hubs, Links, and Satellites 
- ETL to first add Hubs for defining business IDs, followed by Links, and then additional data through satellites
- Encrypt necessary IDs as needed for maintaining security and privacy 
- **Data Marts** are used as a presentation layer since the Data Vault has many connections 

Encrypt Necessary IDs as dedicated from maintaining security and privacy 
Data Marts are used as

| Advantages  | Disadvantages|
|---|---|
|**Incremental Builds** - since the architecure adapts an Agile approach, it is more adaptable to change |**Added Overhead** - Because of the added complexity, for fewer data sources, it is not ideal|
|**Data Lineage** - through the core concepts, the vault keeps track of the historical data | **Explosion of tables** - Explosion on the number of tables compared to 3NF due to core concepts | 
|**Quicker and Easier ETL** - The approach allows parallelizable because of the core components |**Not Focused on Performance** - Large number of relationships making more complex joins|

## Kimball Lifecycle and Dimensional Modelling
![[Untitled-1.png]]

**Program/Project Planning**
- Assesses the organization's readiness for a DW/BI initiative, establishes the preliminary scope and jsutification, obtains resources and launches the program/project
- Ano gusto sa life 
**Business Requirements Definition**
- Aligning the DW/BI initiative with business requirements is absolutely crucial. Best of breed technologies won't salvage a DW/BI environment that fails to focus on the business. 
- If you do not use the right tools to solve the problem it is useless
- Ano plano mo gawin in life
**Top Track/Technology Track**
- establishes the overall framework to support the integration of multiple technologies. Using the capabilities identified in the architecture design as a shopping list, you then evaluate and select specific topics
- Implement in life
**Middle Track/Data Track**
- Begins by translating the requirements into a dimensional model. The dimensional model is then transformed into a physical structure. The focus is on performance tuning strategies, such as aggregation, indexing, and partitioning, during the physical design. Last but not least the, ETL system
- Enough ba si python/java...?
**Bottom Track/Bi Application Track**
- The design and development of the BI applications. The DW/BI project isn't done when you deliver data. BI applications, in the form of parameter-driven templates and analyses, will satisfy a large percentage of the business users' analytic needs
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
The SDLC aims to produce a high-quality software that meets or exceeds customer expectations, reaches completion within times and cost estimates. 
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

#### The DW/BI initiative begins with a series of program and project planning activities
- **Asses Readiness**
	- The most critical readiness factor is to have a strong executive business sponsor. Business sponsors should have a clear vision for the DW/BI system’s potential impact on the organization. Optimally, business sponsors have a track record of success with other internal initiatives.
	- The second readiness factor is having a strong, compelling business motivation for tackling the DW/BI initiative. This factor often goes hand in hand with sponsorship. The DW/BI project needs to solve critical business problems to garner the resources required for a successful launch and healthy lifespan.
	- The third factor when assessing readiness is feasibility. This includes technical and resource feasibility, but data feasibility is the most crucial. Data feasibility is a major concern because there is no short-term fix if you’re not already collecting reasonably clean source data at the right granularity.
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
	- Scoping requires the joint input of the IT organization and business management. The scope of a DW/BI project should be both meaningful to the business organization and manageable for the IT organization.  
	- Justification requires an estimation of the benefits and costs associated with the DW/BI initiative.  Hopefully, the anticipated benefits grossly outweigh the costs. IT usually is responsible for deriving the expenses.  
	- Delivering “a single version of the truth” or “flexible access to information” isn’t sufficient financial  justification. You need to peel back the layers to determine the quantifiable impact of improved decision making made possible by these sound bites.
	- The limitations and kung ano lang kaya gawin ng developers 
	- Justification
		- The cost
		- Benefits 
		- The time to develop 
	- Impact
		- The cost of life 
- Staffing
	- DW/BI projects require the integration of a cross-functional team with resources from both the business and IT communities. It is common for the same person to fill multiple roles on the team
	- Who are involved? 
	- Opportunities for newly Grads 
![[Untitled-2.png]]
- **Developing and Maintaining the Plan**
	- The key team members should develop estimates of the effort required for their tasks; the project manager can’t dictate the amount of time allowed and expect conformance. The project plan should identify acceptance checkpoints with business representatives after every major roadmap milestone and deliverable to ensure the project remains on track.  
	- Finally, DW/BI projects are vulnerable to scope creep largely due to a strong need to satisfy business users’ requirements. You have several options when confronted with changes: Increase the scope, play the zero-sum game, or say “no”. The most important thing about scope decisions is that they shouldn’t be made in an IT vacuum. The right answer depends on the situation.
	- The project manager does not makes the estimates
	- Are we actually accomplishing something? 
	- Scope creep - A small bump on the scope making it bigger to satisfy the business requirements
	- Zero-sum - What should I stop doing it? Gaining control on the scope agreement

#### Business requirements definition

**Collaborating with business users to understand their requirments and ensure their buy-in**
- Requirements planning 
	- **Choose the Forum**
		- Business user requirements sessions are typically interwoven with source system expert data discovery sessions. However, you don’t ask business representatives about the granularity or dimensionality of their critical data
		- Ask the right person on the requirements 
	- **Identify the Req. Team**
		- Regardless of the approach, you need to identify and prepare the involved project team members. Before sitting down with business users, you need to make sure to approach the sessions with the right mindset. Don’t presume you already know it all
		- Should be accompanied with the same language 
	- **Select, Schedule, Prep. Business representatives**
	- When it comes to preparing the interviewees, the business sponsor should communicate with them, stressing their commitment to the effort and the importance of everyone’s participation.
	- Prepare for the impact for the business
	- Make sure everyone is on the same page 
	- Don't waste your/someone's time 
- Collect Business Requirements
	- **Launch**
		- The designated kickoff person should script the primary talking points for the first few minutes when the tone of the interview  meeting is set.
		- Someone needs to talk about the primary talking point
		- Someone at the beginning to states the purpose
	- **Interview flow**
		- The objective of an interview is to get business users to talk about what they do and why they do it. Questions should depend on who you are talking to
		- The flow of the conversation
		- Flow vs time restraint
	- **Wrap up**
		- As the interview is coming to a conclusion, ask each interviewee about their success criteria for the project. Of course, each  criterion should be measurable.
		- The final minutes of the meeting 
		- Saying everything what has been agreed during the meeting 
		- Success criteria 
- Documenting Requirements
	- When writing up the findings document, you should begin with an executive summary, followed by a project overview covering the process used and participants involved. The bulk of the document centers on the business processes; foreach process, describe why business users want to analyze the process’ performance metrics, what capabilities they want, their current limitations, and potential benefits or impact
	- Describe why needs the users 
	- What features
	- List down everything 
- Prioritize requirements 
	- After the findings have been presented, it is time to prioritize using the prioritization grid. The grid’s vertical axis refers to the potential impact or value to the business. The horizontal axis conveys feasibility. Each of the finding’s business process themes is placed on the grid based on the representatives’ composite agreement regarding impact and feasibility
	- Least effort more impact first 

| Technical Architecture Design | Product Selection and Installation |
| -- | -- |
|The technical architecture is the blueprint of the DW/BI environment's technical services and infastrcuture | In many ways the architecture plan is similar to a shopping list for selecting product that fit into the plan's framework
|Establish Architecture Task Force | Understand Corporate Purchasing process |
| Collect architecture related requirements  | Develop Product Evaluation Matrix |
| Create architecture model |Conduct market research|
|Determine architecture implementation phases | Evaluate a shortlist of options  |
|Design and specify subsystems | If necessary, conduct a prototype
|Create the architecture plan | Select product, install trial, and negotiate | 
|Finalize and review technical architecture | 


**Dimensional Modellings:** More of this in the following lectures :p

**Physical Design**: The dimensional models developed and documented via a preliminary source-to-target mapping need  
to be translated into a physical database. In addition, hardware, software, and tools are evolving rapidly, so the following  
physical design activities and considerations merely scratch the surface.

1. Develop Naming and Database Standards 
2. Develop Physical Database model
3. Develop Initial Index Plan 
4. Design Aggregations, including OLAP Database 
5. Finalize Physical Storage Details 

**BI Application Specification** - before you start designing the initial applications, it’s helpful to establish standards, such as common pull-down menus and consistent output look and feel. Using these standards, you specify each application template and capture  
sufficient information about the layout, input variables, calculations, and breaks, so both the application developer and  
business representatives share a common understanding.

**BI Application Development**- When you move into the development phase for the BI applications, you again need to focus on standards; naming conventions, calculations, libraries, and coding standards should be established to minimize future rework. The  
application development activity can begin when the database design is complete, the BI tools and metadata are  
installed, and a subset of historical data has been loaded. The BI application template specifications should be  
revisited to account for the inevitable changes to the model since the specifications were completed.

#### Wrap-Up Activities

**Deployment** - It refers to the process of making the application work on a target device, whether it be a test server, production environment or a user's computer or mobile device. Software and application deployment are terms that can be used interchangeably. The technology, data, and BI application  tracks converge at deployment. Unfortunately, this convergence does not happen naturally but requires substantial preplanning

**Maintenance and Growth.** 
- Support - User support is immediately crucial following the deployment to ensure the business community gets hooked. 
- Education - You must provide a continuing education program for the DW/ BI system. 
- Technical Support - The DW/BI system needs to be treated as a production environment with service level agreements. 
- Program Support - The DW/BI program lives on beyond the implementation of a single phase.

#### Pitfalls to Avoid: 

1. Neglect to acknowledge that DW/BI success is tied directly to business acceptance. If the users haven't accepted the DW/BI system as a foundation for improved decision making, your efforts have been exercises in futility
2. Presume the business, its requirements and analytics, and the underlying data and the supporting technoogy are static
3. Load only summarized data into the presentation area's dimensional structures
4. Populate dimensional models on a standalone basis without regard to a data architecture that ties them together using shared, conformed dimensions 
5. Make the supposedly queryable data in the presentation area overly complex. Database designers who prefer a more complex presenation should spend a year supporting business users; they'd develop a much better appreciation for the need to seek simpler solutions. 
6. Pay more attention to back room operational performance and ease-of-devleopment than to front room query performance and ease of use 
7. Allocate energy to construct a normalized data structure, yet runout of budget before building a viable presentation area based  on dimensional models 
8. Tack a galactic multilayer project rather than pursuing more manageable, although still compelling, iterative development efforts
9. Fail to embrace or recruit an influential, accessible, and reasonable senior management visionary as the business sponsor of the DW/BI effort 
10. Become overlay enamored with technology and data rather than focusing on the business's requirements and goals 


**Dimensional Modelling addresses:**
- Understandable to business users
- Fasi query performance 
**What is so special about Dimensional Modelling?**
- modeling enables fast retrieval of information from large datasets by providing a structure that separates out unrelated or inconsequential data from the main body. The dimensional model also helps identify relationships between different types of data, allowing for deeper analysis of trends and patterns.

#### Fact tables 
- The fact table in a dimensional model stores the performance measurements resulting from an organization’s business process events. The data on each row is at a specific level of detail, referred to as the grain, such as one row per product sold on a sales transaction.  One of the core tenets of dimensional modeling is that all the measurement rows in a fact table must be at the same grain.
- All fact tables have two or more foreign keys that connect to the dimension tables’ primary keys. When all the keys in the fact table correctly match their respective primary keys in the corresponding dimension tables, the tables satisfy referential integrity. The fact table generally has its own primary key composed of a subset of the foreign keys (composite key). Every table that has a composite key is a fact table. Fact tables express many-to-many relationships.

#### Dimension Tables
- Dimension tables are integral companions to a fact table. The dimension tables contain the textual context associated with a business process measurement event. They describe the “who, what, where, when, how, and why” associated with the event. It is not uncommon for a dimension table to have 50 to 100 attributes. Dimension tables tend to have fewer rows than fact tables, but can be wide with many large text columns. Each dimension is defined by a single primary key, which serves as the basis for referential integrity with any given fact table to which it is joined.
- Dimension attributes serve as the primary source of query constraints, groupings, and report labels. In a query or report request, attributes are identified as the by words. For example, when a user wants to see dollar sales by brand, brand must be available as a dimension attribute. In many ways, the data warehouse is only as good as the dimension attributes; the analytic power of  the DW/BI environment is directly proportional to the quality and depth of the dimension attributes. The more time spent providing attributes with verbose business terminology, the better.


#### Star Schema 
- Each business process is represented by a dimensional model that consists of a fact table surrounded by a halo of dimension tables. This star-like structure is often called a star join.
- The first thing to notice about the dimensional schema is its simplicity and symmetry. Obviously, business users benefit from the simplicity because the data is easier to understand and navigate. Database optimizers process these simple schemas with fewer joins more efficiently. The predictable framework of a dimensional model withstands unexpected changes in user behavior.