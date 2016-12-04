## Recommended uses and how they help.
#### Early Access
Run beta programs on your live application by explicitly including the people you want to see a new feature. Like lining up for a new movie coming out, people really want to see your new functionality. Whether it’s a person or organization or even country. It’s a common best practice to roll out to Canada before the United States or to New Zealand before Australia.

#### Kill Switch
A well-wrapped feature means you can quickly turn it off if it’s performing poorly. This can be the difference between a public relations disaster and minimal impact. When you combine this with percentage rollouts, it’s even more powerful. You can rollout to say 1% of your users and get feedback. If something goes wrong you’ve disrupted the smallest possible audience. If you’re doing this right, you can essentially take risk off the table.

#### Opt In
You can allow users to opt-in for early access to new features. There’s essentially a contract between you and the early user. The user gets something new and cool and in return you expect them to be more tolerant of the feature early stage in development. Google Labs is a great example.

#### Incremental Roll Outs
Do phased rollouts to percentages of your users to verify there are no scalability issues. You can roll out to a random percentage of users to verify to get feedback. This is particularly good for infrastructure projects. If you’re bringing on a new back-end and want to make sure it can handle load in the real world. No more crossing your fingers and hoping - you can ramp up and verify. Instead of releasing the new functionality at 4 am in case it didn’t work well, you can do this during normal business hours. Ramp up to 2% at 9 am to ensure it’s all working properly and keep ramping up during the day. You can even turn it completely off to leave for lunch when you aren’t around to monitor it.

#### Block Users
While a feature flag can enable a specific user or user group to access some element of your site, there is also the capability to protect features from users by excluding them from ever seeing them. One example would be regulations that differ by state or by country. This is applicable to liquor companies or drug companies that have different laws across state or country lines so will want to serve up different experiences in those different geographical areas. Sometimes it’s someone in your own organization who you don’t want to see a certain feature until it’s more baked. This is sometimes called “the CEO rule”. You may also want to block an IP or anyone in a certain domain. It is also common practice to exclude anyone from TechCrunch from seeing new functionality so a new feature won’t be scooped or seen prematurely.

#### Hypothesis Driven Development
Feature flags help you Run A/B tests of features to see which features perform better. If you’re switching you can get measurements and KPIs to see if this change supports your hypothesis.

#### Calendar Driven Launches
Whether you have a big PR splash, a re-branding, or an external event like “Black Friday”, calendar driven launches can be very stressful. You have to flip on many assets and functionality at the same time, and see it the same time as your end users. No matter how often you test in staging, the real world is the final judge. However, with feature flags, you can push all of your functionality “live” to production - but turned off for everyone but your QA and internal testers. This gives you an opportunity and time to flush out any issues, well before your actual launch.

#### Subscription
It’s often more simple and certainly more scalable to control subscription plans by bundling features with feature flags. We at LaunchDarkly for instance have three different subscription plans, and there are different features for each. If you have an interface that allows people on the admin side to access, then they can easily handle changes to visibility. For instance, a product or sales person can give access to a big customer who would like to check out a feature from the next level of subscription. And then once the customer is happy with it, move them on up. The old way involves an engineer and days of work.

#### Newbie vs Power User
It’s likely that you want to show expert users and beginner users different features of your product entirely. For instance, a new and a “power” user have different needs from your product. You want to make them both happy. Without a compromise, you can give two different experiences. Feature flags make it easier to tailor your application to your user base.

#### Maintenance Mode
Put portions (or your entire application) into maintenance mode. Read more here about how LaunchDarkly handles whole-site maintenance, whole-feature maintenance and per-feature maintenance modes.

#### Sunset
All features eventually go to the bit bucket in the sky. If your system has been around for a while, you start to accumulate old features. And there’s a hidden costs to this. It’s expensive to have around hidden features, as you have to QA and make sure they aren’t conflicting with new features, Have to make sure these old features work on new platforms. Old features are a huge hidden tax on software releases. Sometimes the best things to do with old features is to cleanly sunset them.
