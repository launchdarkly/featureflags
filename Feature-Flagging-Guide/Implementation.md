#Implementation Tips
Here are some tips to help you integrate feature flagging into your development process.

Before you select a feature flagging method, you should:

1. **Identify your current pain points** - what is currently difficult to do? What issues keep arising in your development workflow? What issues keep arising in production?

2. **Identify your use cases** - what would you use feature flags for? Who are the stakeholders besides developers? (Product, Business, Sales, etc) Do you want to facilitate team collaboration?

3. **Research a build versus buy solution that takes into consideration:**

    * Total cost of ownership: Homegrown tools are built to exist and serve a particular function, but with new business demands comes the cost of upgrades. There is a high cost to ongoing maintenance, both in time and money. Technical debt accrues over time due to engineer turnover, product neglect, and evolving product demands.
    * Unknown And Evolving Scope: Developing an internal product requires planning, resource allocation, and preparing for the unknown. Because feature flagging platforms are relatively new, it can be difficult to accurately define the scope and construct a solution for needs across not only engineering but also product groups.
    * Minimum Viable Functionality: Internal developer tools are generally not built for usability, scalability, or cross-team support. They are built to solve an immediate pain point or provide minimum viable functionality as quickly as possible.
    * Polyglot Language Support: Companies typically use multiple languages in their stacks and might adopt new languages in the future. This requires an adaptive feature flagging system that can handle the nuances of each language without compromising performance and stability.
    * Compliance: Company-wide internal tools require access controls, audit logs, and potentially custom permissions to ensure that functionality is controlled at an appropriate level.

4. **The Decision** - If you’re looking to build your own platform, this page provides a list of feature flag libraries for every programming language. This can act as a nice starting point to understand the scope of the undertaking. If you’re looking to purchase a platform, you want to make sure that you are integrating a well-tested and proven solution. The platform should also allow you the flexibility to integrate feature flag driven development across teams and across products (web and mobile), either through an on-premise/private instance or managed cloud platform You want to ensure that the feature flagging platform is:
    * Stable
    * Multi-language Compatible
    * Scalable
    * Intuitive 
    * Well-Supported

5. **Integration and Team Coordination** - Feature flag-driven development is both an engineering practice and a cultural shift for your teams. It is a practice that emphasizes team collaboration, feedback, and full release lifecycle management. Therefore, it is important that teams incorporation feature flag release strategy into their continuous delivery pipeline. This release strategy is a DevOps concept where teams integrate feature release planning into the development process. Instead of pushing a new feature to production and being done with it, developers integrate feature flags into the development lifecycle to control their releases. Broadly speaking, feature flagging is a way to control the visibility and on/off state of a particular feature by wrapping the code in a conditional. The process of flagging encourages developers to plan for the initial feature rollout, feature improvements based on user feedback, and overall feature adoption.

Thanks for reading LaunchDarkly’s Guide to Feature Flagging! If you have any feedback, please reach out to us at info@launchdarkly.com. We’d love your help in making this even more complete and useful.
