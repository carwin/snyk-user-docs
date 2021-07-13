# Nucleus Security

* [ Code Dx Enterprise](https://github.com/snyk/user-docs/tree/58f91d848e16ddf2ffcca3711d6b8852412be402/hc/en-us/articles/360018848798--Code-Dx-Enterprise/README.md)
* [ Brinqa](https://github.com/snyk/user-docs/tree/58f91d848e16ddf2ffcca3711d6b8852412be402/hc/en-us/articles/360012728717-Brinqa/README.md)
* [ Fortify SSC integration](https://github.com/snyk/user-docs/tree/58f91d848e16ddf2ffcca3711d6b8852412be402/hc/en-us/articles/360005507838-Fortify-SSC-integration/README.md)
* [ Kenna Security](https://github.com/snyk/user-docs/tree/58f91d848e16ddf2ffcca3711d6b8852412be402/hc/en-us/articles/360013620217-Kenna-Security/README.md)
* [ Nucleus Security](https://github.com/snyk/user-docs/tree/58f91d848e16ddf2ffcca3711d6b8852412be402/hc/en-us/articles/360012502818-Nucleus-Security/README.md)
* [ RiskSense](https://github.com/snyk/user-docs/tree/58f91d848e16ddf2ffcca3711d6b8852412be402/hc/en-us/articles/360015069418-RiskSense/README.md)
* [ Vulcan-Cyber](https://github.com/snyk/user-docs/tree/58f91d848e16ddf2ffcca3711d6b8852412be402/hc/en-us/articles/360012981478-Vulcan-Cyber/README.md)

## Nucleus Security

### Introduction to Snyk and Nucleus Integration

Nucleus allows you to import vulnerability data from a range of security scanning tools. It allows teams to sync vulnerability statuses, create rules, automate workflows, and report across all types of security.

With Snyk and Nucleus you can:

* Include vulnerability data from Snyk for both Snyk Open Source and Synk Container
* Create rules to trigger change management workflows when new Snyk data is ingested
* Report on data from Snyk alongside other tools, including penetration tests, cloud configuration audits, and infrastructure scans

### How it Works

Users can continue to use Snyk just as they do today. From the Nucleus console, set up a simple sync rule to automate the ingestion of the latest Snyk data into your Nucleus instance. Manage results alongside the rest of your vulnerability data without any changes to the normal scanning process.

To display the Snyk data in Nucleus:

1. Create a service account in snyk - [Service Accounts page](https://github.com/snyk/user-docs/tree/58f91d848e16ddf2ffcca3711d6b8852412be402/hc/en-us/articles/360004037597/README.md)
2. Copy the API key that is generated for the service account
3. Open up the Nucleus console and follow the [instructions](https://support.nucleussec.com/hc/en-us/articles/360016559492-Snyk) to set up the Snyk connector
4. Navigate in the Nucleus app to the “Import Via Connector” page and select which projects from Snyk to sync to Nucleus
