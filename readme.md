Dog Rules [Fees]
=======================

This is the DMN repository for the Dog Fees project.

The repository is a maven repository and is updated within the Rules engine. It's currently manually exported from dev to your local respository, and then pushed to both github (for record/backup) and production.
The first time a project is setup in production its best to import the project from a public github repository.

It is found within the Rules engine as `Regulations > Dogs`

To update this repository, clone it from the development rules engine like:

`git clone https://[host]:8080/business-central/git/Regulations/Dogs`

Where [host] is the domain of the development rules engine.

To then update a local repository from dev:
`git pull origin master`

You will then need to add a new remote for github if it doesn't already exist in your local version.

`git remote add wccorigin git@github.com:WellingtonCityCouncil/dog-rules.git`

Then push those changes to github.

`git push remote wccorigin`

For a new repository on production, make the project public on github and then click import project in workbench and use the https public git repository link. You can then choose to make the github repository private again.

For an already existing repository in production, add production as a remote and push updates to it as follows.

`git remote add production https://admin@[host]/business-central/git/Regulations/dog-rules`

`git push production master`

