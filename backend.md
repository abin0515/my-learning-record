# Table of Contents
- [Internet](#internet)
- [Language](#language)
- [Version Control System](#version-control-system)
- [Relational Databases](#relational-databases)
- [APIs](#apis)
- [Caching](#caching)
- [Web Security](#web-security)
- [Testing](#testing)
- [CI/CD](#cicd)

# Internet
## How does the internet work?
The internet is a global network of interconnected computers that communicate using standardized protocols, primarily TCP/IP. When you request awebpage, your device sends a data packet through your internet service provider (ISP) to a DNS server, which translates the website's domain name into an IP address. The packet is then routed across various networks (using routers and switches) to the destination server, which processes the request and sends back the response. 

**Summary: The internet is a global computer network that communicates via TCP/IP protocols; when you request a webpage, your device sends data packets through DNS resolution and routing to reach the target server, which then returns the requested information.**

## What is HTTP?
HTTP (Hypertext Transfer Protocol) is the foundation of web communication, enabling data exchange between clients and servers. It follows a simple request-response pattern where clients (like web browsers) request resources and servers respond with the requested content. Each request is independent (stateless), meaning servers don't remember previous interactions. HTTP is typically used with HTTPS for secure, encrypted communication.

**Summary: HTTP is the core protocol of the web that enables communication between clients and servers through a stateless request-response model, where each request is independent and servers respond with requested resources.**

## What is domain name?
A domain name is a human-friendly address that helps users access websites on the internet. Instead of using numerical IP addresses, domain names provide memorable names like "example.com". Each domain name has two main parts: the name (like "example") and the extension (like ".com"). These names are registered and managed through domain registrars, making it easy for users to find and access websites.

**Summary: Domain names are user-friendly internet addresses that replace numerical IP addresses with memorable names like example.com, making it easier for users to access websites through a simple, readable format.**

## What is hosting?
Hosting is a service that provides the necessary infrastructure to make websites accessible on the internet. It includes server space, storage, and network connectivity to store and deliver website files. Different hosting options are available: shared hosting (multiple websites on one server), VPS (virtual private servers), dedicated hosting (one server per user), and cloud hosting (scalable resources across multiple servers). Hosting providers typically offer additional services like domain registration, security features, and technical support to ensure reliable website operation.

**Summary: Hosting provides the infrastructure needed to make websites accessible online, offering various options from shared to dedicated servers, along with essential services like storage, security, and technical support.**

## DNS and how it works?
DNS (Domain Name System) is like the internet's phone book, translating human-readable domain names into IP addresses that computers use to communicate. It works through a network of servers worldwide, organized in a hierarchy: root servers at the top, followed by top-level domain servers (.com, .org, etc.), and then servers for specific domains. When you enter a domain name, DNS servers work together to find the corresponding IP address, making it possible to access websites using memorable names instead of numbers. This system is essential for internet navigation and supports various online services.

**Summary: DNS is the internet's directory service that converts domain names into IP addresses; it uses a global network of servers working together to help users access websites using memorable names instead of numerical addresses.**

## Browsers and how they work?
Web browsers are applications that help users access and interact with websites. They interpret HTML, CSS, and JavaScript to display web pages and provide features like tabbed browsing, bookmarks, and extensions. Modern browsers use specialized engines (like Chrome's Blink or Firefox's Gecko) to process web content and run JavaScript code. They also include security features to protect users while browsing. Popular browsers like Chrome, Firefox, Safari, and Edge support modern web standards and technologies, making them powerful platforms for accessing and interacting with web content.

**Summary: Web browsers are applications that display web pages and enable user interaction; they use specialized engines to process web content, provide features like tabs and bookmarks, and include security measures to protect users while browsing.**

# Language
## JavaScript
JavaScript is a flexible programming language that powers interactive features on websites. It runs in web browsers to create dynamic content and respond to user actions. With Node.js, JavaScript can also run on servers, making it a versatile tool for both frontend and backend development.

**Summary: JavaScript is a versatile language that powers both web browser interactivity and server-side applications through Node.js, enabling developers to create dynamic, interactive web experiences.**

## Java
Java is a powerful programming language designed for building large-scale applications. It's known for its reliability and ability to run on any platform. Java includes features like automatic memory management and a comprehensive library of tools. It's widely used for enterprise software, Android apps, and cloud services.

**Summary: Java is a reliable, cross-platform language with built-in memory management and extensive libraries, making it ideal for enterprise applications, Android development, and cloud services.**

# Version Control System
## Github
GitHub is a popular platform for managing and sharing code. Built on Git, it provides tools for team collaboration, code review, and project management. Key features include code repositories, pull requests for reviewing changes, issue tracking, and automated workflows. GitHub supports both public and private projects, making it ideal for both open-source and private development. It's widely used by developers to store code, collaborate with teams, and showcase their work.

**Summary: GitHub is a code hosting platform that enhances Git with collaboration tools, offering features for code management, team collaboration, and project tracking, serving as a central hub for both open-source and private software development.**

# Relational Databases
## Relational Databases
Relational databases store data in organized tables with rows and columns, using SQL to manage and query the data. They maintain data relationships through keys and constraints, ensuring data integrity. This structure makes it easy to handle complex queries and transactions, making them ideal for applications that need structured data storage.

**Summary: Relational databases organize data in tables with defined relationships, using SQL for data management and ensuring data integrity through keys and constraints, making them perfect for structured data storage and complex queries.**

## PostgreSQL
PostgreSQL is a powerful open-source database system known for its advanced features and reliability. It supports complex queries, custom data types, and full-text search. With strong data integrity and ACID compliance, it's suitable for both small applications and large-scale data systems.

**Summary: PostgreSQL is a feature-rich open-source database that excels at handling complex queries and custom data types, offering strong data integrity and ACID compliance for applications of all sizes.**

## MySQL
MySQL is a popular database system known for its speed and ease of use. It's widely used in web applications and works well with various programming languages. As part of the LAMP stack, it provides reliable data storage and management for many types of applications.

**Summary: MySQL is a fast and user-friendly database system that's widely used in web applications, offering reliable data management and easy integration with various programming languages and platforms.**

# APIs
APIs (Application Programming Interfaces) are sets of rules that allow different software applications to communicate with each other. They provide a standardized way to access and use services or data without needing to understand their internal workings. APIs can be public or private and are essential for integrating different systems and enabling third-party development.

**Summary: APIs are standardized interfaces that enable software applications to communicate and exchange data, providing a set of rules and tools for accessing functionality without requiring knowledge of the underlying implementation.**

## Open API Specs
OpenAPI Specification (OAS) is a standard format for describing and documenting RESTful APIs. It uses YAML or JSON to define API endpoints, data formats, and authentication methods. This specification helps developers create clear documentation and enables automated tools to generate client libraries and testing tools.

**Summary: OpenAPI Specification is a standardized format for documenting RESTful APIs, making it easier to understand, test, and integrate with APIs through automated tools and clear documentation.**

## REST
REST (Representational State Transfer) is a design style for building networked applications. It uses standard HTTP methods (GET, POST, PUT, DELETE) to interact with resources identified by URLs. REST APIs are stateless, meaning each request contains all necessary information, making them simple and scalable.

**Summary: REST is a design style for web applications that uses standard HTTP methods to interact with resources, following principles like statelessness to create simple, scalable APIs.**

## JSON APIs
JSON APIs use JavaScript Object Notation as a lightweight format for exchanging data between clients and servers. This format is easy to read and write, making it popular for web services and APIs across different platforms and programming languages.

**Summary: JSON APIs use a simple, readable format for exchanging data between clients and servers, making it easy to work with across different platforms and languages.**

## gRPC
gRPC is a modern framework for building fast, efficient communication between services. It allows programs to call functions in remote applications as if they were local, supporting multiple programming languages and providing features like streaming and authentication.

**Summary: gRPC is a high-performance framework that enables programs to call remote functions as if they were local, supporting multiple languages and providing features like streaming for efficient service communication.**

## GraphQL
GraphQL is a query language for APIs that lets clients request exactly the data they need. Unlike traditional APIs that return fixed data structures, GraphQL allows clients to specify their data requirements, reducing unnecessary data transfer and making API interactions more efficient.

**Summary: GraphQL is a flexible query language that lets clients request exactly the data they need from APIs, making data fetching more efficient by eliminating unnecessary data transfer.**

## Authentication
API authentication verifies the identity of users or applications trying to access an API. It uses various methods like API keys, OAuth, JWT, and OpenID Connect to ensure only authorized users can access protected resources. These methods provide different levels of security and are chosen based on the application's needs.

**Summary: API authentication uses methods like API keys, OAuth, and JWT to verify user identity and control access to protected resources, ensuring only authorized users can access sensitive data and services.**

## JWT
JWT (JSON Web Token) is a secure way to transmit information between parties as a JSON object. It consists of three parts: a header, a payload (containing the data), and a signature (for verification). JWTs are commonly used for authentication and authorization in web applications.

**Summary: JWT is a secure token format that transmits user information in three parts (header, payload, signature), commonly used for authentication in web applications.**

## OAuth
OAuth is a standard that allows third-party applications to access user resources without sharing passwords. It works by issuing access tokens after users grant permission, enabling secure access to services like social media accounts or cloud storage.

**Summary: OAuth enables secure access to user resources through tokens, allowing third-party applications to interact with services without exposing user credentials.**

## Token authentication
Token authentication is a method where users receive a unique token after verifying their identity. This token grants access to protected resources without requiring repeated login. The token remains valid until the user logs out or it expires, providing a secure and convenient way to maintain user sessions.

**Summary: Token authentication uses unique tokens to grant access to protected resources, eliminating the need for repeated logins while maintaining security through token validation and expiration.**

## Cookie-Based Authentication
Cookie-based authentication uses browser cookies to maintain user sessions. When a user logs in, the server creates a session and sends a session ID cookie. This cookie is sent with each request, allowing the server to identify the user. While simple to implement, it has limitations with cross-origin requests and modern web applications.

**Summary: Cookie-based authentication uses browser cookies to maintain user sessions, sending a session ID with each request to identify users, though it has limitations with modern web applications and cross-origin requests.**

## OpenID
OpenID is a standard that enables users to log in to multiple websites using a single set of credentials. It works with identity providers to verify user identity, simplifying the login process and reducing the need for multiple usernames and passwords.

**Summary: OpenID enables single sign-on across multiple websites, allowing users to use one set of credentials through trusted identity providers.**

## Security Assertion Markup Language (SAML)
SAML is an XML-based standard for implementing single sign-on and exchanging authentication data between identity providers and service providers. It uses XML assertions to convey user identity information, enabling secure access to multiple systems with a single login.

**Summary: SAML is an XML-based standard for single sign-on that securely exchanges authentication data between identity providers and service providers, enabling users to access multiple systems with one login.**

# Caching
## Caching
Caching stores frequently accessed data in faster storage locations to improve performance. It reduces the need to fetch data from slower sources repeatedly, operating at various levels like browser, application, and database caching. This technique improves speed and efficiency while balancing data freshness.

**Summary: Caching improves performance by storing frequently used data in faster locations, reducing the need to fetch from slower sources while managing the balance between speed and data freshness.**

## Server-side caching
Server-side caching stores frequently accessed data in server memory to improve application performance. It reduces database load by temporarily storing query results and API responses, using tools like Redis and Memcached to speed up response times.

**Summary: Server-side caching improves performance by storing frequently accessed data in server memory, reducing database load and speeding up response times using tools like Redis and Memcached.**

## CDN (Content Delivery Network)
CDNs are networks of servers distributed worldwide that deliver web content to users based on their location. They improve website performance by serving content from servers closer to users, reducing latency and bandwidth costs while enhancing reliability and security.

**Summary: CDNs are distributed server networks that deliver web content from locations closer to users, improving website performance, reducing latency, and enhancing reliability and security.**

## Client Side Caching
Client-side caching stores website resources locally on users' devices to improve performance. It uses browser mechanisms like HTTP headers and storage APIs to save and retrieve content, reducing load times and network traffic while requiring careful management of content updates.

**Summary: Client-side caching stores website resources locally on users' devices, using browser mechanisms to improve performance and reduce server load while managing content freshness.**

# Web Security
## Web Security
Web security protects applications from threats and vulnerabilities. It includes measures like strong authentication, encryption for data transmission, and input validation to prevent attacks. Regular security testing and updates help maintain application security and user trust.

**Summary: Web security implements multiple layers of protection including authentication, encryption, and input validation to safeguard applications from threats while maintaining user trust through regular testing and updates.**

## Scrypt
Scrypt is a password hashing function designed to resist brute-force attacks by using significant memory and computational resources. It makes password cracking impractical, especially against specialized hardware like GPUs and ASICs, making it effective for secure password storage.

**Summary: Scrypt is a memory-hard password hashing function that makes password cracking computationally expensive by using substantial resources, particularly effective against specialized hardware attacks.**

## Bcrypt
Bcrypt is a secure password hashing function that includes built-in salting to prevent rainbow table attacks. Its key feature is an adjustable cost factor that can be increased over time to maintain security against growing computational power.

**Summary: Bcrypt is a secure password hashing function with built-in salting and an adjustable cost factor, making it resistant to rainbow table attacks and adaptable to increasing computational power.**

# Testing
## Testing
Testing is a systematic process to evaluate software functionality, performance, and quality. It includes various levels like unit testing (individual components), integration testing (component interactions), system testing (entire system), and acceptance testing (user requirements). Testing can be manual or automated, aiming to identify defects and ensure reliable performance.

**Summary: Testing systematically evaluates software through multiple levels (unit, integration, system, acceptance) to ensure functionality, identify defects, and verify reliable performance.**

## Unit Testing
Unit testing checks individual code components in isolation to ensure they work correctly. Developers write automated tests with predefined inputs to verify each component's behavior, helping catch bugs early and support safe code changes.

**Summary: Unit testing verifies individual code components in isolation using automated tests, helping catch bugs early and ensuring each piece of functionality works correctly.**

## Functional Testing
Functional testing verifies that software meets its specified requirements by testing its behavior from a user's perspective. It's typically done as black box testing, where testers check inputs and outputs without knowing the internal code structure.

**Summary: Functional testing verifies software meets requirements by testing from a user's perspective, focusing on inputs and outputs without knowledge of internal code.**

# CI/CD
## CI/CD
CI/CD (Continuous Integration/Continuous Delivery) is a set of practices that automate the software development process. It consists of three main parts:

1. Continuous Integration (CI): Developers regularly merge their code changes into a central repository. Each merge triggers automated builds and tests to catch issues early.

2. Continuous Delivery (CD): Code changes are automatically deployed to testing environments. This ensures the code is always in a deployable state.

3. Continuous Deployment (CD): In some implementations, changes are automatically deployed to production after passing all tests.

This approach helps teams:
- Find and fix bugs quickly
- Reduce manual work
- Ensure consistent code quality
- Speed up the development process

**Summary: CI/CD automates software development by integrating code changes, running tests, and deploying updates automatically, helping teams catch issues early and maintain high code quality.**

# More about Databases
## ORMs
Object-Relational Mapping (ORM) is a programming technique that allows developers to interact with a relational database using object-oriented programming concepts. ORM frameworks map database tables to classes and rows to objects, enabling developers to perform database operations through objects rather than writing raw SQL queries. This abstraction simplifies data manipulation and improves code maintainability by aligning database interactions with the application's object model. ORM tools handle the translation between objects and database schemas, manage relationships, and often provide features like lazy loading and caching. Popular ORM frameworks include Hibernate for Java, Entity Framework for .NET, and SQLAlchemy for Python.

**Summary: ORM is a technique that lets developers work with databases using object-oriented programming, mapping database tables to classes and rows to objects, making database operations more intuitive and maintainable while reducing the need to write raw SQL queries.**

## ACID
ACID is an acronym representing four key properties that guarantee reliable processing of database transactions. It stands for Atomicity, Consistency, Isolation, and Durability. Atomicity ensures that a transaction is treated as a single, indivisible unit that either completes entirely or fails completely. Consistency maintains the database in a valid state before and after the transaction. Isolation ensures that concurrent transactions do not interfere with each other, appearing to execute sequentially. Durability guarantees that once a transaction is committed, it remains so, even in the event of system failures. These properties are crucial in maintaining data integrity and reliability in database systems, particularly in scenarios involving multiple, simultaneous transactions or where data accuracy is critical, such as in financial systems or e-commerce platforms.

**Summary: ACID is a set of four properties (Atomicity, Consistency, Isolation, Durability) that ensure database transactions are reliable and maintain data integrity, making sure transactions are either fully completed or fully failed, keeping data consistent, handling multiple transactions safely, and preserving changes even after system failures.**