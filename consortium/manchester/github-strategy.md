# Using GitHub
[TODO] I think this is good but maybe belongs in a policies and sops section? or best practice... Are we all going te enforce the same GH and SC policy? or maybe we get rid of this entirely?
## Creating repositories
Repositories are for discreet applications. Repository names should start with a project prefix and then the name of the application. Prefixes are:
| Prefix | Project Name |
|---|---|
| SDE-SKILLS- | Prefix for global projects or information for the SDE Skills Hub | 


Repository names should be all lower case with words divided by a dash for readability. E.g. sde-skills-dev-docs

## Naming files
[TODO] Do we need different standards for different programming languages?

## Branching Strategy
There are three stacks:

- **Production:** what is available to end user.
- **Staging:** for QA and testing purposes before deployment to production.
- **Development:** for development purposes.

The suggested branching strategy has the following workflow:

1. The code which is in production is in the "main" branch.
2. If the new feature (or fix) is required, the new branch is forked from "main" - the content of this branch is equivalent to the "development" stack.
3. When the developer is happy with the new feature (fix), a pull request (aka PR) is created. The content of this PR is equivalent to the "staging" stack.
4. Repositories should be configured to require review by at least one other person. The developer creating the PR should assign a reviewer.
5. The reviewer should check the code and either accept or reject the PR. The reviewer should include comments about their decision. A reviewer can comment for discussion with the developer without rejecting if needs any clarification

## Continuous Integration Best Practice
[TODO]