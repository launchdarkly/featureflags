## An introduction to feature flagging software.
Feature flags give a software organization the power to reduce risk, iterate quicker, and gain more control. Feature flags allow you to decouple feature rollout from code deployment. This separation allows you unprecedented control of who sees what when, independent of release. And the “you” can be anyone in your organization - from developers, ops, designers, product managers, or marketers. Allowing control over a release unlocks the true power of your software.

This guide will show you how you can start using feature flags in your organization. We’ll give step by step instructions on how feature flags fit into your process. We’ll cover how feature flags can be combined with blue/green deployments and branching. Even if you’re already using feature flags, we discuss advanced use cases like database migration that you might find valuable.

Feature flagging is a method by which developers wrap a new feature in an if/then statement to gain more control over its release. By wrapping a feature with a flag, it’s possible to isolate its effect on the system and to turn that flag on or off independent from a deployment. This effectively separates feature rollout from code deployment. Feature flagging is a core component of continuous delivery that empowers software organizations to release quickly and reliably.

![Anatomy](https://featureflags.io/wp-content/uploads/2018/03/anatomy.jpg "Feature Flag Anatomy")

Martin Fowler, Jez Humble, and Facebook’s Engineering team are widely credited with introducing the concept of feature flagging (also called feature toggling or feature switching). Within the context of continuous delivery, feature flags provided the foundation for a framework that would allow developers to release software faster and with less risk and more control.

![Flags or Toggles](http://featureflags.io/wp-content/uploads/2018/03/flags-or-toggles.jpg "Feature Flags or Toggles")

Here are some companies who actively practice feature flag-driven development:
* [Apiary](https://launchdarkly.com/casestudies/apiary.html)
* [AppDirect](https://launchdarkly.com/casestudies/appdirect.html)
* [Behalf](https://launchdarkly.com/casestudies/behalf.html)
* [CircleCI](https://launchdarkly.com/casestudies/circleci.html)
* [Domain](http://tech.domain.com.au/2015/05/feature-flagging-framework/)
* [Etsy](https://www.infoq.com/news/2014/03/etsy-deploy-50-times-a-day)
* [Facebook](https://www.facebook.com/notes/1000330413333156/)
* [Flickr](https://bit.ly/dZZzfY)
* [Instagram](https://www.infoq.com/news/2016/04/continuous-deployment-instagram)
* LinkedIn
* [Upserve](https://launchdarkly.com/casestudies/upserve.html)
* Yammer
