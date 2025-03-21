# Table of Contents
- [Internet](#internet)
- [Language](#language)
- [Version Control System](#version-control-system)
- [Relational Databases](#relational-databases)
- [APIs](#apis)

# Internet
## How does the internet work?
The internet is a global network of interconnected computers that communicate using standardized protocols, primarily TCP/IP. When you request awebpage, your device sends a data packet through your internet service provider (ISP) to a DNS server, which translates the website's domain name into an IP address. The packet is then routed across various networks (using routers and switches) to the destination server, which processes the request and sends back the response. 

**Summary: The internet is a global computer network that communicates via TCP/IP protocols; when you request a webpage, your device sends data packets through DNS resolution and routing to reach the target server, which then returns the re quested information.**

## What is HTTP?
HTTP (Hypertext Transfer Protocol) is a protocol used for transmitting hypertext via the World Wide Web. It defines how messages are formatted and transmitted, and how web servers and browsers should respond to various commands. HTTP operates on a request-response model: a client (usually a web browser) sends an HTTP request to a server for resources, such as web pages or files, and the server responds with the requested content and an HTTP status code indicating the result of the request. HTTP is stateless, meaning each request from a client to a server is independent and does not retain information about previous interactions. It forms the foundation of data communication on the web and is typically used with secure HTTP (HTTPS) for encrypted communication.

**Summary: HTTP is a stateless request-response protocol that governs how web browsers and servers communicate; it defines how web content is requested, formatted, transmitted, and received, forming the foundation of data exchange on the World Wide Web.**

## What is domain name?
A domain name is a human-readable address used to identify a specific location on the internet, making it easier to access websites and online services. It translates to an IP address, which is a numerical identifier used by computers to locate and connect to servers. A domain name consists of two main parts: the second-level domain (e.g., "example" in "example.com") and the top-level domain (e.g., ".com"). Domain names are managed by domain name registrars and are essential for establishing a web presence, providing a user-friendly way to navigate to websites instead of using numeric IP addresses.

**Summary: Domain names are human-readable internet addresses that map to numeric IP addresses; they consist of second-level and top-level domains (like example.com) and serve as user-friendly identifiers that eliminate the need to remember complex IP numbers when accessing websites.**

## What is hosting?
Hosting refers to the service of providing server space and resources for storing and delivering website files and applications to users over the internet. Hosting providers offer the infrastructure, such as servers, storage, and network connectivity, required to make websites and applications accessible online. There are various types of hosting, including shared hosting (where multiple websites share a single server), virtual private servers (VPS), dedicated hosting (where a single server is dedicated to one user), and cloud hosting (which uses a network of servers to provide scalable resources). Hosting services often include domain registration, security features, and technical support to ensure websites are reliably available and perform well.

**Summary: Hosting is a service that provides server space and technical infrastructure to store website files and make them accessible online; it comes in various types (shared, VPS, dedicated, cloud) and typically includes resources for storage, connectivity, security, and support to ensure website availability.**

## DNS and how it works?
DNS (Domain Name System) is a hierarchical, decentralized naming system for computers, services, or other resources connected to the Internet or a private network. It translates human-readable domain names (like www.example.com) into IP addresses (like 192.0.2.1) that computers use to identify each other. DNS servers distributed worldwide work together to resolve these queries, forming a global directory service. The system uses a tree-like structure with root servers at the top, followed by top-level domain servers (.com, .org, etc.), authoritative name servers for specific domains, and local DNS servers. DNS is crucial for the functioning of the Internet, enabling users to access websites and services using memorable names instead of numerical IP addresses. It also supports email routing, service discovery, and other network protocols.

**Summary: DNS is a hierarchical naming system that translates domain names into IP addresses; it works through a global network of servers organized in levels (root, TLD, authoritative, local) that work together to resolve queries, allowing users to access websites using memorable names rather than numeric addresses.**


## Browsers and how they work?
Web browsers are software applications that enable users to access, retrieve, and navigate information on the World Wide Web. They interpret and display HTML, CSS, and JavaScript to render web pages. Modern browsers like Google Chrome, Mozilla Firefox, Apple Safari, and Microsoft Edge offer features such as tabbed browsing, bookmarks, extensions, and synchronization across devices. They incorporate rendering engines (e.g., Blink, Gecko, WebKit) to process web content, and JavaScript engines for executing code. Browsers also manage security through features like sandboxing, HTTPS enforcement, and pop-up blocking. They support various web standards and technologies, including HTML5, CSS3, and Web APIs, enabling rich, interactive web experiences. With the increasing complexity of web applications, browsers have evolved to become powerful platforms, balancing performance, security, and user experience in the ever-changing landscape of the internet.

**Summary: Web browsers are applications that translate HTML, CSS, and JavaScript into visual web pages; they use specialized rendering engines (like Blink, Gecko, WebKit) and JavaScript engines to process content, while providing features for navigation, security, and customization through extensions, making them sophisticated platforms for accessing and interacting with web content.**

# Language
## JavaScript
JavaScript is a versatile, high-level programming language primarily used for adding interactivity and dynamic features to websites. It runs in the browser, allowing for client-side scripting that can manipulate HTML and CSS, respond to user events, and interact with web APIs. JavaScript is also used on the server side with environments like Node.js, enabling full-stack development. 

**Summary: JavaScript is a versatile scripting language used in both frontend and backend development, enhancing webpage interactivity in browsers and enabling server-side development through Node.js.**

## Java
Java is a high-level, object-oriented programming language known for its portability, robustness, and scalability.It's widely used for building large-scale enterprise applications, Android mobile apps, and web services. Java features automatic memory management (*garbage collection*), a vast standard library, and strong security features, making it a popular choice for backend systems, distributed applications, and cloud-based solutions.

**Summary: Java is a "write once, run anywhere" object-oriented language, renowned for its reliability and cross-platform capabilities, widely used in enterprise systems and Android application development.**

# Version Control System
## Github
GitHub is a web-based platform for version control and collaboration using Git. Owned by Microsoft, it provides hosting for software development and offers features beyond basic Git functionality. GitHub includes tools for project management, code review, and social coding. Key features include repositories for storing code, pull requests for proposing and reviewing changes, issues for tracking bugs and tasks, and actions for automating workflows. It supports both public and private repositories, making it popular for open-source projects and private development. GitHub's collaborative features, like forking repositories and inline code comments, facilitate team development and community contributions. With its extensive integrations and large user base, GitHub has become a central hub for developers, serving as a portfolio, collaboration platform, and deployment tool for software projects of all sizes.

**Summary: GitHub is a web-based platform that extends Git with collaboration features for software development; it offers repositories, pull requests, issues tracking, and workflow automation, serving as both a code hosting service and social coding platform where developers can manage projects, review code, and collaborate on both open-source and private initiatives.**

# Relational Databases
## Relational Databases
Relational databases are a type of database management system (DBMS) that organizes data into structured tables with rows and columns, using a schema to define data relationships and constraints. They employ Structured Query Language (SQL) for querying and managing data, supporting operations such as data retrieval, insertion, updating, and deletion. Relational databases enforce data integrity through keys (primary and foreign) and constraints (such as unique and not-null), and they are designed to handle complex queries, transactions, and data relationships efficiently. Examples of relational databases include MySQL, PostgreSQL, and Oracle Database. They are commonly used for applications requiring structured data storage, strong consistency, and complex querying capabilities.

**Summary: Relational databases organize data in structured tables with predefined schemas and relationships; they use SQL for data operations, enforce integrity through keys and constraints, and excel at handling complex queries and transactions, making them ideal for applications requiring consistent, structured data storage with well-defined relationships.**

## PostgreSQL
PostgreSQL is an advanced, open-source relational database management system (RDBMS) known for its robustness, extensibility, and standards compliance. It supports a wide range of data types and advanced features, including complex queries, foreign keys, and full-text search. PostgreSQL is highly extensible, allowing users to define custom data types, operators, and functions. It supports ACID (Atomicity, Consistency, Isolation, Durability) properties for reliable transaction processing and offers strong support for concurrency and data integrity. Its capabilities make it suitable for various applications, from simple web apps to large-scale data warehousing and analytics solutions.

**Summary: PostgreSQL is an advanced open-source relational database system known for its extensibility, standards compliance, and robust feature set; it supports ACID transactions, custom data types, and complex queries while maintaining data integrity, making it suitable for applications ranging from small web services to large-scale data warehousing.**

## MySQL
MySQL is an open-source relational database management system (RDBMS) known for its speed, reliability, and ease of use. It uses SQL (Structured Query Language) for database interactions and supports a range of features for data management, including transactions, indexing, and stored procedures. MySQL is widely used for web applications, data warehousing, and various other applications due to its scalability and flexibility. It integrates well with many programming languages and platforms, and is often employed in conjunction with web servers and frameworks in popular software stacks like LAMP (Linux, Apache, MySQL, PHP/Python/Perl). MySQL is maintained by Oracle Corporation and has a large community and ecosystem supporting its development and use.

**Summary: MySQL is a popular open-source relational database system valued for its speed, reliability, and ease of use; it's a core component of the LAMP stack and many web applications, offering SQL-based data management features like transactions and indexing while maintaining good integration with various programming languages and platforms.**

# APIs
## APIs
An API (Application Programming Interface) is a set of defined rules and protocols that allow different software applications to communicate and interact with each other. It provides a standardized way for developers to access and manipulate the functionalities or data of a service, application, or platform without needing to understand its internal workings. APIs can be public or private and are commonly used to integrate disparate systems, facilitate third-party development, and enable interoperability between applications. They typically include endpoints, request methods (like GET, POST, PUT), and data formats (like JSON or XML) to interact with.

**Summary: APIs are standardized interfaces that enable different software applications to communicate and exchange data; they provide a set of rules, protocols, and tools for accessing functionality without requiring knowledge of the underlying implementation. They typically include endpoints, request methods (like GET, POST, PUT), and data formats (like JSON or XML) to interact with.**

## Open API Specs
The OpenAPI Specification (OAS), formerly known as Swagger, is a standard for defining and documenting RESTful APIs. It provides a structured format in YAML or JSON to describe API endpoints, request and response formats, authentication methods, and other metadata. By using OAS, developers can create a comprehensive and machine-readable API description that facilitates client generation, automated documentation, and testing. This specification promotes consistency and clarity in API design, enhances interoperability between different systems, and enables tools to generate client libraries, server stubs, and interactive API documentation.

**Summary: OpenAPI Specification is a standardized format for describing RESTful APIs using YAML or JSON; it documents endpoints, request/response formats, and authentication methods, enabling automated client generation, interactive documentation, and consistent API design across different systems and tools.**

## REST
A REST API (Representational State Transfer Application Programming Interface) is an architectural style for designing networked applications. It relies on standard HTTP methods (GET, POST, PUT, DELETE) to interact with resources, which are represented as URIs (Uniform Resource Identifiers). REST APIs are stateless, meaning each request from a client to a server must contain all the information needed to understand and process the request. They use standard HTTP status codes to indicate the outcome of requests and often communicate in formats like JSON or XML. REST APIs are widely used due to their simplicity, scalability, and ease of integration with web services and applications.

**Summary: REST is an architectural style for designing networked applications that uses standard HTTP methods to interact with resources identified by URIs; it follows key principles including statelessness and standardized operations, making it popular for its simplicity, scalability, and compatibility with the web's infrastructure.**

## JSON APIs
JSON or JavaScript Object Notation is an encoding scheme that is designed to eliminate the need for an ad-hoc code for each application to communicate with servers that communicate in a defined way. JSON API module exposes an implementation for data stores and data structures, such as entity types, bundles, and fields.

**Summary: JSON APIs use JavaScript Object Notation as a lightweight data interchange format for client-server communication; they provide a standardized way to structure data that's both human-readable and machine-parsable, making it an efficient choice for web services and APIs across different platforms and programming languages.**

## gRPC
gRPC is a high-performance, open source universal RPC framework, RPC stands for Remote Procedure Call, there's an ongoing debate on what the g stands for. RPC is a protocol that allows a program to execute a procedure of another program located on another computer. The great advantage is that the developer doesn't need to code the details of the remote interaction. The remote procedure is called like any other function. But the client and the server can be coded in different languages.

**Summary: gRPC is a high-performance RPC framework that enables programs to call functions in remote applications as if they were local; it uses Protocol Buffers for efficient serialization, supports bidirectional streaming, and allows cross-language communication, making it ideal for building distributed systems and microservices architectures.**

## GraphQL
GraphQL is a query language for APIs and a runtime for executing those queries, developed by Facebook. Unlike REST, where fixed endpoints return predefined data, GraphQL allows clients to request exactly the data they need, making API interactions more flexible and efficient. It uses a single endpoint and relies on a schema that defines the types and structure of the available data. This approach reduces over-fetching and under-fetching of data, making it ideal for complex applications with diverse data needs across multiple platforms (e.g., web, mobile).

**Summary: GraphQL is a query language for APIs. Unlike REST, GraphQL allows clients to request exactly the data they need, making API interactions more flexible and efficient.**

## Authentication
API authentication is the process of verifying the identity of clients attempting to access an API, ensuring that only authorized users or applications can interact with the API's resources. Common methods include API keys, OAuth 2.0, JSON Web Tokens (JWT), basic authentication, and OpenID Connect. These techniques vary in complexity and security level, from simple token-based approaches to more sophisticated protocols that handle both authentication and authorization. API authentication protects sensitive data, prevents unauthorized access, enables usage tracking, and can provide granular control over resource access. The choice of authentication method depends on factors such as security requirements, types of clients, ease of implementation, and scalability needs. Implementing robust API authentication is crucial for maintaining the integrity, security, and controlled usage of web services and applications in modern, interconnected software ecosystems.

**Summary: API authentication verifies the identity of clients accessing an API through methods like API keys, OAuth, JWT, and OpenID Connect; it protects resources, prevents unauthorized access, enables usage tracking, and provides access control, with the appropriate method depending on security requirements, client types, implementation complexity, and scalability needs.**