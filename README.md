# Study notes
Wish list - DevOps | DevSecOps | Penetration Testing | SOC | Container security | Kubernetes | Infrastructure as Code | Cryptography 
Stuff to figure out - API security, what is DKIM

## SC-100 Materials - Notes from Microsoft Learn
Components of Zero Trust
1. Identity
2. Endpoints
3. Applications
4. Network
5. Infrastructure
6. Data
Core Principles
1. Verify explicitly
2. Use least privilege access
3. Assume breach

### Applications
What are cloud services and shadow IT?
- Cloud Services: applications accessible anywhere with internet, allows rapid deployment and flexibility to scale and deploy.
- ***Risk001 - Shadow IT*** : use of nonsanctioned applications that hasn't been reviewed against organization's security policies, potentially introducing risk to the organization.
How to protect against shadow IT?
- Microsoft recommends a continuous process
  ```
  Discover Shadow IT > Identify risk levels of applications > Evaluate compliance > Analyze usage > Manage cloud applications > Continuous monitoring
  ```

## API Security
Application Programming Interface (API) allows software applications to interact with each other. API security is crucial as they enable access to sensitive function and data. This typically happens between client and servers over public network.

### Key characteristics
- Web applications have numerous endpoints that use different protocols and can expand over time
- Incoming requests formats that change frequently which is harder for traditional security tools to keep up (which is manual and error-prone)
- Clients oftendo not use a web browser, with requests coming from native and mobile applications or other service and software components. Web security tools cannot use browser verifications to detect malicious bots.

### Main architectural styles in modern APIs
- SOAP - highly structured message protocol that supports multiple low-level protocols.
- REST - simplier approach to use HTTP/S as the transport protocol and typically using JSON format for data transfer

### Some key issues with API Security
- Broken authentication and authorization
- Lack of rate limiting - Attackers can abuse API by scraping data / exceed usage limits
- Code injection to perform unauthorized operations or compromise backend
- Read more on OWASP API Top 10 Security Threats

## Catalog of Risks mentioned so far - with personal notes and views
***Risk001 - Shadow IT***  
  - __Comment__: Shadow IT is a issue caused by a combination of ease of access, low cost of entry to cloud services, and lack of employee awareness.  
  - __Real life scenario__: Using social media / messaging applications for business purpose | Subscribing to free online cloud services *harder to catch*  
  - __Risk Analysis__: Business impact | Business and personal data at risk | Compliance impact  
  - __Reactive Response__: Review and onboard service | Terminate use | Redirect users   
  - __Proactive Controls__: Employee awareness | Enforce data handling policies | Collaboration with legal, finance and procurement *very effective* | Monitor network traffic to detect cloud services used
