# Table of Contents
- [Internet](#internet)
- [Language](#language)
- [Version Control System](#version-control-system)
- [Relational Databases](#relational-databases)
- [APIs](#apis)
- [Caching](#caching)

# Internet
## How does the internet work?
The internet is a global network of interconnected computers that communicate using standardized protocols, primarily TCP/IP. When you request awebpage, your device sends a data packet through your internet service provider (ISP) to a DNS server, which translates the website's domain name into an IP address. The packet is then routed across various networks (using routers and switches) to the destination server, which processes the request and sends back the response. 

**Summary: The internet is a global computer network that communicates via TCP/IP protocols; when you request a webpage, your device sends data packets through DNS resolution and routing to reach the target server, which then returns the requested information.**

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

**Summary: GraphQL is a query language and runtime for APIs that enables clients to request precisely the data they need from a single endpoint; unlike REST's fixed response structure, it uses a type system and schema to let clients specify their exact data requirements, reducing over-fetching and under-fetching while providing more flexible and efficient data retrieval for complex applications.**

## Authentication
API authentication is the process of verifying the identity of clients attempting to access an API, ensuring that only authorized users or applications can interact with the API's resources. Common methods include API keys, OAuth 2.0, JSON Web Tokens (JWT), basic authentication, and OpenID Connect. These techniques vary in complexity and security level, from simple token-based approaches to more sophisticated protocols that handle both authentication and authorization. API authentication protects sensitive data, prevents unauthorized access, enables usage tracking, and can provide granular control over resource access. The choice of authentication method depends on factors such as security requirements, types of clients, ease of implementation, and scalability needs. Implementing robust API authentication is crucial for maintaining the integrity, security, and controlled usage of web services and applications in modern, interconnected software ecosystems.

**Summary: API authentication verifies the identity of clients accessing an API through methods like API keys, OAuth, JWT, and OpenID Connect; it protects resources, prevents unauthorized access, enables usage tracking, and provides access control, with the appropriate method depending on security requirements, client types, implementation complexity, and scalability needs.**

## JWT
JWT (JSON Web Token) is an open standard for securely transmitting information between parties as a JSON object. It consists of three parts: a header (which specifies the token type and algorithm used for signing), a payload (which contains the claims or the data being transmitted), and a signature (which is used to verify the token's integrity and authenticity). JWTs are commonly used for authentication and authorization purposes, allowing users to securely transmit and validate their identity and permissions across web applications and APIs. They are compact, self-contained, and can be easily transmitted in HTTP headers, making them popular for modern web and mobile applications.

**Summary: JWT is an open standard for secure information exchange that consists of three parts (header, payload, signature); it's commonly used for authentication/authorization in web applications as it provides a compact, self-contained way to transmit user identity and permissions in a tamper-proof token that can be easily verified.**

## OAuth
OAuth is an open standard for authorization that allows third-party applications to access a user's resources without exposing their credentials. It works by issuing access tokens after users grant permission, which applications then use to interact with resource servers on behalf of the user. This process involves a resource owner (the user), a resource server (which holds the data), and an authorization server (which issues tokens). OAuth enables secure, token-based access management, commonly used for granting applications permissions to interact with services like social media accounts or cloud storage.

**Summary: OAuth is an authorization protocol that enables third-party applications to access user resources without requiring credentials; it uses a token-based system where users grant permission to applications, allowing secure delegated access to services like social media or cloud storage without exposing passwords.**

## Token authentication
Token-based authentication is a protocol which allows users to verify their identity, and in return receive a unique access token. During the life of the token, users then access the website or app that the token has been issued for, rather than having to re-enter credentials each time they go back to the same webpage, app, or any resource protected with that same token. Auth tokens work like a stamped ticket. The user retains access as long as the token remains valid. Once the user logs out or quits an app, the token is invalidated. Token-based authentication is different from traditional password-based or server-based authentication techniques. Tokens offer a second layer of security, and administrators have detailed control over each action and transaction.

**Summary: Token authentication is a stateless security method where users receive a unique token upon verification that grants access to protected resources for a limited time; it eliminates the need to repeatedly enter credentials, functions like a digital ticket, and provides administrators with granular control over user sessions and permissions.**

## Cookie-Based Authentication
Cookie-based authentication is a method of maintaining user sessions in web applications. When a user logs in, the server creates a session and sends a unique identifier (session ID) to the client as a cookie. This cookie is then sent with every subsequent request, allowing the server to identify and authenticate the user. The actual session data is typically stored on the server, with the cookie merely serving as a key to access this data. This approach is stateful on the server side and works well for traditional web applications. It's relatively simple to implement and is natively supported by browsers. However, cookie-based authentication faces challenges with cross-origin requests, can be vulnerable to CSRF attacks if not properly secured, and may not be ideal for modern single-page applications or mobile apps. Despite these limitations, it remains a common authentication method, especially for server-rendered web applications. 

**Summary: Cookie-based authentication maintains user sessions by storing a unique session ID in the client's browser cookies and keeping the actual session data on the server; this stateful approach is simple to implement and natively supported by browsers, but has limitations with cross-origin requests, CSRF vulnerabilities, and modern application architectures like SPAs and mobile apps.**

## OpenID
OpenID is an open standard for decentralized authentication that allows users to log in to multiple websites and applications using a single set of credentials, managed by an identity provider (IdP). It enables users to authenticate their identity through an external service, simplifying the login process and reducing the need for multiple usernames and passwords. OpenID typically works in conjunction with OAuth 2.0 for authorization, allowing users to grant access to their data while maintaining security. This approach enhances user convenience and streamlines identity management across various platforms.

**Summary: OpenID is a decentralized authentication standard that enables single sign-on across multiple websites and applications; it allows users to verify their identity through trusted third-party identity providers, eliminating the need for separate credentials for each service and typically working alongside OAuth for a complete authentication and authorization solution.**
Firebase:
Starts an OAuth 2.0 + OIDC flow with Google.
Receives the tokens (Access Token + ID Token).
Uses the ID token to create a Firebase session for that user.
You can then access firebase.auth().currentUser to get user info.

## Security Assertion Markup Language (SAML)
Security Assertion Markup Language (SAML) is an XML-based framework used for single sign-on (SSO) and identity federation, enabling users to authenticate once and gain access to multiple applications or services. It allows for the exchange of authentication and authorization data between an identity provider (IdP) and a service provider (SP). SAML assertions are XML documents that contain user identity information and attributes, and are used to convey authentication credentials and permissions. By implementing SAML, organizations can streamline user management, enhance security through centralized authentication, and simplify the user experience by reducing the need for multiple logins across different systems.

**Summary: SAML is an XML-based standard for implementing single sign-on and exchanging authentication data between identity providers and service providers; it uses XML assertions containing identity information to enable users to authenticate once and access multiple systems, providing enterprises with centralized identity management and improved security while enhancing user experience.**

# Caching
## Caching
Caching is a technique used in computing to store and retrieve frequently accessed data quickly, reducing the need to fetch it from the original, slower source repeatedly. It involves keeping a copy of data in a location that's faster to access than its primary storage. Caching can occur at various levels, including browser caching, application-level caching, and database caching. It significantly improves performance by reducing latency, decreasing network traffic, and lowering the load on servers or databases. Common caching strategies include time-based expiration, least recently used (LRU) algorithms, and write-through or write-back policies. While caching enhances speed and efficiency, it also introduces challenges in maintaining data consistency and freshness. Effective cache management is crucial in balancing performance gains with the need for up-to-date information in dynamic systems.

**Summary: Caching is a performance optimization technique that stores copies of frequently accessed data in faster storage locations; it operates at multiple levels (browser, application, database) to reduce latency, network traffic, and server load, using strategies like time-based expiration and LRU algorithms while balancing the trade-offs between speed and data consistency.**

## Server-side caching
Server-side caching is a technique used to improve application performance by storing frequently accessed data in memory on the server, reducing the need for repeated data retrieval or computation. This approach helps to speed up response times and reduce the load on databases and other backend services. Common methods include caching database query results, HTML fragments, and API responses. Popular server-side caching tools and technologies include Redis, Memcached, and built-in caching mechanisms in web frameworks. By efficiently managing and serving cached content, server-side caching enhances scalability and responsiveness of applications.

**Summary: Server-side caching stores frequently accessed data in memory on the server to improve performance; it reduces database and backend service load by temporarily storing query results, HTML fragments, and API responses using technologies like Redis and Memcached, resulting in faster response times and enhanced application scalability.**

## CDN (Content Delivery Network)
A Content Delivery Network (CDN) service aims to provide high availability and performance improvements of websites. This is achieved with fast delivery of website assets and content typically via geographically closer endpoints to the client requests.
Traditional commercial CDNs (Amazon CloudFront, Akamai, CloudFlare and Fastly) provide servers across the globe which can be used for this purpose. Serving assets and contents via a CDN reduces bandwidth on website hosting, provides an extra layer of caching to reduce potential outages and can improve website security as well

**Summary: CDNs are distributed server networks that deliver web content to users based on their geographic location; they improve website performance by serving assets from endpoints physically closer to users, reducing latency and bandwidth costs while enhancing reliability through additional caching layers and improving security through specialized protection mechanisms.**

## Client Side Caching
Client-side caching is a technique where web browsers or applications store data locally on the user's device to improve performance and reduce server load. It involves saving copies of web pages, images, scripts, and other resources on the client's system for faster access on subsequent visits. Modern browsers implement various caching mechanisms, including HTTP caching (using headers like Cache-Control and ETag), service workers for offline functionality, and local storage APIs. Client-side caching significantly reduces network traffic and load times, enhancing user experience, especially on slower connections. However, it requires careful management to balance improved performance with the need for up-to-date content. Developers must implement appropriate cache invalidation strategies and consider cache-busting techniques for critical updates. Effective client-side caching is crucial for creating responsive, efficient web applications while minimizing server resource usage.

**Summary: Client-side caching stores website resources locally on users' devices to improve performance and reduce server load; it uses browser mechanisms like HTTP headers, service workers, and storage APIs to save and retrieve content, significantly reducing load times and network traffic while requiring careful invalidation strategies to ensure content remains up-to-date.**
