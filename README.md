# Welcome your Attini project

By exploring the contents of this project you can understand how to work with Attini.

Find more information about the attini-config [here](https://docs.attini.io/api-reference/attini-configuration.html "attini-config").

Find more information about the deployment plan [here](https://docs.attini.io/api-reference/deployment-plan.html "deployment plan").

Find more information about the Init deployment [here](https://docs.attini.io/architecture/init-deploy.html "init deployment").

---

## Deploy your first CloudFormation stack

1. Open deployment-plan.yaml

2. Navigate to Resources.DeploymentPlan.Properties.DeploymentPlan.States.Step1 and configure your [Stack](https://docs.attini.io/api-reference/deployment-plan-types.html#attini-deploy-deploymentplan-attinicfn "AttiniCfn").

3. Run `attini deploy run .`

---

## Useful commands

* On-broad/update the Attini framework with some useful default roles.

      attini setup --accept-license-agreement --create-deployment-plan-default-role --create-init-deploy-default-role

* See information about your current environment.

      attini context

* Register a dev environment with Attini.

      attini environment create dev

* Package and deploy your current directory to dev.

      attini deploy run . -e dev

* Package a distribution from your current directory.

      attini package .

* Deploy a distribution to a dev environment.

      attini deploy run attini_dist/attini-skeleton.zip -e dev