# Study notes
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
- Shadow IT *Risk001*: use of nonsanctioned applications that hasn't been reviewed against organization's security policies, potentially introducing risk to the organization.
How to protect against shadow IT?
- Microsoft recommends a continuous process
  ```
  Discover Shadow IT > Identify risk levels of applications > Evaluate compliance > Analyze usage > Manage cloud applications > Continuous monitoring
  ```

### Catalog of Risks mentioned so far - with personal notes and views
*Risk001* Shadow IT
__Comment__: Shadow IT is a issue caused by a combination of ease of access, low cost of entry to cloud services, and lack of employee awareness.
Real life scenario: Using social media / messaging applications for business purpose | Subscribing to free online cloud services *harder to catch* | 
__Risk Analysis__: Business impact | Business and personal data at risk | Compliance impact
__Reactive Response__: Review and onboard service | Terminate use | Redirect users 
__Proactive Controls__: Employee awareness | Enforce data handling policies | Collaboration with legal, finance and procurement *very effective* | Monitor network traffic to detect cloud services used
