# Toolchain for Poultry Sense Data Ingestor

This repository includes toolchain code to deploy a serverless data pipeline that uses Python and IBM Cloud Functions. The pipeline synchronizes data from Poultry Sense with IBM Food Trust. 

## Included toolchain components

* [Continuous Delivery](https://cloud.ibm.com/catalog/services/continuous-delivery): Enable tool integrations that support your development, deployment, and operation tasks.
* [GitHub](https://github.com/about): Store your source code in a new or existing repository on GitHub.com and engage in 
social coding through wikis, issue tracking, and pull requests
* [Eclipse Orion Web IDE](https://projects.eclipse.org/projects/ecd.orion): Develop for the web and the cloud in this browser-based integrated development environment (IDE)

## Steps

While you can use the individual actions locally, this collection of endpoints is meant to be deployed to IBM Cloud Functions. You can [deploy this application to IBM Cloud](#deploying-to-ibm-cloud) or [deploy it manually](#deploying-manually) by cloning this repo first.  

You can then review the [Actions](https://cloud.ibm.com/functions/actions) in the IBM Cloud console, along with your [Cloud Functions APIs](https://cloud.ibm.com/functions/apimanagement).

### Deploying to IBM Cloud

<p align="center">
    <a href="https://cloud.ibm.com/devops/setup/deploy?repository=https%3A%2F%2Fgithub.com%2Fsberajaw%2Fpoultrysense-bts-ingest-toolchain&branch=main">
    <img src="https://cloud.ibm.com/devops/graphics/create_toolchain_button.png" alt="Create toolchain">
    </a>
</p>

Click **Create toolchain** to deploy this same application to IBM Cloud. This option creates a deployment pipeline, complete with a hosted GitLab project and DevOps toolchain. [IBM Cloud DevOps](https://www.ibm.com/cloud/devops) services provides toolchains as a set of tool integrations that support development and deployment to IBM Cloud Functions. 

### Deploying manually 

To deploy this application to IBM Cloud using the command line, you can leverage the IBM Cloud Developer Tools.

* Install [IBM Cloud Developer Tools](https://cloud.ibm.com/docs/cli?topic=cloud-cli-getting-started) on your machine by running the following command:
  ```
  curl -sL https://ibm.biz/idt-installer | bash
  ```