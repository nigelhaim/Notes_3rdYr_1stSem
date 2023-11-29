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
- **Modelling**- Emphasized on the representation of data. Ensures that the data remains **consistent**, **resilient**, and **accessible**, even in complex environment 
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
- Assesses the organization's readiness for a DW/BI initiative, establishes the preliminary scope and justification, obtains resources and launches the program/project
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
- **Scoping and Justification** 
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
- **Staffing**
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

**Collaborating with business users to understand their requirements and ensure their buy-in**
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

## Retail Case Study
**What is a Lifecycle?**
- The SDLC aims to produce a **high-quality software that meets or exceeds customer expectations** reaches completion within times and cost estimates
- **What are the parts of a Kimball Lifecycle?**
	- Program/Project Planning, Business Requirments Definition. Technology Track. Data Track. BI Application Track. Deployment. Growth and Maintenance
- **What is Dimensional Modelling?**
	- Dimensional data modeling is an **analytical approach used in databases and data warehouses for organizing and categorizing facts into dimension tables**
- **What are the key concepts in Dimensional Modelling?**
	- Fact Table, Dimension Table, Star Schema 

### Four-Step Dimensional Design Process
1. **Select the Business Process**
	- A business process is a **low-level activity performed by an organization**, such as taking orders, invoicing, receiving payments, handling service calls, registering students, performing a medical procedure, or processing claims. 
2. **Declare the Grain**
	- Declaring the grain means **specifying exactly what an individual fact table row represents**. The grain conveys the level of detail associated with the fact table. It provides the answer to, "How do you describe a single row in the fact table"? 
3. **Identify the Dimensions**
	- Dimensions fall out of the question, "**How do business people describe the data resulting form the business process measurements events?**" You need to decorate fact tables with a robust set of dimensions representing all possible descriptions
4. **Identifying the Facts 
	- Declaring the grain means **specifying exactly what an individual fact table row represents**. The grain conveys the level of detail associated with the fact table. It provides the answer to "How do you describe a single row in the fact table?"

### Retail Case Study
1. **Select the Business Process**
	- In our retail case study, **management wants to better understand customer purchases as captured by the POS system**. Thus the business process you're modelling is **POS retail sales transactions.** This data enables the business users to analyze which products are selling in which stores on which days under what promotional conditions in which transactions. 
2. **Declare the grain**
	- In our case study the **most granular data is an individual product on a POS transaction**, assuming the POS system rolls up all sales for a given product within a shopping cart into a single line item. Although users probably are not interested in analyzing single items associated with a specific POS transactions, you can't predict all the ways they'll want to cull through that data.
3. **Identify the Dimensions**
	- The following **descriptive dimensions apply to the case: date, product, promotion, cashier, and all method of payment**. In addition, the POST transaction ticket number is included a s a special dimension, as described in the section "Degenerate Dimensions for Transaction Numbers" later.
4. **Identifying the Facts**
	- The facts collected by the POS system include the **sales quantity, per unit regular, discount, and net paid prices, and extended discount and sales dollar amounts.** The extended sales dollar amount equals to the sales quantity multiplied by the net unit price. Likewise, the extended discount dollar amount is the sales quantity multiplied by the unit discount amount. 

![[RetailSalesFact.png]]
##### What are the Derived Facts? 
- You can compute the gross profit by the subtracting the extended cost dollar amount from the extended sales dollar amount, or revenue. **Although computed, gross profit is also perfectly additive across all the dimensions:** you can calculate the gross profit of any combination of products sold in any set of stores on any set of days. Dimensional modelers sometimes question whether a calculated derived fact should be stored in the database. **We generally recommend it be stored physically.**
##### What are Non-Additive Facts? 
- **Percentages and ratios, such as gross margin, are non-additive**. The numerator and denominator should be stored in the fact table. The ratio can then be calculated in a BI tool for any slice of the fact table by remembering to calculate the ratio of the sums, not the sum of the ratios.

##### What are transaction Fact Tables? 
- **Transaction fact tables tend to be highly dimensional**. Even though transaction fact tables are unpredictably and sparsely populated, they can be truly enormous. Most billion and trillion row tables in a data warehouse are transaction fact tables. 

### Dimension table details 
Now that we've walked through the four-step process, let's return to the dimension tables and focus on populating them with robust attributes.
#### Date Dimension
![[Chart.png]]
![[Schema.png]]
**Dimensional models always need an explicit date dimension table**. There are many **date attributes not supported by the SQL date function**, including week numbers, fiscal periods, seasons, holidays, and weekends. rather than attempting to determine these nonstandard calendar calculations in a query, you should look them up in a date dimension table. 

##### Flags and Indicators as Textual Attributes
- Like many operational flags and indicators, the date dimension's holiday indicator is a simple indicator with two potential values. Because dimension table attributes serve as report labels and values in pull-down query filter lists
![[Date1.png]]
##### Current and Relative Date Attributes 
- Most date dimension attributes are not subject to update. June 1, 2013 will always roll up to June, Calendar Q2, and 2013. However, there are attributes you can add to the basic date dimension that will change over time, including IsCurrentDay, IsCurrentMonth, IsPrior60Days, and so on. IsCurrentDay obviously must be updated each day; the attribute is useful for generating reports that always run for today. A nuance to consider is the day that IsCurrentDay refers to. 

#### Product Dimension 
>[!Note]- Product Dimension
>![[ProductDimension.png]]

**Flatten Many-to-One Indices**
- Keeping the repeated low cardinality values in the primary dimension table is a fundamental dimensional modeling technique. Normalizing these values into separate tables defeats the primary goals of simplicity and performance

**Attributes with Embedded Meaning**
- Often operational product codes, identified in the dimension table by the NK notation for natural key, have embedded meaning with different parts of the code representing significant characteristics of the product

**Numeric Values as Attributes or Facts**
- If the numeric value is used primarily for calculation purposes, it likely belongs in the fact table. Because standard price is non-additive, you might multiply it by the quantity for an extended amount which would be additive.
>[!Note]- Numeric Values as Attributes or Facts
>![[ProductDimensionTable.png]]

**Drilling Down on Dimension Attributes**
- A reasonable product dimension table can have 50 or more descriptive attributes. Each attribute is a rich source for constraining and constructing row header labels. Drilling down is nothing more than asking for a row header from a dimension that provides more information
- Drilling down in a dimensional model is nothing more than adding row header attributes from the dimension tables. Drilling up is removing row headers. You can drill down or up on attributes from more than one explicit hierarchy and with attributes that are part of no hierarchy. 

>[!Note]- Dirlling Down on Dimension Attributes 
>![[reciept.png]]

#### Store Dimension 
**Multiple Hierarchies in Dimension Tables**
- The store dimension is the case study's primary geographic dimension. Each store can be thought of as a location. You can roll stores up to any geographic attribute, such as ZIP code , county, and state in the United States. Contrary to popular belief, cities and states withing the United States are not a hierarchy. Since many states have identically named cities, you'll want to include a City-State attribute in the store dimension. 
- Stores likely also roll up an internal organization hierarchy consisting of store districts and regions. These two different store hierarchies are both easily represented in the dimension because both the geographic and organizational hierarchies are well defined for a single store row. 
- The column describing selling square footage is numeric and theoretically additive across stores. You might be tempted to place it in the fact table. However it is clearly a constant attribute of a store and is used as a constraint or label more often that it used as an additive element in a summation. For these reasons, selling square footage belongs in the store dimension table. 

#### Dimension Table Details 
**Degenerate Dimensions**
- Operational transaction control number such as order numbers, invoice numbers, and bill-of-lading numbers usually give rise to empty dimensions and are represented as dimensions in transaction fact tables. The degenerate dimension is a dimension key without a corresponding dimension table. 

**Other Retail Dimensions**
- The decision whether a dimension should be associated with a fact table should be a binary yes/no on the fact table's declared grain. For example, there's probably a cashier identified for each transaction. The corresponding cashier dimension would likely contain a small subset of non-private employee attributes. Like the promotion dimension, the cashier dimension will likely have a No Cashier row for transactions that are processed through self-service registers. 
- A trickier situation unfolds for the payment method. Perhaps the store has rigid rules and only accepts one payment method per transaction. This would make your life as a dimensional modeler easier because you'd attach a simple payment method dimension to the sales schema that would likely include a payment method description, along with perhaps a grouping of payment methods into either cash equivalent or credit payment types. 


### Retail Schema in Action 
>[!Note]- Retail schema in action
>![[sidebside.png]]


### Retail Schema Extensibility 

Let's turn our attention to extending the initial dimensional design. Several years after the rollout of the retail sales schema, the retailer implements a frequent shopper program. 

Our original schema gracefully extends to accommodate this new dimension largely because the POS transaction data was initially modeled at its most granular level. The addition of dimensions applicable at that granularity did not alter the existing dimension keys or facts; all existing BI applications continue to run without any changes. 

The predictable symmetry of dimensional models enable them to absorb some rather significant changes in source data and/or modelling assumptions without invalidating existing BI applications, including: 

**New dimension attributes** - If you discover new textual descriptors of a dimension, you can add these attributes as a new columns/

**New dimensions** - as we just discussed, you can add a dimension to an existing fact table by adding a new foreign key column and populating it correctly with values of the primary key from the new dimension

**New measured facts** - If new measured facts become available, you can add them gracefully to the fact table. 

### Factless Fact Tables 

There is one important question that cannot be answered by the previous retail sales schema: What products were on  promotion but did not sell? The sales fact table records only the SKU actually sold. There are not fact table rows with zero facts or SKUs that didn't sell because doing so would enlarge the fact table enormously. This fact table enables you to see the relationship between the keys as defined by a promotion, independent of other events, such as actual product sales. We refer to it as a factless fact table because it has no measurement metrics.  
>[!Note]- Factless Fact tables
>![[Factless.png]]

### Dimension and Fact Table Keys 

Now that the schemas have been designed, we’ll focus on the dimension and fact tables’ primary keys, along with other row  
identifiers.


**Dimension Table Surrogate Keys**
- The unique primary key of a dimension table should be a surrogate key rather than relying on the operational system identifier, known as the natural key. Surrogate keys go by many other aliases: meaningless keys, integer keys, non-natural keys, artificial keys, and synthetic keys. Surrogate keys are simply integers that are assigned sequentially as needed to populate a dimension
**Dimension natural and Durable**
- If the dimension’s natural keys are not absolutely protected and preserved over time, the ETL system needs to assign permanent durable identifiers, also known as supernatural keys. A persistent durable supernatural key is controlled by the DW/ BI system and remains immutable for the life of the system.

**Fact Table Surrogate keys**
- Although we’re adamant about using surrogate keys for dimension tables, we’re less demanding about a surrogate key for fact tables. Fact table surrogate keys typically only make sense for back room ETL processing.


### Resisting Normalization Urges 
**Snowflake Schema with Normalized Dimensions**
- Dimension table normalization is referred to as snowflaking. Redundant attributes are removed from the flat, denormalized  dimension table and placed in separate normalized dimension tables

>[!Note]- Snowflake Schema with Normalized Dimensions
>![[Resist.png]]

**Outriggers**

Although we generally do not recommend snowflaking, there are situations in which it is permissible to build an outrigger  
dimension that attaches to a dimension within the fact table’s immediate halo. The outrigger date attributes are descriptively and uniquely labeled to distinguish them from the other dates associated with the business process. It only makes sense to outrigger a primary dimension table’s date attribute if the business wants to filter and group this date by nonstandard calendar attributes, such as the fiscal period, business day indicator, or holiday period. 

>[!Note]- Outriggers
>![[Outriggers.png]]

**Centipede Fact Tables with Too Many Dimensions**

## Physical Design 
- This module discusses key concepts on how to effectively translate the expected schemas (logical design) into actual database structures (physical design)/
#### Four-step Dimensional process
### Logical design -> Physical design 
- Pen and paper -> SQL statements

### What is Physical design in DWH? 
- During the physical design process, a developer converts the data gathered during the logical design phase into a description of the physical database structure. 
**Indexes**
- Speed up queries 
#### Logical Design
**Entities**- linked together using relationships
**Attributes**- used to describe the entities
**Unique identifiers**- distinguis between instances 

#### Physical Design 
- **Entities** -> **Tables**
- **Relationships** -> **Foreign keys**
- **Attributes** -> columns
- **Unique identifiers** -> **Unique Constraints**


> [!Note]- Once you have converted your logical design to a physcial one, you must create some or all of the following structures
> ![[Pasted image 20231005085440.png]]


#### Tablespaces 
- consists of one or more datafiles, which are physical structures withing the operating system you are using
- **Design perspective** - containers for physcial design structures 
- need to be separated by differences. Tables should be separated from indexes, small should be separated from large. 
- represent logical business units if possible 

#### Tables or Partitioned Tables
- **Tables**
	- basic unit of data storage
	- container for the expected amount of raw data 
- **Partitioned tables**
	- nonpartitioned ones addresses the key problem of support ting very large data volumes 
	- allowing to divide them into smaller and more manageable pieces 
- Data is stored in physical blocks, holds one partition of data, Each partitioned table maintains various metadata about the sort properties across all operations that modify it. 

>[!Note]- Tables and Partitioned Tables
>![[Pasted image 20231005085930.png]]

#### Indexes and Partitioned Indexes 
- **Indexing**
	- Improves database performance by minimizing the number of disc visits required to fulfill a query. 
	- Data structure technique used to locate and quickly access data in databases. 
- The Main key / Candidate key is duplicated in the first column, which is the Search key. The second column is the Data Reference or Pointer which contains a set of pointers holding the address of the disk block where that particular key value can be found. 
> [!Note]- Structure of an index
> ![[Pasted image 20231005090228.png]]


#### Indexes and Partitioned Indexes
**Bitmap indexes**
- Very common in data warehousing environments. 
- improve the performance of read-only queries that involve large datasets
- data structure that represents the presence or absence of data values in a table or column.

>[!Note]- Bitmap Index
>![[Pasted image 20231005090904.png]]
>![[Pasted image 20231005090923.png]]


##### Features of a Bitmap index
- **Space efficiency** - Bitmap indexes are highly space-efficient because they use a compact binary representation to store the occurrence of each value or combination of values in each attribute.
- **Fast query processing** - bitmap indexes can be used to quickly answer complex queries involving multiple attributes using set-based operations such as AND, OR, and NOT.
- **Low maintenance overhead** - Bitmap indexes require relatively low maintenance overhead because they can be updated incrementally as data changes. 
- **Reduced I/O overhead** - Bitmap indexes can be used to avoid expensive I/O operations by using a compressed representation of the data.

#### Index and Partitioned Indexes
**Partitioned index** - decomposed into smaller and more manageable pieces 
**Global Indexes** - partitioned independently of the table on which they are created 
**Local Indexes** - automatically linked to the partitioning method for a table

>[!Note]- Indexes and Partitioned Indexes\
>![[Pasted image 20231005091731.png]]

## Views
- Tailed representation of the data contained in one or more tables or other views. 
- takes the output of a query and treats it as a table. 
- do not require any space in the database
- Provide an additional level of table security by restricting access to a predetermined set of rows or columns of a table 
- Hide data complexity 
- Present the data in  a different perspective from that of the base table 
- Isolate applications from changes in definitions of base tables
#### Base tables 
- view derives its data from the  tables
- All operations performed on a view actually affect the base tables

>[!Note]- Views
>![[Pasted image 20231005092747.png]]

### Materialized views
- query results that have been stored in advance so long-running calculations are not necessary
- resemble tables or partitioned tables and behave like indexes in that they are used transparently and improve performance

>[!Note]- Materialized view
>![[Pasted image 20231005095042.png]]

## Hardware and I/O Considerations in Data Warehouses 

#### Why Hardware and I/O are important? 
- I/O performance should always be a key consideration for DWH designers and administrators; it should be designed to meet heavy I/O-intensive requirements

**I/O performance should always be a key consideration for data warehouse designers and administrators. The typical workload in a data warehouse is especially I/O intensive**
#### Integrity Constraints 
- enforce business rules associated with your database 
- prevent having invalid information in the tables. 
- constraints are only used for query rewrite

#### Guidelines

**Configure I/O for Bandwidth not Capacity** - Storage configurations for a data warehouse should be choses based on the I/O bandwidth that they can provide, and not necessarily on their overall storage capacity.

**Stripe Far and Wide** - The guiding principle in configuring an I/O system for a data warehouse is to maximize I/O bandwidth by having multiple disks and channels access each database object.

**Use Redundancy** - Because data warehouses are often the largest database systems in a company, they have the most disks and thus are also the most susceptible to the failure of a single disk. Therefore, disk redundancy is a requirement for data warehouses to protect against a hardware failure. 

**Test the I/O System before building the database** - The most important time to examine and tune the I/O system is before the database is even created. Once the database files are created, it is more difficult to reconfigure the files.

**Plan for Growth** - A data warehouse designer should plan for future growth of a data warehouse. There are many approaches to handling the growth in a system, and the key consideration is to be able to grow the I/O system without compromising the I/O bandwidth. 

#### How is DWH partitioning helpful? 
- Partitioning offers support for very large tables and indexes by letting you decompose them into smaller and more manageable pieces called partitions. 

#### Parallel execution 
- Capability that addresses the challenge of finding and presenting the right information in a timely fashion in the vast quantity of data stored in any databases 

#### Why integrity constraints are helpful in DWH? 
- provides a mechanism for ensuring that data conforms to guidelines specified by the database administrator. Constraints can be used for data cleanliness and query optimization. 


# Inventory Case Study

Most organizations have an underlying value chain of key business processes. The value chain identifies the natural, logical flow of an organization’s primary activities. For example, a retailer issues purchase orders to product manufacturers. The products are delivered to the retailer’s warehouse, where they are held in inventory. A delivery is then made to an individual store, where again the products sit in inventory until a consumer makes a purchase.

Operational source systems typically produce transactions or snapshots at each step of the value chain. The primary objective of most analytic DW/BI systems is to monitor the performance results of these key processes. Because each process produces unique metrics at unique time intervals with unique granularity and dimensionality, each process typically spawns one or more fact tables. To this end, the value chain provides high-level insight into the overall data architecture for an enterprise DW/BI environment

>[!Note]- Waterfall
>![[Pasted image 20231005103027.png]]

### Inventory Models
#### Model #1: Inventory Periodic Snapshot 
Making sure the right product is in the right store at the right time minimizes out-of-stocks (where the product isn’t available on the shelf to be sold) and reduces overall inventory carrying costs. The retailer wants to analyze daily quantity-on-hand inventory levels by product and store.

| Business Process | Grain | Dimensions | Fact | 
|---|---|---|---|
|Inventory Management | Date, Product, Store | Daily Inventory of products | Quanitity at Hand | 

>[!Note]- Inventory Periodic Snapshot
>![[Pasted image 20231005103239.png]]
>Is Quanitity Addititive? 


**Semi-Additive Facts**: In the inventory snapshot schema, the quantity on hand can be summarized across products or   stores and result in a valid total. Inventory levels, however, are not additive across dates because they represent snapshots of a level or balance at one point in time. Because inventory levels (and all forms of financial account balances) are additive across some dimensions but not all, we refer to them as semi-additive facts.  

**Enhanced Inventory Period Snapshot**: The simplistic view in the periodic inventory snapshot fact table enables you to see a time series of inventory levels. For most inventory analysis, quantity on hand isn’t enough. Quantity on hand needs to be used in conjunction with additional facts to measure the velocity of inventory movement and develop other interesting metrics such as the number of turns and number of days’ supply. Notice that quantity on hand is semi-additive, but the other measures in the enhanced periodic snapshot are all fully additive. The quantity sold amount has been rolled up to the snapshot’s daily granularity.

#### Model #2: Inventory Transactions 

Even though the transaction fact table is simple, it contains detailed information that mirrors individual inventory manipulations. The transaction fact table is useful for measuring the frequency and timing of specific transaction types to answer questions that couldn’t be answered by the less granular periodic snapshot.  

Even so, it is impractical to use the transaction fact table as the sole basis for analyzing inventory performance. Although it is theoretically possible to reconstruct the exact inventory position at any moment in time by rolling all possible transactions forward from a known inventory position, it is too cumbersome and impractical for broad analytic questions that span dates, products, warehouses, or vendors.

>[!Note]- Model#2
>![[Pasted image 20231005104958.png]]

>[!Note]- Model#3
>![[Pasted image 20231005105041.png]]

### Types of fact Tables 
| | Transaction | Periodic Snapshot | Accumulating Snapshot |
|--|--|--|--|
|Periodicity| Discrete transaction point in time | Recurring snapshots at regular, predictable intervals | Interdeterminate time span for evolving pipeline/workflow |
|Grain | 1 row per transaction or transaction line | 1 row per snapshot period plus other dimensions | 1 row per pipeline occurence | 
|Data dimension | Transaction date | Snapshot date | Multiple dates for pipeline's key milestones |
| Facts | Transaction performance | Cumulative performance for time interval | Performance for pipeline occurrence | 
| Fact table sparsity | Sparse or dense, depending on activity | Predictably dense | Sparse or dense, depending on pipeline occurrence | 
|Fact table updates | No updates, unless error correction | No updates, error correction | Updated whenever pipeline activity occurs |

Periodic snapshots are needed to see the cumulative performance of the business at regular, predictable time intervals. Unlike the transaction fact table where a row is loaded for each event occurrence, with the periodic snapshot, you take a picture (hence the snapshot terminology) of the activity at the end of a day, week, or month, then another picture at the end of the next period, and so on. The periodic snapshots are stacked consecutively into the fact table. The periodic snapshot fact table often is the only place to easily retrieve a regular, predictable view of longitudinal performance trends.


Although perhaps not as common as the other two fact table types, accumulating snapshots can be very insightful. Accumulating snapshots represent processes that have a definite beginning and definite end together with a standard set of intermediate process steps. Accumulating snapshots are most appropriate when business users want to perform workflow or pipeline analysis.

#### Lags Between milestones and milestone counts
Because accumulating snapshots often represent the efficiency and elapsed time of a workflow or pipeline, the fact table typically contains metrics representing the durations or lags between key milestones. Sometimes the lag metrics are simply the raw difference between the milestone dates or date/time stamps

### Value Chain Integration
Both business and IT organizations are typically interested in value chain integration. Business management needs to look across the business’s processes to better evaluate performance. Obviously, this requires the ability to consistently look at customer information across processes, such as quotes, orders, invoicing, payments, and customer service. Similarly, organizations want to analyze their products across processes, or their employees, students, vendors, and so on.

>[!Note]- Value Chain Integration 
>![[Pasted image 20231005105728.png]]


## Enterprise Data Warehouse bus architecture 

A bus is a common structure to which everything connects and from which everything derives power. The bus in a computer is a standard interface specification that enables you to plug in a disk drive, DVD, or any number of other specialized cards or devices.  

The enterprise data warehouse bus architecture provides a rational approach to decomposing the enterprise DW/BI planning task. The master suite of standardized dimensions and facts has a uniform interpretation across the enterprise.  

The bus architecture enables DW/BI managers to get the best of both worlds. They have an architectural framework guiding the overall design, but the problem has been divided into bite-sized business process chunks that can be implemented in realistic time frames.  

The bus architecture is independent of technology and database platforms. All flavors of relational and OLAP-based dimensional models can be full participants in the enterprise data warehouse bus if they are designed around conformed dimensions and facts.

>[!Note]- bus architecture 
>![[Pasted image 20231005105937.png]]

#### Enterprise Data Warehouse Bus Matrix 
Working in a tabular fashion, the organization’s business processes are represented as matrix rows. It is important to remember you are identifying business processes, not the organization’s business departments. The matrix rows translate into dimensional models representing the organization’s primary activities and events, which are often recognizable by their operational source.  

The columns of the bus matrix represent the common dimensions used across the enterprise. It is often helpful to create a list of core dimensions before filling in the matrix to assess whether a given dimension should be associated with a business process.

>[!Note]- Bus Matrix Enterprise
>![[Pasted image 20231005110054.png]]

The matrix’s columns address the demands of master  
data management and data integration head-on.  

Each business process-centric implementation project incrementally builds out the overall architecture. Multiple development teams can work on components of the matrix independently and asynchronously, with confidence they’ll fit together.  

The matrix enables you to communicate effectively within and across data governance and DW/BI teams. Even more important, you can use the matrix to communicate upward and outward throughout the organization.



#### Common bus matrix Mistakes 

**Departmental or overly encompassing rows** - The matrix rows shouldn’t correspond to the boxes on a corporate organization chart representing functional groups. Some departments may be responsible or acutely interested in a single business process, but the matrix rows shouldn’t look like a list of the CEO’s direct reports.

**Report-centric or too narrowly defined rows** - At the opposite extreme, the bus matrix shouldn’t resemble a laundry list of requested reports. A single business process supports numerous analyses; the matrix row should reference the business process, not the derivative reports or analytics.

**Overly generalized columns** - A “person” column on the bus matrix may refer to a wide variety of people, from internal employees to external suppliers and customer contacts. Because there’s virtually zero overlap between these populations, it adds confusion to lump them into a single, generic dimension.

**Separate columns for each level of a hierarchy** - The columns of the bus matrix should refer to dimensions at their most granular level. Some business process rows may require an aggregated version of the detailed dimension, such as inventory snapshot metrics at the weekly level.


#### Conformed dimensions
- should be built once in the ETL system and then replicated either logically or physically throughout the enterprise DW/BI environment.
>[!Note]- Benefits: Drilling Across Fact Tables
>![[Pasted image 20231005110819.png]]

#### Types 

**Identical Conformed Dimensions**
- At the most basic level, conformed dimensions mean the same thing with every possible fact table to which they are joined. The date dimension table connected to the sales facts is identical to the date dimension table connected to the inventory facts. Identical conformed dimensions have consistent dimension keys, attribute column names, attribute definitions, and attribute values (which translate into consistent report labels and groupings). Dimension attributes don’t conform if they’re called Month in one dimension and Month Name in another; likewise, they don’t conform if the attribute value is “July” in one dimension and “JULY” in another. Identical conformed dimensions in two dimensional models may be the same physical table within the database.  
- Most conformed dimensions are defined naturally at the most granular level possible. The product dimension’s grain will be the individual product; the date dimension’s grain will be the individual day.

**Shrunken Rollup Conformed Dimension with Attribute Subset**
- Dimensions also conform when they contain a subset of attributes from a more granular dimension. Shrunken rollup dimensions are required when a fact table captures performance metrics at a higher level of granularity than the atomic base dimension. This would be the case if you had a weekly inventory snapshot in addition to the daily snapshot.

>[!Note]- Shrunken Rollup Conformed Dimension with Attribute Subset
>![[Pasted image 20231005111120.png]]

**Shrunken Conformed Dimension with Row Subset**
- Another case of conformed dimension subsetting occurs when two dimensions are at the same level of detail, but one represents only a subset of rows. For example, a corporate product dimension contains rows for the full portfolio of products across multiple disparate lines of business
>[!Note]- Shrunken Conformed Dimension with Row Subset
>![[Pasted image 20231005111232.png]]

**Shrunken Conformed Dimensions on the Bus Matrix**
 - The bus matrix identifies the reuse of common dimensions across business processes. Typically, the shaded cells of the matrix indicate that the atomic dimension is associated with a given process. When shrunken rollup or subset dimensions are involved, you want to reinforce their conformance with the atomic dimensions.
>[!Note]- Shrunken Conformed dimensions on the bus matrix
>![[Pasted image 20231005111333.png]]


#### Issues 
**Conformed Dimensions in Agile Movement** - Conformed dimensions allow a dimension table to be built and maintained once rather than re-creating slightly different  
versions during each development cycle. Reusing conformed dimensions across projects is where you get the  
leverage for more agile DW/BI development.
**Conformed Dimensions in Agile Movement** 
- Conformed dimensions allow a dimension table to be built and maintained once rather than re-creating slightly different versions during each development cycle. 
- Reusing conformed dimensions across projects is where you get the leverage for more agile DW/BI development. If you fail to focus on conformed dimensions because you’re under pressure to deliver something yesterday the departmental analytic data silos will likely have inconsistent categorizations and labels.


Revenue, profit, standard prices and costs, measures of quality and customer satisfaction, and other key  
performance indicators (KPIs) are facts that must also conform. If facts live in more than one dimensional model, the underlying definitions and equations for these facts must be the same if they are to be called the same thing.


If they are labeled identically, they need to be defined in the same dimensional context and with the same units of measure from dimensional model to dimensional model. For example, if several business processes report revenue, then these separate revenue metrics can be added and compared only if they have the same financial definitions.


---
# Finals 

## Data pipelines 
- Sources -> **Processing** -> Data Mart 

### What are Data Pipelines? 
- A data pipeline is a means of moving data from one place to a destination. Along the way, data is transformed and optimized so that it can be analyzed for business insights. 

**Characteristics of a data pipeline**

- THis is incluseive of data transformations, such as filtering, masking, and aggregations 
- Organizing the data 
- The bytes of every data type 
- Includes data transformations
- **Filtering**
	- Sometimes there is data that will be left out 
- **Masking**
	- Snapshots 

## Characteristics of a Data Pipeline

- **Data Transformations:**
  - Inclusive of data transformations, such as filtering, masking, and aggregations.
  - Ensure appropriate data integration and standardization.

- **Data Processing:**
  - The type of data processing that a data pipeline requires is usually determined through a mix of exploratory data analysis and defined business requirements.

- **Foundation for Data Projects:**
  - Well-organized data pipelines provide the foundation for a range of data projects.
  - This can include exploratory data analyses, data visualizations, and machine learning tasks.

### Types of data pipelines 
#### Batch pipelines 
- Set time interval 
	- OMTP
	- OLAP
- Batch processing 
	- Only need to call once 
>[!Note]- Batch Pipelines
>![[Pasted image 20231120144609.png]]

- **Definition:**
  - As the name implies, batch processing loads "batches" of data into a repository during set time intervals, typically scheduled during off-peak business hours.

- **Optimal Use Case:**
  - Batch processing is usually the optimal data pipeline when there isn't an immediate need to analyze a specific dataset.

- **Workflow:**
  - It forms a workflow of sequenced commands, where the output of one command becomes the input of the next command.
  - This series of commands will continue until the data is completely transformed and loaded into the data repository.


- **Examples**
	- Inventory 
#### Streaming Data
- Continous calling 
- **Examples**
	- Real-time transactions 

>[!Note]- Streaming Data
>![[Pasted image 20231120144739.png]]

- **Definition:**
  - Unlike batching processing, streaming data is leveraged when it is required for data to be continuously updated. For example, apps or point of sale systems need real-time data to update inventory and sales history of their products.

- **Event and Topic:**
  - A single action, like a product sale, is considered an "event," and related events, such as adding an item to checkout, are typically grouped together as a "topic" or "stream."

- **Latency and Reliability:**
  - Since data events are processed shortly after occurring, streaming processing systems have lower latency than batch systems.
  - However, they aren't considered as reliable as batch processing systems.


### Core steps in Data pipeline 
#### Data ingestion 
- Import of data 
- Load of files 
>[!Note]- Data Ingestion 
>![[Pasted image 20231120144935.png]]
- **Definition:**
  - Unlike batching processing, streaming data is leveraged when it is required for data to be continuously updated. For example, apps or point of sale systems need real-time data to update inventory and sales history of their products.

- **Best Practice:**
  - While businesses can choose to extract data only when they are ready to process it, it's a better practice to land the raw data within a cloud data warehouse provider first.

#### Data Transformation 
- Making everything standard 
- Use Case Diagram 
- Step by step process on how to trransform the data 
#### Data Storage 
- The transformed data is then stored within a data repository, where it can be exposed to various stakeholders. Within streaming data, this transformed data are typically known as consumers, subscribers, or recipients.
>[!Note]- Data Storage
>![[Pasted image 20231120151717.png]]

### Use Cases of Data pipeline 

#### Exploratory Data Analysis

Exploratory Data Analysis is used by data scientists to analyze and investigate data sets and summarize their main characteristics, often employing data visualization methods. It helps determine how best to manipulate data sources to get the answers you need.

#### Data Visualization

Data Visualization represents data via common graphics, such as charts, plots, infographics, and even animations. These visual displays of information communicate complex data relationships and data-driven insights in a way that is easy to understand.

#### Machine Learning

Machine Learning is a branch of artificial intelligence (AI) and computer science which focuses on the use of data and algorithms to imitate the way that humans learn, gradually improving its accuracy.

### ETL

#### What is ETL 
- In computing Extract, Transform, Load is a three-phase proces where data is extracted, transformed and loaded into an output data container 

You may find that some terms, such as data pipeline and ETL pipeline, are used interchangeably in conversation.  
However, you should think about an ETL pipeline as a subcategory of data pipelines


#### Data Pipelines vs. ETL 

- ETL pipelines follow a specific sequence. As the abbreviation implies, they extract, transform, and then load  
the data. All data pipelines do not need to follow this sequence. In fact, ELT pipelines have become more  
popular with the advent of cloud-native tools.  

- ETL pipelines also tend to imply the use of batch processing, but the scope of data pipelines is broader.  
They can also be inclusive of stream processing.  

- Data pipelines as a whole do not necessarily need to undergo data transformations, like ETL pipelines.  
It’s just rare to see a data pipeline that doesn’t utilize transformations to facilitate data analysis.
#### How to create an ETL system 
1. Gather and identify the necessary requirements
2. Identify how to build components for extracting data
3. Identify how to build components for transforming data
4. Identify how to build components for loading and delivering the data
5. Identify how to build components for managing the ETL environment in production

#### Requirements you need to focus on 
- **Business Needs:**
  - Maintain a list of key performance indicators (KPIs) uncovered during the business requirements definition.
  - Include drill-down and drill-across targets for investigating changes in KPIs.

- **Compliance:**
  - Consult with legal and compliance officers to list data and final reports subject to compliance restrictions.
  - Specify data requiring proof of security for copies under your control.

- **Data Quality:**
  - List data elements with known unacceptable quality.
  - Note agreements with source systems for correcting data before extraction.
  - Include data elements discovered during profiling, to be continuously monitored and flagged in the ETL process.
- **Security:**
  - Expand the compliance checklist to cover known security and privacy requirements.

- **Data Integration:**
  - Use the bus matrix of business processes to generate a priority list for conforming dimensions.
  - Annotate each row of the bus matrix with the executive demand for business processes to participate in the integration process.
  - Confirm agreement from the ETL team responsible for each business process.

- **Data Latency:**
  - List all legitimate business demands for data based on timing requirements (daily, many times per day, within seconds, instantaneously, etc.).

- **Archiving and Lineage:**
  - List data sources and intermediate data steps to be archived.
  - Specify retention policies, compliance, security, and privacy constraints.

- **BI Delivery Interfaces:**
  - List all fact and dimension tables directly exposed to BI tools, derived from the dimensional model specification.
  - Enumerate OLAP cubes and special database structures required by BI tools.
  - Specify known indexes and aggregations agreed upon to support BI performance.

- **Available Skills:**
  - Inventory department skills, including operating system, ETL tool, scripting language, programming language, SQL, DBMS, and OLAP.
  - Identify skills required for current and future systems.

- **Legacy Licenses:**
  - List legacy operating system, ETL tool, scripting language, programming language, SQL, DBMS, and OLAP licenses.
  - Specify whether exclusive use is mandated or recommended.
### Some Subsystems for Extracting Data

#### Subsystem #1: Data Profiling
Data profiling involves the technical analysis of data to describe its content, consistency, and structure. It is akin to performing a SELECT DISTINCT investigative query on a database field.

- **Purpose:**
  - Assess the suitability of a candidate data source for inclusion in the data warehouse.
  - Provide early go/no-go decisions.
  - Offer guidance on the extent

11-20-2023

## Data Visualization and Analytics (Guest Lecture)

### Introduction to Analytics 
#### About the guest
##### My journey in Data
- **Truths**
	- 4 years of working
	- non-technical background and started tech career in a business strategy team 

- **Lie**
	- passionate about coding (self-learned and passed coding)
- **More about me:**
	- Currently Handle MayaBank's growth data science team
	- Used to work in non-profit project design and program delivery before pivoting into tech role at Grab 
	- Customer-obsessed, problem-obsessed, and I am a very curious person. 
		- Asking the right questions > The mathematical aspect

#### What is Data Science? 
- **Science**
	- Focused on empirical evidence 
	- Reproducibility 
		- A way to reproduce the results 
	- Extensive use of mathematical concepts to properly tune different models and to optimize results 
	- Methodologies are based on mathemat6ical theories and frameworks. 
		- Many ways to produce a preidction modelts and in the end all are based on the mathematical concepts 
- **Art**
	- Relies on a exploratory workflow and a clear hypothesis 
		- Art -> Science = Data science 
	- Does not follow a strict procedure 
		- No one really tells you what is the perfect model
		- It all depends on the person that handles the data 
	- Model performance is greatly dependent on the features is greatly dependent on the features 
		- How do they represent this concept in the real world? 
	- Many data science deicsions are left to hte person who holds the project 

#### What is analytics?

##### "I have no plans of working in any data role. How is analytics thinking useful for me?"

##### As a software engineer: 
- Analytical thinking can give you more structure on ho you debug your code. 
- It can also help you to cost/size certain opportunities to help communicate your agenda to senior management.

##### As a product manager: 
- Defining opportunities on how you grow your product. 
- Uncover insights to develop new products. 

##### 6 Types of analytics questions 
**Descriptive**
- Summarize a characteristic of a set of data
	- Describing the situation 
- Examples include: 
	- determining the propportion of males
	- mean number of servings of fresh fruits and vegetables per day,
	- freque4ncy of viral illnesses in a set of data collected from a group of individuals 
	- there is no interpretation of the result itself as the result is a fact
- **Exploratory**
	- Analyze the data to see if there are patterns, trends, or relationships between variables 
		- You don't know what you'll get but it gives you a better understanding
	- These types of analyses are also called "hypothesis-generating" analysis because rather that testing a hypothesis, you are looking for patterns that would support proposing a hypothesis
	- Eg. Exploring the relationship of diet and viral illness
- **Inferential**
	- Coming form your exploratory analysis, you test your hypothesis to see if it is true
	- For example, there could be a relationship between viral illness and diet, but is this true for the whole of the Philippine? Or only within a certain region? 
	- The type of people/data given 
- **Predictive**
	- Analyze the data to see if there are patterns, trends, or relationships between variables 
	- For example, this type of study does not care about what type of people will eat fruits and vegetables. It cares moer about knowing if a person will eat fruits and vegetables next week.
- **Causal**
	- A causal question asks about whether changing one factor will change another factor, will change another factor, on average, in a population. Sometimes the underlying design of the data collection, by default, allows for the question that you ask to be casual. 
	- E.g We know that people who eat vegetables have fewer viral illnesses, but does eating vegetables lead to a reduciton of viral cases? 
- **Mechanistic**
	- Focuses on the how
	- How does eating fruits and vegetables lead to fewer viral illnesses? 

### Analytics planning 

#### What is an analytics plan? 
Analytics can get very messy if you're not focused on where to look. This is where a plan comes in handy!
- Narrows down the scope of the problem to what is essential 
- Helps you decide on what you actually want to know to come up with an answer of a project. 

#### What is an analytics plan?
Analytics can get very messy if you're not focused on where to look. This is where a plan comes in handy!
- Narrows down the scope of the problem to what is essential 
- Helps you decide on what you actually want to know to come up with an answer or a project. 


#### What needs to be clarified even before we start analytics planning? 
- The context and problem 
- The main objectives and key questions 
- The scope and limitations 

#### Why do we need to do analytics planning? 
- Ensure that valuable analysis is done 
	- Make sure to look at the things that actually matter 
- Correct metrics are being looked at 
- Insights are actionable 
	- What good is it for you to give suggestions? 
- Time is used efficiently 
	- Pace yourself to uncover things simply
- Sufficient view of the issue is employed 
	- Narrow it down, but if its too narrow then it could be insufficient
- Accurate numbers are presented 
- Correct conclusions are made

#### Essential parts of an analytics framework: 
#### Identify the problem: 
- What is the problem? Is it worth solving? 
#### Define the constraints:
- What is the realm of possibility? What are the things we can control? 
#### Structure analysis: 
- What metrics are involved? What key questions do we need to answer? 
#### Design methodology: 
- What calculations or algorithms are appropriate to answer key questions?
#### Creating insights and conclusions 
- A way to communicate whatever you found in the analytics plan

## Exercise 
- Imagine that you work as an elf in the analytics division of Santa Claus' toy factory
Santa Claus' factory's distribution channels work like a ride-hailing app 
- All the demand is on Christmas eve midnight. 
- There are many children that have toys under their name 
- But a limited number of reindeer to meet the demand 
- Available reindeers recieve unfulfilled jobs if they are within a good child's radius

This is why only the top X% good children receive toys. 

This year, many reindeers are sick with COVID-19. That means many children might not be matched to any reindeers to deliver their gifts. I have some budget for reindeer rewards, but im not sure if that will move the needle. What is the best way to deliver gifts this Christmas season? 


An analytics problem is: 
- Measurable - so we know the north star metric. 
- Related to a key objective that we want to achieve

| Not problems | Problems | 
|-|-|
|Reduce reindeer service area | Reindeers are waisting too much time delievering gifts in very far-flung areas|
|increase the number of reindeers matched to children | The number of reindeers are being matched to children is 20% below Santa's target | 
|Implement productivity rewareds for reindeers who deliever more gifts | spend on reindeer rewards is too high| 


Sizing the problem 
Is the problem worth solving? 
Sometimes,  there are some problems where the most efficient course of action is to do nothing. 

Defining the constraints:
- What are the limitations and assumptions in your analysis? 
- Constraints restrictions our solutions and analysis plan to only the components that are possible relevant. Thies also serve as guardrils when creating solutions

Examples 

![[Pasted image 20231120123531.png]]



Structuring the anaylsis 
- What do we want to know? 
	- Describe: 
		- What are out levers to better match reindeer and children? 
		- Reindeer rewards for productivity? 
		- Children on the nice list 
		- Distance of top children on the nice list
	- Evaluate: 
		- How much impact each lever can give us to solve the problem

- This is where we define/outline what we want to describe/evaluate/validate 
- What are the key questions that we should answer? 

Creating insights and conclusions:
- Never trust your data!
	- Always sense check if the averages, min, max values make sense. It can also tell you if these values might need special handling 
- Ensure you have enough data points to make your conclusions 
- Beware of confirmation bias. Make counter-validation part of your analysis.


# Lab exer 3

## Install pyenv 
- Use pip 

### pyenv install 3.8.4

We do this because apache-airflow is not compatible with the latest version of python
