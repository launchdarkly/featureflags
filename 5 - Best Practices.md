## Get the most from your flags with our best practices.

#### [← Previous](./4%20-%20Cleaning%20Up.md) | [Table of Contents](./README.md) | [Next →](6%20-%20Flags%20vs%20Branching.md)

Flags are helpful when you think about how they help YOU and your organization. Feature flags should be first-class objects, not just sit in a config file that only developers can access.

#### Choose the Right Level of Flagging
At what level should you be feature flagging? Truthfully, it’s all dependent on the right level for your organization. There are some companies that flag everything at a very granular microservice level and have hundreds or thousands of flags. Others just like to use feature flags for a migration of one system to another. For example, when rolling out a dramatically new website, a dramatically new back-end, it’s common to put a feature flag in as a master switch. Start using them and see how they affect your feature release process. If you want more control, add more. If they’re cluttering up your application in a way you can’t control, take a step back and reexamine.

#### Flag Naming
Just because you are careful about flagging a feature doesn’t mean you’ve been careful with naming conventions. True story: two teams that both thought a particular feature flag was one for them only. They both started writing code that addressed this feature flag. And good analogy would be - imagine having a room with two light switches that control the same light and each person got progressively upset about whether the light was “on” or “off.” It took long time to get this solved and both parties were super frustrated. So long story short, be careful with naming.

Also consider what will happen with turnover. If flags aren’t labeled well, someone could mistakenly dial up flags controlling infrastructure and cause severe disruptions and outages.

A good rule of thumb is if a feature is always on or off, then the flag should be removed. For example, if a flag is added to ramp up between two systems or put out something with hypothesis-driven development, you should remove a flag once the rollout is complete. It's served its purpose.

#### Set Up Logging
Along these same lines, it’s helpful to log who has changed feature flags. This can help you solve who the question of “who made this change?” Once you know you can talk to them to figure out good next steps so that you can align everyone’s goals for the feature. There’s no wasted time, you already know who has rights (by organization, team, project, etc.).

#### Give Access to Non-Technical Users
Feature flags are most effective when they can be put in the hands of non-technical users (Product team, QA team, etc.). Figure out how to get this control into their hands as well as developers. This reduces a major bottleneck in feature control. This can also have an incredible effect on the Product-Engineering relationship and lead to more unified [rollout thinking](https://launchdarkly.com/casestudies/upserve.html).

#### Control Access to Flags
Many companies choose to give different members in their team different visibility and access to certain environments or groups of flags. One example would be to lock changes in the production environment from anyone in with a temporary login or anyone on the support team. When it comes to the rights to change a subscription, that can be real money. Potential to be destructive.

#### Flag Statuses
Flag statuses allow teams to manage both short and long-term flags, and know when flags are safe to remove. These statuses can be dynamically updated based on the flag’s usage. For example, if a flag was not used for over 7 days, then you could surface a status that would tell you that the flag is safe to remove from your code. These statuses give teams full visibility into their feature flag lifecycles, the ability to clean up flags that are obsolete, and know which features are rolled out.

#### [← Previous](./4%20-%20Cleaning%20Up.md) | [Table of Contents](./README.md) | [Next →](6%20-%20Flags%20vs%20Branching.md)
