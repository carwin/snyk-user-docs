# Install the Snyk plugin on your Jenkins account

* [ Configure your Continuous Integration](https://support.snyk.io/hc/en-us/articles/360004002258-Configure-your-Continuous-Integration)
* [ Continuous Integration: language support](https://support.snyk.io/hc/en-us/articles/360004032157-Continuous-Integration-language-support)
* [ AWS CodePipeline integration](https://support.snyk.io/hc/en-us/articles/4402158184081-AWS-CodePipeline-integration)
* [ Azure Pipelines integration](https://support.snyk.io/hc/en-us/articles/360004127677-Azure-Pipelines-integration)
* [ Bitbucket Pipelines integration overview](https://support.snyk.io/hc/en-us/articles/360004032177-Bitbucket-Pipelines-integration-overview)
* [ CircleCI integration overview](https://support.snyk.io/hc/en-us/articles/360004002278-CircleCI-integration-overview)
* [ Configure your CircleCI integration](https://support.snyk.io/hc/en-us/articles/360004002298-Configure-your-CircleCI-integration)
* [ Getting Snyk Orb details from the CircleCI registry](https://support.snyk.io/hc/en-us/articles/360004032197-Getting-Snyk-Orb-details-from-the-CircleCI-registry)
* [ GitHub Actions integration](https://support.snyk.io/hc/en-us/articles/360019718618-GitHub-Actions-integration)
* [ Bitbucket Pipelines integration](https://support.snyk.io/hc/en-us/articles/360000921778-Bitbucket-Pipelines-integration)

 [See more](https://support.snyk.io/hc/en-us/sections/360001152577-CI-CD-integrations)

##  Install the Snyk plugin on your Jenkins account

The Snyk plugin for Jenkins is [maintained and documented](https://plugins.jenkins.io/snyk-security-scanner) from within Jenkins. Regardless of the kinds of projects you mostly manage from Jenkins \(freestyle or pipeline\), install the Snyk security task on your Jenkins account with these steps. Once complete, the plugin is available for configuration for any of your freestyle projects and pipelines.

### Note

Note: steps supported solely by Jenkins are in high-level only. See [Jenkins documentation](https://jenkins.io/doc/) for additional assistance.

#### How to install the Snyk plugin

1. Navigate to the Manage Jenkins=&gt;Manage Plugins area of Jenkins to install the Snyk Security plugin for Jenkins. See the [Jenkins documentation](https://jenkins.io/doc/) for additional information.

   ![image1.png](https://support.snyk.io/hc/article_attachments/360006275598/uuid-a1504227-4c48-ab40-d363-ab5dc74b1c71-en.png)

2. Navigate to Manage Jenkins=&gt;Global Tool Configuration and click Snyk installations ... to add a Snyk installation.

   ![image2.png](https://support.snyk.io/hc/article_attachments/360006212937/uuid-58fedef0-524e-ba88-e4f9-2ce8fd1b2430-en.png)

   ![image3.png](https://support.snyk.io/hc/article_attachments/360006275618/uuid-253d3b55-1301-e97c-636b-2c25b90089e2-en.png)

3. Enter a unique name.
4. Ensure Install automatically is selected.
5. This ensures your plugin automatically upgrades when there are newer versions available.
6. From the Install with snyk.io section enter values for these fields:
   * Install automatically—default is selected. This ensures your plugin automatically updates when available.
   * Version—the plugin version you would like to install; we recommend leaving the default latest to stay up-to-date with our Snyk CLI changes.
   * Update policy interval \(hours\)—this is a Jenkins parameter by which Jenkins checks the version of the installed plugin based on the value of this parameter and the frequency of your builds, updating the installation as necessary as part of the Snyk security task step if no other builds have triggered update checks already for that installation during that time interval. We recommend a policy of 24 hour intervals.
7. Save the changes.
8. From the Snyk app, retrieve your Snyk API token:
   * From your Snyk account, navigate to settings ![cog\_icon.png](https://support.snyk.io/hc/article_attachments/4402908592145/cog_icon.png) &gt; **General**.
   * If you are a member of an organization, copy the **Organization API** key; if yours is a personal account, then copy the **Personal access token**.
9. Return to your Jenkins account. From the **Credentials** area in Jenkins, enter your **Snyk API token** to enable Snyk to communicate with Jenkins, accessing your project, scanning and monitoring it.
10. Use these values:
    * Kind—Snyk API token
    * Scope—GlobalToken—Snyk API token as retrieved from your Snyk account
    * ID—Enter a name for the token
    * Description—optional free text

For more information about global credentials, see the [Jenkins documentation.](https://plugins.jenkins.io/snyk-security-scanner)
