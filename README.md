<h1 align="center">Insiders <a href="https://twitter.com/intent/tweet?text=Insiders%20-%20Archive%20of%20Potential%20Insider%20Threats%20https://github.com/trickest/insiders%20&hashtags=security,bugbounty,bugbountytips,assets,infosec,cybersecurity,recon,reconnaissance"><img src="https://img.shields.io/badge/Tweet--lightgrey?logo=twitter&style=social" alt="Tweet" height="20"/></a></h1>
<h3 align="center">Archive of Potential Insider Threats</h3>
Company employees' accounts, especially online git repositories, can leak sensitive data. We have found that they are even more likely to expose secrets than official brand accounts. This project aims to create a comprehensive archive of public code repositories belonging to the employees of companies that have bug bounty programs.

### Directory Structure
```
├── targets
│   ├── Target
│   │   ├── github-users.txt                     # User accounts collected from multiple sources
│   │   ├── github-repos.txt                     # GitHub repositories owned by the collected users
│   │   ├── github-repos-shell.txt               # GitHub repositories that use `Shell` as a primary language - according to our statistics, these are the most likely to expose secrets
│   │   ├── github-raw.json                      # JSON file containing all users/repos data
│   │   └── README.md                            # Markdown file containing multiple statistics describing the collected data
```

## How it works
A [Trickest](https://trickest.com) workflow collects a list of targets, enumerates their employees, collects their data, cleans it up, and pushes it to this repository.

![Trickest Workflow - Hostnames](insiders.png "Trickest Workflow - Inventory")
### TB; DZ (Too big; didn't zoom)
- Get the initial list of target names from [Project Discovery's Chaos dataset](https://chaos.projectdiscovery.io/) (Thanks, [ProjectDiscovery](https://github.com/projectdiscovery))
- Use a slightly modified version of [CrossLinked](https://github.com/m8r0wn/CrossLinked) to collect employee names and usernames from LinkedIn(Thanks, [m8r0wn](https://github.com/m8r0wn))
- Generate username permutations based on the collected names/usernames.
- Enumerate public GitHub organization members using the [GitHub CLI](https://cli.github.com/) (Thanks, GitHub?)
- Merge the collected potential usernames and pass them to our own [enumerepo](https://github.com/trickest/enumerepo) (Public release soon!) which validates the usernames and enumerates their public repositories.
- All of the collected orgs/usernames/repos/gists are then passed to [TruffleHog](https://github.com/trufflesecurity/trufflehog) to find exposed secrets/credentials (Thanks [Truffle Security](https://github.com/trufflesecurity)!) as highlighted above in the `Secrets` workflow. Note that the results of this part are not pushed to this repository for obvious reasons. They are only accessible to our users who can edit/customize this workflow to view the secrets, receive notifications about new ones, or export them using one of our integrations.
- In the end, we parse and organize the collected data and push it here (except for the `Secrets` part.)
- We have the workflow scheduled to run regularly to keep the data up-to-date at all times.

## Contribution
All contributions/ideas/suggestions are welcome! If you want to add/edit a target/workflow, feel free to create a new ticket via [GitHub issues](https://github.com/trickest/inventory/issues), tweet at us [@trick3st](https://twitter.com/trick3st), or join the conversation on [Discord](https://discord.gg/7HZmFYTGcQ).

## Build your own workflows!
We believe in the value of tinkering. Sign up for a demo on [trickest.com](https://trickest.com) to customize this workflow to your use case, get access to many more workflows, or build your own from scratch!
