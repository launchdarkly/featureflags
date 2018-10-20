## Tips to reduce technical debt during implementation

#### [← Previous](./3%20-%20Getting%20Started.md) | [Table of Contents](./README.md) | [Next →](5%20-%20Best%20Practices.md)

#### Cleaning Code Patterns & Avoiding Technical Debt
Increased technical debt is a common objection to implementing feature flags. Here’s our suggested approach for avoiding crufty if/then branches you’ll have to clean up later.

#### Write the new feature
Step one is to write the new feature, gated by the feature flag, on a short-lived feature branch off of `master`(call it `pk/awesome-xyz-support`):

```python
...
if ldclient.toggle('temp-awesome-xyz', user, False):
    do_the_new_thing()
...
else:
    do_the_old_thing()
...
```

Next, before you submit your pull request for this change, create a second branch, off of the first, and call it `cleanup/awesome-xyz`. This branch removes the feature flag, leaving just the new code:

```python
...
do_the_new_thing()
...
```

#### Conventions
There are a couple of naming conventions used here:
* the feature flag is prefixed with `temp-`. This signals that it is meant to be a temporary flag, and is intended to be cleaned up at some point in the future. This is different from permanent flags, like ones relating to maintenance mode.
* The cleanup branch is named `cleanup/${FLAG_NAME}`. This signals that it is intended to clean up that flag. This will be useful if you are scanning the list of branches later on

#### Submit your pull requests
Submit the first pull request, with your feature branch targeting master. When it passes code review, merge and deploy as usual.

Next, submit the second pull request. Don’t merge it until you are satisfied that everything is good with the new code, but you can have your team review it while the other changes are in the front of everyone’s mind.

You can use the [flag status indicators](http://blog.launchdarkly.com/launched-flag-status-indicators/) to give you an indication when it is safe to merge the cleanup branch because all users are getting the new variation.

#### Why do it this way?
The advantage to managing cleanup this way is that you do the work to remove the flag when all of the context is fresh in your mind. At this point, you know all the pieces that get touched by the change, and it is easier to be sure you don’t forget something.

You will need to merge master back into your cleanup branch periodically, but that is usually easier than it would be to recall all of the context relating to the original change.

This is certainly not the only way to handle this issue, but it seems to work pretty well for our team. I’d love to hear how your team handles cleaning up feature flags!
