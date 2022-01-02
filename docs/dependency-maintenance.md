---
layout: default title: Dependency maintenance
nav_order: 5
---

# Dependency maintenance

## Regular upgrading

In order to always rely on the latest versions of our dependencies with the latest security fixes, we should regularly
check for outdated versions and upgrade them. The advantage of regular upgrading is that the amount of changes needed to
upgrade will stay low most of the time, since most of the required steps are already done in a previous upgrade. This is
better than waiting for a long period of time and having to touch a lot of places in the code base. The bigger a pull
request gets, the harder it will be to determine the impact of the changes on the application.

### Dependabot

Dependabot is a feature from GitHub that can automatically check for outdated dependencies in repositories. Setting it
up is very simple and may take you ten minutes. See
the [documentation](https://docs.github.com/en/code-security/supply-chain-security/keeping-your-dependencies-updated-automatically/about-dependabot-version-updates)
for a more comprehensive explanation.

You can configure various things in the configuration-file to automate for example the assignee or labels. Make use of
these features to automate most of the tasks. See this example from
the [space-management](https://github.com/KA-Huis/space-management/blob/acceptance/.github/dependabot.yml) repository
for some inspiration.

### Template for upgrading

A template for the ticket (issue) has been created that must be used when upgrading. This template enforces a few
things:

* The version changes of dependencies will be documented, making them more traceable.
* The correct way of upgrading dependencies will be applied.
* Anyone can follow the process, since all the steps are written down.

The raw template can be
found [here](https://raw.githubusercontent.com/KA-Huis/guides/main/tools/dependency-upgrade-template.md) and can be
copied and pasted in the body of the GitHub-issue. The steps can then be followed.

### Composer best practices

To safely upgrade the dependencies, don't use the `composer upgrade` command. Carefully examine the changes in release notes or upgrade guide. Then apply an upgrade for the desired dependency.

In composer, you can run the following command to only update one or more dependencies:

```shell
composer update <depdendency name> --with-depdendencies
```


## Resources

* [4 Tips for Using Composer Efficiently](https://blog.martinhujer.cz/17-tips-for-using-composer-efficiently/) by [Martin Hujer](https://github.com/mhujer)