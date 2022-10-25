# Github Action Templates

Regroup all github actions templates use within the demarque organisation

# Project not compatible with templates

1. MARKET_ELASTICSEARCH

# Update github action templates

## Test changes in actions before switching

1. Create a new branch from staging
1. Add changes in template
1. Choose an action from which you will run the test
1. Change tag name/version (ex. gh-workflow-templates-v2) in this action for the new branch name
1. Run the action in github to see if everything is ok (You can force an action to run by simply replacing to 'on: push' at the top)
1. Once test succeeded you can procede to upgrade the template

## Upgrade the template

1. Checkout master branch
1. Change code in the template file.
1. Create a pull request with thoses changes (Make sure to add a description in the PR)
1. Post your new PR in #ops slack channel
1. Wait for the PR to be merge
1. Create a new release/tag from master and upgrade the version
1. Procede to bump version in actions

## Bump template version in actions

1. Create a new PR that will upgrade the actions to the new template version (Change all gh-workflow-templates-v2)
1. Make sure every actions succeeded in github
