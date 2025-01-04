# What is software-architecture?
Software architecture is sum of all the important decisions within a product. Important decisions are all decisions that are difficult to change in the course of further development.

Software architecture defines the structure of a software product. This includes elements, the externally visible properties of the elements, and the relationships between the elements.

These two basic materials can be used to describe a wide variety of architecture views. The static (module) view contains the following elements: classes, packages, namespaces, directories, and projects—in other words, all the containers you can use for programming code in that particular programming language. In the distribution view, the following elements can be found: archives (JARs, WARs, assemblies), computers, processes, communication protocols and channels, and so on. In the dynamic (runtime) view we are interested in the runtime objects and their interactions.

### What are guardrails in Architecture?
Create an architecture that restricts the design space during the development of the software system and gives you direction in your work. Guardrails allow developers and architects to orient themselves. The decisions are channeled uniformly and can be understood and traced, giving the software system a homogeneous structure. When solving maintenance tasks, guardrails guide all participants in a uniform direction, and lead to faster and more consistent results during the adaptation or extension of the system.

Investment in software should pay for itself for as long as possible. New software should incur the lowest possible maintenance and expansion costs in the course of its lifetime—in other words, the technical debt must be kept as low as possible. 

##### Target Architecture
The architecture planned by the development team is called 'target architecture'

##### Actual Architecture
the architecture represented by the source code is called 'actual architecture'

#### Reasons behind deviations from Target Architectures
* The development team misunderstands or is ignorant of the target architecture. The implementation therefore violates the specifications of the target architecture. 
* Business and technical details were overlooked while planning the target architecture and it wasn’t adapted accordingly. In such a case, the target architecture may be superfluous or should be developed further.
* Competing quality goals, such as performance and loose coupling, only become apparent during later development. Furthermore, they are often implemented differently in different areas of the source code.
The difference between actual and target architecture creates complexity for the development team.

![image](https://github.com/user-attachments/assets/6978d3f4-755d-4bbd-a3b2-2ae40fd43e0a)

The goal of durable architecture is to reduce development and maintenance costs. Software should be easily modifiable. The software development team should be able to quickly navigate the source code and its structures during their work. This is particularly important because developers and architects spend most of their time reading and understanding code.

#### How to make your code more flexible?
* Encapsulation and loose coupling
* Dependency on abstractions
* Programming against abstractions 

### What is Technical Debt?
Technical debt refers to the <b>implied cost of future rework or inefficiencies caused by choosing an easier, quicker, or suboptimal solution in software development instead of a more robust, long-term approach</b>. While these shortcuts can speed up development initially, they often result in maintenance challenges, bugs, or scalability issues that require additional effort to address later.

Technical debt arises when false or suboptimal technical decisions are made, whether consciously or unconsciously. Such decisions lead to additional effort at a later point in time, which delays maintenance and expansion. 

When Technical Debt increases, the software system becomes error-prone, the development team gets a reputation for being sluggish, and changes that used to be possible within two person-days now take up to twice or three times as long.
 I have noticed that for every 500,000 lines of code (LOC), one or two full-time developers are required for maintenance. In other words, 40-80 hours per week per 500,000 LOC is a good starting point for determining the time needed to fix bugs and make small adjustments. If new functionality is to be integrated into the system, you will of course require even more capacity.

 #### Major causes of Technical Debt
 * No knowledge of software architecture
 * Complexity and size of software systems
 * Architectural erosion arises unnoticed
 * A lack of understanding of custom software development processes on the part of managers and customers

#### Types of Technical Debt
* Implementation Debt
* Design and Architecture Debt
* Test Debt
* Documentation Debt

##### Implementation Debt  
The source code contains “code smells”, such as long methods, code duplicates, and similar.

##### Design and architecture debt: 
The design of classes, packages, subsystems, layers, and modules is inconsistent or complex and does not fit the planned architecture. The source code contains “code smells”, such as long methods, code duplicates, and similar.

##### Test debt: 
Tests are missing or only the positive case is tested. The test coverage with automated unit tests is low. 
##### Documentation debt: 
There is no documentation, or the documentation that exists is incomplete or outdated. The overview of the architecture is not supported by the documents. Design decisions are not documented.

#### Minimize Technical Debt
* Architecture discussions within the team
* Key Metrics Monitoring
* Pair Programming
* Mob Programming
* Mob Architecting
![image](https://github.com/user-attachments/assets/05ab0b30-d86f-42c1-8c60-1e0533dd304d)

