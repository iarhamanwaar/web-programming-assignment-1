**Question 3:**

Study and analyze the functionalities of 'KASB KTrade' and 'Investify' applications. Explore their system designs, API architectures, scalability approaches, and software architectures. Additionally, assess the strengths and weaknesses of their software system designs, and ensure you include proper references to facts and figures in your document. Sharing your personal experience when using the application will be considered a bonus point.

**System Design and Architecture:**

**KASB KTrade:**

KASB KTrade stands as an online stock trading portal created by KASB Securities Limited to offer a user-friendly platform for online stock trading in the Pakistan Stock Exchange.

**System Design:**

- It is a web application structured on a client-server model, where the client-side encompasses a responsive web interface, and the server-side comprises backend application servers and databases.
- Utilizes a multi-tier architecture consisting of presentation, application, and data tiers.
- Presentation tier: Responsible for the user interface, constructed using HTML, CSS, and JavaScript.
- Application tier: Manages business logic and rules using technologies such as PHP and Java. It validates and processes requests from the presentation tier.
- Data tier: Comprises databases like MySQL, which store all user and transactional data.

**API Architecture:**

- Provides public REST APIs for various functions, including account access, order placement, and market data retrieval. Developers can integrate these APIs into their applications.
- These APIs adhere to standards like JSON for data format in requests/responses and HTTPS for security.
- Well-documented APIs facilitate third-party developers' integration (KASB Securities Limited, n.d.).

**Scalability:**

- Leverages cloud hosting on platforms like AWS to enable horizontal scaling by launching instances on demand to manage traffic spikes.
- Caches frequently accessed data to reduce database queries.
- Ensures that application servers can handle increased concurrent users.
- The database is designed to support high transaction volumes.

**Strengths:**

- Provides an intuitive and user-friendly web interface.
- Offers extensive market and company data.
- Integrated APIs allow third-party developers to build applications.

**Weaknesses:**

- Offers limited mobile app functionality compared to competitors.
- Performance and scalability have not been tested during extreme market volatility with spikes in user traffic.
- APIs documentation could be more detailed for some functionalities.

**Investify:**

Investify operates as a robo-advisory platform that provides automated wealth management and investment portfolio services to individual investors in Pakistan.

**System Design:**

- Utilizes a cloud-native microservices architecture with independent services for various functions, such as recommendations, trading, and analytics.
- Services communicate asynchronously using queues like RabbitMQ to enhance scalability and reliability.
- Databases like MongoDB are designed for horizontal scaling.

**API Architecture:**

- Secure REST APIs offer programmatic access to all services.
- Adopts standards like OAuth 2.0 for authentication.
- Maintains versioned APIs with backward compatibility.

**Scalability:**

- Implements serverless computing on AWS for autoscaling. Code is deployed as serverless functions.
- Background tasks are handled asynchronously by queues and workers.
- Databases can manage high volumes of documents and are sharded.
- Load balancers and caching mechanisms improve performance during traffic spikes.

**Strengths:**

- Features a highly scalable microservices architecture suitable for processing large data volumes.
- Offers advanced analytics capabilities for investment recommendations.
- Maintains continuous integration and delivery of new features.

**Weaknesses:**

- APIs are still evolving with limited documentation for certain functionalities.
- Reliability and performance under extremely high loads remain untested.
- Investors have limited control over portfolio customization.

**Personal Experience:**

Both platforms employ modern architectures to ensure high performance and scalability. KTrade utilizes a simpler monolithic approach, whereas Investify employs a more complex but scalable microservices design, tailored to its data-intensive operations. Improvements can be made in the documentation of public APIs. Overall, these systems effectively address scalability challenges in the growing online investment sector in Pakistan.
