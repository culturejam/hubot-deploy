# hubot-deploy [![Build Status](https://travis-ci.org/culturejam/hubot-deploy.png?branch=master)](https://travis-ci.org/culturejam/hubot-deploy).

[GitHub Flow][1] via [hubot][3]. Chatting with hubot creates [deployments][2] on GitHub and dispatches [Deployment Events][4]. This is a customized fork.

![](https://f.cloud.github.com/assets/38/2331137/77036ef8-a444-11e3-97f6-68dab6975eeb.jpg)

There's a bunch of [ChatOps](https://github.com/atmos/hubot-deploy/blob/master/docs/chatops.md) commands.

## Forked Customizations
This is a customized fork of the [atmos/hubot-deploy](https://github.com/atmos/hubot-deploy)
upstream. Here's a list of customizations.

#### Personalized Github tokens are required
Each user must give Hubot their own personal Github token. This depends on the
[github-credentials][7] script in [hubot-scripts][6].

## Installation

* Add hubot-deploy to your `package.json` file.
* Add hubot-deploy to your `external-scripts.json` file.
* [Configure](https://github.com/atmos/hubot-deploy/blob/master/docs/configuration.md) your repos and providers for easy aliasing and custom options.
* Understand how the [GitHub API tokens are used](https://github.com/atmos/hubot-deploy/blob/master/docs/tokens.md).

## Runtime Environment

You need to set the following environmental variables.

| Environmental Variables |                                                 |
|-------------------------|-------------------------------------------------|
| HUBOT_GITHUB_TOKEN            |A [GitHub token](https://github.com/settings/applications#personal-access-tokens) with [repo:deployment](https://developer.github.com/v3/oauth/#scopes). The owner of this token creates [Deployments][5].

## See Also

* [hubot](https://github.com/github/hubot) - A chat robot with support for a lot of networks.
* [heaven](https://github.com/atmos/heaven) - Listens for Deployment events from GitHub and executes the deployment for you.
* [hubot-auto-deploy](https://github.com/atmos/hubot-auto-deploy) - Manage automated deployments on GitHub from chat.
* [github-credentials](https://github.com/github/hubot-scripts/blob/master/src/scripts/github-credentials.coffee) - Map your chat username to your GitHub username if they differ

[1]: https://guides.github.com/overviews/flow/
[2]: https://developer.github.com/v3/repos/deployments/
[3]: https://hubot.github.com
[4]: https://developer.github.com/v3/activity/events/types/#deploymentevent
[5]: https://developer.github.com/v3/repos/deployments/
[6]: https://github.com/github/hubot-scripts
[7]: https://github.com/github/hubot-scripts/blob/master/src/scripts/github-credentials.coffee
