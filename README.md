# Serverless Data Pipeline: Poultry Sense -> IBM Food Trust Data Ingestor

This repository includes toolchain code to deploy a serverless application that uses Python and IBM Cloud Functions.

## Included toolchain components

* [Continuous Delivery](https://cloud.ibm.com/catalog/services/continuous-delivery): Enable tool integrations that support your development, deployment, and operation tasks.
* [GitHub](https://github.com/about): Store your source code in a new or existing repository on GitHub.com and engage in 
social coding through wikis, issue tracking, and pull requests

## Steps

While you can use the individual actions locally, this collection of endpoints is meant to be deployed to IBM Cloud Functions. You can [deploy this application to IBM Cloud](#deploying-to-ibm-cloud) or [deploy it manually](#deploying-manually) by cloning this repo first.  

You can then review the [Actions](https://cloud.ibm.com/functions/actions) in the IBM Cloud console, along with your [Cloud Functions APIs](https://cloud.ibm.com/functions/apimanagement).
<table>
  <thead>
      <tr>
        <th>Method</th>
        <th>HTTP request</th>
        <th>Description</th>
      </tr>
  </thead>
  <tbody>
    <tr>
      <td>Create</td>
      <td>POST /database</td>
      <td>Inserts an object</td>
    </tr>
    <tr>
      <td>Read</td>
      <td>GET /database/<font color="#ec407a">objectId</font></td>
      <td>Retrieves an object</td>
    </tr>
    <tr>
      <td>ReadAll</td>
      <td>GET /database</td>
      <td>Retrieves all objects</td>
    </tr>
    <tr>
      <td>Delete </td>
      <td>DELETE /database/<font color="#ec407a">objectId</font></td>
      <td>Deletes an object</td>
    </tr>
    <tr>
      <td>DeleteAll</td>
      <td>DELETE /database</td>
      <td>Deletes all objects</td>
    </tr>
    <tr>
      <td>Update</td>
      <td>PUT /database/<font color="#ec407a">objectId</font></td>
      <td>Updates content of an object</td>
    </tr>
  </tbody>
</table>

### Deploying to IBM Cloud

<p align="center">
    <a href="https://cloud.ibm.com/devops/setup/deploy?repository=https%3A%2F%2Fgithub.com%2Fsberajaw%2Fpoultrysense-bts-ingest&branch=master">
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

## Next steps
* Learn more about augmenting your Node.js applications on IBM Cloud with the [Node.js Programming Guide](https://cloud.ibm.com/docs/node?topic=nodejs-getting-started).
* Explore other [sample applications](https://cloud.ibm.com/developer/appservice/starter-kits) on IBM Cloud.

## License

[Apache 2.0](LICENSE)