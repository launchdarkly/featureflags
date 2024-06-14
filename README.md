> [!CAUTION]
> This repository is archived. For up-to-date information on the topics covered here, visit [docs.launchdarkly.com](https://docs.launchdarkly.com/home).



### Table of Contents
1. [Introduction](https://github.com/launchdarkly/featureflags/blob/master/1%20-%20Introduction.md)
2. [Uses](https://github.com/launchdarkly/featureflags/blob/master/2%20-%20Uses.md)
3. [Getting Started](https://github.com/launchdarkly/featureflags/blob/master/3%20-%20Getting%20Started.md)
4. [Cleaning Up](https://github.com/launchdarkly/featureflags/blob/master/4%20-%20Cleaning%20Up.md)
5. [Best Practices](https://github.com/launchdarkly/featureflags/blob/master/5%20-%20Best%20Practices.md)
6. [Flags vs Branching](https://github.com/launchdarkly/featureflags/blob/master/6%20-%20Flags%20vs%20Branching.md)
7. [Blue-Green Deployments](https://github.com/launchdarkly/featureflags/blob/master/7%20-%20Blue-Green%20Deployments.md)
8. [Database Migrations](https://github.com/launchdarkly/featureflags/blob/master/8%20-%20Database%20Migrations.md)
9. [Implementation](https://github.com/launchdarkly/featureflags/blob/master/9%20-%20Implementation.md)

Welcome to the new home of our Feature Flagging Guide.

LaunchDarkly serves 4 billion feature flags daily to help software teams build better software, faster. LaunchDarkly gives you the power to separate feature rollout from code deployment and manage feature flags at scale. Ultimately, you can deliver faster, more personalized software with less risk.

## About LaunchDarkly

LaunchDarkly is a continuous delivery platform that provides feature flags as a service and allows developers to iterate quickly and safely. We allow you to easily flag your features and manage them from the LaunchDarkly dashboard. With LaunchDarkly, you can:

* Roll out a new feature to a subset of your users (like a group of users who opt-in to a beta tester group), gathering feedback and bug reports from real-world use cases.
* Gradually roll out a feature to an increasing percentage of users, and track the effect that the feature has on key metrics (for instance, how likely is a user to complete a purchase if they have feature A versus feature B?).
* Turn off a feature that you realize is causing performance problems in production, without needing to re-deploy, or even restart the application with a changed configuration file.
* Grant access to certain features based on user attributes, like payment plan (eg: users on the ‘gold’ plan get access to more features than users in the ‘silver’ plan). Disable parts of your application to facilitate maintenance, without taking everything offline.

LaunchDarkly provides feature flag SDKs for
* [Java](http://docs.launchdarkly.com/docs/java-sdk-reference)
* [JavaScript](http://docs.launchdarkly.com/docs/js-sdk-reference)
* [PHP](http://docs.launchdarkly.com/docs/php-sdk-reference)
* [Python](http://docs.launchdarkly.com/docs/python-sdk-reference)
* [Go](http://docs.launchdarkly.com/docs/go-sdk-reference)
* [Node.JS](http://docs.launchdarkly.com/docs/node-sdk-reference)
* [.NET](http://docs.launchdarkly.com/docs/dotnet-sdk-reference)
* [Ruby](http://docs.launchdarkly.com/docs/ruby-sdk-reference)
* [Python Twisted](http://docs.launchdarkly.com/docs/python-twisted-sdk-reference)
* [iOS](http://docs.launchdarkly.com/docs/ios-sdk-reference)
* [Android](http://docs.launchdarkly.com/docs/android-sdk-reference)

Many of the specific uses for LaunchDarkly’s features are covered within the [uses](https://github.com/launchdarkly/featureflags/blob/master/2%20-%20Uses.md) section of our guide, although we recommend you start with the [first chapter](https://github.com/launchdarkly/featureflags/blob/master/1%20-%20Introduction.md) for a comprehensive overview. For other questions, technical or otherwise, feel free to visit our site’s [FAQ](https://launchdarkly.com/faq.html) or our [support page](https://support.launchdarkly.com/)!

## Integrations
LaunchDarkly has numerous software integrations that are designed to make your experience smoother when using feature flags in combination with other products. These include:
* [Slack](http://docs.launchdarkly.com/docs/slack)
* [HipChat](http://docs.launchdarkly.com/docs/hipchat)
* [Webhooks](http://docs.launchdarkly.com/docs/webhooks)
* [Optimizely](http://docs.launchdarkly.com/docs/optimizely)
* [New Relic](http://docs.launchdarkly.com/docs/newrelic)
* [Visual Studio Team Services](http://docs.launchdarkly.com/docs/visual-studio-team-services-extension)
* [Bitbucket Pipelines](http://docs.launchdarkly.com/docs/bitbucket-pipelines)


## Community
Our community is open to anyone with interest in feature flagging or dark launching software! Feel free to head to any of the following links for more information, and a warm welcome into the world of dark launching.
* [Community Page](https://launchdarkly.com/community.html)
* [San Francisco Dark Launching Meetup](http://www.meetup.com/San-Francisco-Dark-Launching-Meetup/)
* Twitter: [@LaunchDarkly](https://twitter.com/LaunchDarkly)

## Known issues
For all known issues, visit the LaunchDarkly [support page](https://support.launchdarkly.com/) for help.

## Contributions
Our guide and SDKs are all open source, and we encourage pull-requests and other contributions from the community. If you have a suggestion or correction for our guide feel free to commit a pull request on this repo and it will be reviewed.

When contributing please ensure that you do the following:
 1. Read through our [Contributor’s Guide](http://docs.launchdarkly.com/docs/sdk-contributors-guide) before submitting any SDK pull requests.
 2. Create a new branch for each different change.
