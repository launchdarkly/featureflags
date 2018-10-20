## Setting up your first feature flag

#### [← Previous](./2%20-%20Uses.md) | [Table of Contents](./README.md) | [Next →](4%20-%20Cleaning%20Up.md)

#### Early Access
While starting to feature flag is easy, it becomes increasingly more complicated as you scale and habitualize the practice as a team. So, why put the effort into maintaining a feature flagging process to begin with? Here are some quotes from feature flag proponents:

>"Feature flags are so so valuable. We use this for internal and private beta releases (we did with our recent launch of Podcasts) and plan to do this when we launch our new frontpage to start getting feedback from the community."  
>**Ryan Hoover, Founder of Product Hunt**

>"Feature flags and flippers mean we don’t have to do merges, and that all code (no matter how far it is from being released) is integrated as soon as it is committed. Deploys become smaller and more frequent; this leads to bugs that are easier to fix, since we can catch them earlier and the amount of changed code is minimized."  
>**Ross Harmes, Flickr**

>"By hosting the code that supports new functionality in the client application before we activate the feature, we greatly reduce the risk associated with the launch... Having this sort of dormant functionality also makes aborting launches easier when adverse effects are discovered during a rollout. In such cases, we can simply switch the feature off, iterate, and release an updated version of the app."  
>**Site Reliability Engineer: How Google Runs Production Systems**

>"We practice continuous deployment and make small changes frequently to the site. We use what we call "config flags," ...and a lot of the code for features runs “dark” for days or weeks, and feature launches mean flipping a switch in the code."  
>**Chad Dickerson, Etsy**

When it comes to creating your first feature flag, there are several options. Open source libraries are a great way to get started:

* AngularJS | [Angular Feature Flags](https://github.com/mjt01/angular-feature-flags) | by Michael Taranto
* EmberJS | [Feature Flags](https://guides.emberjs.com/v1.10.0/configuring-ember/feature-flags/) | by Ember
* .NET | [Feature Toggle](https://github.com/jason-roberts/FeatureToggle) | by Jason Roberts
* Java | [Togglz](http://www.togglz.org/) | by Christian Kaltepoth
* FF4J | [Feature Flipping](http://www.ff4j.org/) | by Cédrick Lunven
* PHP | [Feature Flags](https://github.com/etsy/feature) | by Etsy
* Python (Django) | [Waffle](https://github.com/jsocol/django-waffle) | by James Socol
* Python (Django) | [Gargoyle](https://github.com/disqus/gargoyle) | by Disqus

Feature flagging is a straightforward concept that becomes difficult to manage on an enterprise scale. It’s easy to manage one feature flag by modifying a configuration file, but when you have multiple feature flags across different environments, it’s harder to keep everyone in sync in a compliant fashion.

At this point you may consider if a feature flagging system is the right path for your company. So, you must ask yourself the question - to build or to buy? The tradeoffs for each option depend on your resources, time, and internal expertise. Here is more details on the inputs and outputs you can expect when [making the build versus buy decision](http://blog.launchdarkly.com/buying-vs-building-a-feature-flagging-system/).
