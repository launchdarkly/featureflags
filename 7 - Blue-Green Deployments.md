## Handling risk with proper release management.

#### [← Previous](./6%20-%20Flags%20vs%20Branching.md) | [Table of Contents](./README.md) | [Next →](8%20-%20Database%20Migrations.md)

#### Using feature flags for granular release control and risk mitigation for blue-green deployments

Blue-green deployments have long been a proven technique to mitigate risk in software releases. By adding feature flags, developers are ushering in a new era of blue-green deployments, one with unprecedented granular control over feature releases. This article discusses how to effectively integrate feature flags into your blue-green deployment process.

At its core, a blue-green deployment is a release practice that maintains two production environments called blue and green, switching between whether the blue or green environment is live. The primary benefit of this approach is to mitigate risk and control the timing of releases. The blue version might have the new version and green the old version. If something goes wrong, you can switch back to the more stable environment.

The old way of blue-green deployments was more of an all-or-none approach. Traffic was funneled in a binary fashion, all to blue or all to green. It was also focused around timing: you could determine when you wanted to switch traffic and then switch back if something went wrong.

![bluegreen](https://featureflags.io/wp-content/uploads/2018/03/bluegreen.jpg "blue-green deployment")

Blue-green deployments, therefore, are a macro level of risk mitigation. You are not focusing on testing smaller features, like a new search bar, and it’s usually something controlled by your operations team, not development.

With this blue/green deployment methodology, we are placing the burden of risk mitigation on our system architecture to test different application versions. Imagine if you just wanted to test a small search bar update, would you want to go through an entire versioning process of duplicating environments and routing traffic? This method may be overly excessive for small changes, especially if you are practicing continuous delivery and releasing multiple times per week (or per day).

To get more refined release granularity, you can complement your blue/green deployment with [feature flags](http://blog.launchdarkly.com/feature-flag-driven-development/). These flags are conditionals (if/else statements) that compartmentalize code at the ‘feature level’, meaning you can control the display of particular features instead of relying on separate application versions.

![bluegreenff](https://featureflags.io/wp-content/uploads/2018/03/bluegreenfeatureflags.jpg "blue-green feature flags")

Using feature flags, you could still manage your traffic with a load balancer with the added benefit of gradually rolling out new features to your users. For example, you could switch from green to blue with the feature flag turned “off” in blue. Then, once traffic was flowing to blue, you can turn on the feature flag and gradually release the feature to 1%, 5%, 20%… of your users until you were satisfied with the performance and feedback.

Coupling feature flags with blue/green deployments could be best used with major application releases (like upgrading from version 1 to version 2 of a platform). However, for less substantial feature changes or gradual testing, you could utilize feature flags to manage feature releases within a single production environment. This will allow you to continuously release small features while still mitigating risk. It also allows you to release faster because you can practice continuous delivery while substantially reducing risk in the release phase.

#### [← Previous](./6%20-%20Flags%20vs%20Branching.md) | [Table of Contents](./README.md) | [Next →](8%20-%20Database%20Migrations.md)
