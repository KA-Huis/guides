**Ticket title:** Upgrading dependencies YYYY-MM-DD

This ticket is part of our regular dependency upgrading policy. It follows the current template that can be found in
our [Guides website](https://ka-huis.github.io/guides/dependency-maintenance).

<!-- This template contains all dependency managers that are relevant to the organization. Remove any unnecessary one that do not apply for this repository or module. -->

## Outdated versions

### NPM

<!-- Run `npm outdated` and paste the results in a code block. Make sure it's properly formatted. -->

```text
Paste here the output.
```

<!-- Read the upgrade guides of the dependencies and list down any important notices here. -->

### Composer

<!-- Run `composer outdated` and paste the results in a code block. Make sure it's properly formatted. -->

```text
Paste here the output.
```

<!-- Read the upgrade guides of the dependencies and list down any important notices here. -->

## Proposed upgrades

<!-- Create an advice about which upgrades you think needs to be done. Patch and minor upgrades are usually fine, but major upgrades may not always be a good option. Since it's always different, you will have to propose which upgrades needs to be done. Substantiate your advice with good arguments and keep grammar and spelling in mind. -->

<!-- If you propose major upgrades then first discuss it with the main project contributors, before working on a pull request. --> 

## Pull requests

<!-- Here you can list down all pull requests that you have created for easy reference. Decide if the proposed upgrades needs to be done in multiple pull requests to keep it small and reviewable. No one likes to dig into a huge git diff and review it. The smaller it is the higher the chance it will be approved and merged. -->

<!-- Keep in mind that pull requests that changes the lock-file needs te be made after each other to prevent merge conflicts. Merge conflicts must not be fixed manually, but by the dependency manager in order to prevent corrupt hashes. -->

<!-- Follow the best practices defined in the guide ["Dependency maintenance"](https://ka-huis.github.io/guides/dependency-maintenance) to correctly apply upgrades. -->