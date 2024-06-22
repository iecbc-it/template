# README
This is a repo template 👨🏼‍🔬  


## Description 🤝
Short. 
What was your motivation?  
What problem does it solve?  
What application does?
Why you used the technologies you used?



## Getting started 🚀 
Use [this tool](https://githubnext.com/projects/repo-visualization/) to explore the project if it is large

##  Development 🐙
- There are TODO comments in the code.
- Install git hooks. Run this command `git config core.hooksPath .githooks`.
- [Configure GPG keys if required](doc/GPG-KEYS.md)


### Branching strategy 🚨
This branching strategy will save you save you. 
- `number of environments == number of protected branches` e.g. for `prod`, `stg`, `dev` environments, you should have `prod`, `stg`, `dev` branches respectively.
    - Rename `master`/`main` branch to `prod`
- Do development on `dev` branch. Propagate changes from `dev` -> `stg` -> `prod` branches. CI/CD will deploy to respective environments upon merging. Merging is a deployment trigger.
- How to do development on the `dev` branch.
    - If you have a dev environment per a developer (temporary/disposable environments 😎), do a [Gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) on a `dev` branch. 
        - CI/CD should be configured that features branches are deployed to respective personal `dev` environments.
    - If the `dev` environment is shared for all developers, do a [Trunk Based Development](https://www.youtube.com/watch?v=v4Ijkq6Myfc) on a `dev` branch. Avoid further branching, bug if you do so, do not hold feature branches for long before merging them to `dev` branch.


#### Semantic Rleases
Releases must follow [semantic versioning](https://semver.org/lang/uk/)  
Follow [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) to bump the version. [READ THIS SUMMARY](https://www.conventionalcommits.org/en/v1.0.0/#summary)

- Following this convention, automation will create release and pre-release tags automatically.
- Following this convention, automation will generate `CHANGELOG.md`  automatically.
- [semver comparsion operators](https://github.com/Masterminds/semver)
- To trigger a new release without actually making any changes, run `git commit --allow-empty -m "fix: trigger release with empty commit" && git push`


### Building 🧱

### Deploying 🏋🏼


## Useful links 
- [.gitignore file generator](https://www.toptal.com/developers/gitignore/)
- [Markdown table generator](https://www.tablesgenerator.com/markdown_tables)
- [Kubernetes Manifests Generator](https://k8syaml.com/)
- [Generate banner online](https://manytools.org/hacker-tools/ascii-banner/)

Enjoy Coding ❤