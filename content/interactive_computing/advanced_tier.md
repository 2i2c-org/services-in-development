# 2i2c AdvancedTier

In 2i2c’s Advanced, 2i2c configures and deploys three JupyterHubs on behalf of a community making recommendations that are appropriate for many research and education scenarios. It assumes that there are multiple  ‘Community Representatives’ who are authorized to communicate with 2i2c on behalf of the community.  

*At various points in this procedure, there may be service details or feature options that 2i2c are able to provide but are not being offered within the Advanced Tier at this time. In those situations, Premium Tier are more appropriate for the community.*

2i2c requires a signed service agreement before deploying infrastructure on behalf of a community.

This process is started as soon as the Opportunity has been marked ‘Closed-Won’ and BD has signed off as ready for deployment. By signing off, BD is asserting



1. This agreement is fully signed and executed by all parties (the community, 2i2c, and CS&S)
2. The signed agreement is uploaded and available in the 2i2c AirTable
3. The metadata in Airtable for the opportunity is verified and consistent with the signed service agreement. In particular, the start date for the opportunity, the end date for the opportunity, the revenue expected from this agreement included estimated cloud costs and MAUs.  
4. CS&S has the required contact information to be able send out invoices.
5. At least one ‘Community Representative’ has been identified as the primary point of contact for the Product and Services Team to communicate with.  Name, GitHub id, and email address for this person must be in the AirTable contacts table.
6. A choice for the community identifier **&lt;community_id>**

The following community facing questions are critical to resolve before 2i2c is able to roll out infrastructure for a community:


    Q: What do you want to achieve by working with 2i2c? Can you paint me a picture that describes the future you wish to materialize?


    Q: Can you describe this research community more? Is it segmented? Are there archetypes or personas?


    Q: At a high level, what is your community trying to achieve and how open data/compute infrastructure will help advance toward your mission/vision?


    Q: Can you describe the data? Collaborating open science communities orbit around the heaviest objects in their science space -- their data. Where is it?

BD should request written answers to these questions before the service agreement is fully signed.

At the Advanced Tier, 2i2c is able to work with a community who wants to retain ownership of its billing account. 2i2c can also deploy infrastructure to AWS, GCP, Azure, or Jetstream2.  

Technical questions that need to be answered as part of the roll out process:



* What cloud infrastructure will be used?
* How is the cloud bill going to be paid?
* How will authentication for users work?
* How will access be provided to 2i2c engineers?

2i2c does require complete and full administrative access to the cloud infrastructure provider.  To be able to deploy the infrastructure, 2i2c needs to be able to manage its own access.

In particular, universities and colleges with institutional IT policies may not be available at the Advanced Tier.  If 2i2c has to apply for access for each engineer then the agreement should be structured as a Premium Tier instead.

*What if we need to use an institutional cloud account or system like NASA SMCE where 2i2c does not control access? Premium Tier.*

Upon hand-off from BD, a new Project is created with these components. The timeline is the relative to the date the contract is signed by the community. 

Advanced Tier Rollout



* Identify roll out coordinator within 2i2c ( &lt; 3 days)
* Schedule initial technical meeting ( &lt; 3 days)
* Initial technical meeting (30 mins) ( 1 week )
    * Align on technical requirements
    * Explain 2i2c infrastructure
    * Highlight Right-to-replicate
    * Choice of cloud provider and region
    * Discuss options on authentication
    * Discuss GitHub organizations and teams
    * Request account information and initial accounts
* Community research and preparation of slide deck (1-2 weeks)
* Email Community to schedule rollout meeting ( 1-2 weeks )
* Deploy the following infrastructure:
    * Kubernetes Cluster
    * Community Hub
    * Workshop Hub
    * Binder Hub
    * GitHub org for community and sub teams
    * JupyterBook companion site
    * Sample image environment configuration repo
    * Sample binder project repo
    * Quay account
* Rollout meeting with Community representatives (60 mins) ( &lt; 3 weeks )
    * Validate community expectations
    * Review 2i2c value proposition
    * Demo deployed infrastructure
        * Community Hub  (authenticated)
        * Workshop Hub (shared password or authenticated)
        * Binder Hub (open or authenticated)
        * JupyterBook companion site
        * Initial image to configure
    * Identify additional configuration requirements
        * Image management and creation
        * Domain name and landing page
        * Storage options including bucket storage
        * 
* Complete configuration requested during roll out
* Email community to invite them to onboard their users.
* Training and Onboarding sessions (ongoing)
    * Community Hub Champion Training
    * Intro to Grafana
    * Image management
    * User management
    * Right to replicate
    * Right to participate
    * 2i2c service level objectives
    * Events and workshops

The following introductory email is sent to the Technical Community Lead and cc’d to all Community Representatives. The purpose of this first meeting is to Align on the Technical Requirements to be able to deploy infrastructure.  


    Welcome to 2i2c’s Advanced Tier.  


    Our infrastructure team will schedule the deployment and rollout of a JupyterHub for your community.


    To kick-off this process, we request a technical meeting with your community to align on the infrastructure required for your community.

	

	{Use [cal.com](cal.com) to set up a meeting time?}


    The purpose of this meeting is to make some technical choices about how 2i2c should deploy infrastructure on your community’s behalf. 

	Here are the topics we need as an outcome of this technical meeting

	



    * Choice of cloud provider and region
    * Discuss options on authentication
    * Discuss GitHub organizations and teams
    * Request account information and initial accounts

    After this meeting, the 2i2c will begin its deployment process.


    Our team works on a two week iteration model. Our next iteration period is for &lt;date> to &lt;date> and we commit to having your hubs provisionally deployed by the end of that iteration.


    Once these hubs are available, 2i2c will invite all of your community representatives to a formal Rollout meeting where we will demo the infrastructure and align on next steps.


    Kind regards


    2i2c Product and Services Team



## Community research and slide deck

The purpose of this activity is to understand who this community is and how 2i2c expects to align with the community. The point is to state hypothesis on what 2i2c thinks is important to the community. These hypotheses will be validated in the roll out meeting.

Use these questions as a basis:

Q: What do you want to achieve by working with 2i2c? Can you paint me a picture that describes the future you wish to materialize?

Q: Can you describe this research community more? Is it segmented? Are there archetypes or personas?

Q: At a high level, what is your community trying to achieve and how open data/compute infrastructure will help advance toward your mission/vision?

Q: Can you describe the data? Collaborating open science communities orbit around the heaviest objects in their science space -- their data. Where is it?

Items to include



* Identify the people involved in the community
* Identify community website and any github repository
* Identify sample workflows or projects that the community is involved with
* Capture the technical requirements that were discussed in the Technical Alignment Meeting.
* Describe the platform components that are deployed
* List of remaining actions that 2i2c needs guidance to complete the rollout of Advanced Tier.

This document will be used in a rollout meeting and be a source of truth to align the 2i2c team’s knowledge about this community during the engagement.


## Email Community to schedule rollout meeting


    Dear Community Representatives,


    As part of the roll out of 2i2c Advanced Tier, we invite you attend a Roll out meeting to discuss the following:



    * Discuss community expectations
    * Demo deployed infrastructure
        * Community Hub
        * Workshop Hub
        * Binder Hub
        * JupyterBook
    * Refine configuration options

    { use [cal.com](cal.com)  to schedule meeting }


    Kind regards


    2i2c Product and Services Team



## Deploy the infrastructure

The initial deployment should be guided by what is known at this point about this community. It is important to have at least a functional deployment prior to the Roll out meeting.

Using the Infrastructure guide, use the PS engineering runbooks



* Kubernetes Cluster
* Community Hub
* Workshop Hub
* Binder Hub
* GitHub org for community and sub teams
* JupyterBook companion site
* Sample image environment configuration repo
* Sample binder project repo
* Quay account

2i2c chooses a single word to represent the name of this community in our infrastructure.  This one word will be used as an identifier for the project, billing, cluster, hub, and URL.  

&lt;**community_id>**

Set up billing accounts

2i2c deploys a Kubernetes cluster following the process documented in [https://infrastructure.2i2c.org/hub-deployment-guide/new-cluster/new-cluster/](https://infrastructure.2i2c.org/hub-deployment-guide/new-cluster/new-cluster/) . This step is covered by [https://infrastructure.2i2c.org/hub-deployment-guide/runbooks/phase2/](https://infrastructure.2i2c.org/hub-deployment-guide/runbooks/phase2/) where the following decisions are made on behalf of the community. 



* Region / Zone of the cluster: **AWS / GCP / Azure / Jetstream2**
* Name of cluster: ***&lt;community_id>***
* Is GPU required?: **Yes/No**

2i2c deploys a staging and production JupyterHub in this new cluster by following [https://infrastructure.2i2c.org/hub-deployment-guide/runbooks/phase3/initial-hub-setup/](https://infrastructure.2i2c.org/hub-deployment-guide/runbooks/phase3/initial-hub-setup/)

Choices made by 2i2c in consultation with the Community at the Advanced Tier



* Name of the hub:
* Will Dask gateway be required?: **Yes/No**
* Authentication mechanism: **Varied**
* Splash image: **2i2c Logo or url provided by the community**
* URL of the community’s webpage: None or url provided by the community.
* Funded by information (name and URL): If provided by community
* List of admin users: **Community Representatives**

Use jupyterhub-fancy-profiles and configure the following images



* JupyterDocker stacks scipy
* JupyterDocker stacks datascience
* Pangeo image
* Rocker RStudio

Bring your own image

Build your own image



* Dynamic image building

PS should make a best guess on an initial profile configuration for this community which can be validated during the Roll out.


## Rollout meeting with Community Representatives 

This should be 60 - 90 mins meeting between 2i2c and Community Representatives

Objectives of the meeting:



* Validate community expectations and priorities
    * Review 2i2c value proposition
    * Demo deployed infrastructure
        * Community Hub  (authenticated)
        * Workshop Hub (shared password or authenticated)
        * Binder Hub (open or authenticated)
        * JupyterBook companion site
        * Initial image to configure
    * Identify additional configuration requirements
        * Image management and creation
        * Domain name and landing page
        * Storage options including bucket storage

The Roll Out slide deck contains what 2i2c assumes to be important to this community. The meeting is an opportunity to validate those assumptions.


## Post rollout meeting follow up

Update the slide deck with information learned from the community.

Create GitHub issues to capture additional configuration required for the infrastructure


## Email community to invite them to onboard their users

Once the hub has been deployed, notify the Community Representatives with the following email:


    Your 2i2c JupyterHubs has been deployed at 


    https://&lt;community_id>.2i2c.cloud 


    https://workshop.&lt;community_id>.2i2c.cloud 


    https://binder.&lt;community_id>.2i2c.cloud 


    {replace with domain specific URLs if applicable}


    As a Community Representatives, the following accounts 



* Name 1, Email 1, GitHub 1
* Name 2, Email 2, GitHub 2

    have been configured as administrator accounts. Please verify that you are able to log in with your {authentication method for this hub} credentials.  If you are unable to log in, please send an email to [support@2i2c.org](mailto:support@2i2c.org) 


    Your hub has been pre-configured with a number of commonly used images


    Use jupyterhub-fancy-profiles and configure the following images

* JupyterDocker stacks scipy
* JupyterDocker stacks datascience
* Pangeo image
* Rocker RStudio

    Bring your own image


    Build your own image

* Dynamic image building

    See our [User environment and interface — Hub Service Guide](https://docs.2i2c.org/admin/howto/environment/) documentation for recommendations on creating and maintain your own images. At the Essential Tier, 2i2c is not able to provide direct technical support on images but we encourage you to post in [2i2c.discourse.org](2i2c.discourse.org) to share your configuration. It is likely there is another community that has encountered a similar issue that you can adapt for your community.


    As part of our Advanced Tier, 2i2c is able to work with your community up to 4 hours each quarter to provide additional technical guidance and support around image configuration.


    We have preconfigured the following profiles for for your users:


    { list profiles preconfigured}


    We can adjust how much RAM each user instance consumes. Please contact [support@2i2c.org](mailto:support@2i2c.org) if you need to change these values. We can also work with you to restrict certain subteams within your community to have access to particular profile types.


    As administrators, community representatives can log in to [https://grafana](https://grafana).&lt;communiy_id>.2i2c.cloud and observe the historical usage.  


    Cloud usage costs are the responsibility of the community and 2i2c will pass these costs on to you on a monthly basis.  We will alert you if your usage has increased more than 20% from the previous month to ensure you are staying within your intended cloud usage budget.


    File storage.  Each user has been assigned a quota on their home directories of 10GB.  Files storage incurs a cost even if no user instances are being started. Please periodically review Grafana homedirs table to see who is using space.  


    Shared files.  We have configured a special directory shared that is read only. The administrators have special access to shared_readwrite which allows files that need to be read by multiple users to be uploaded.  When doing computation in the cloud, please also consider object storage like S3 buckets as an alternative to block file storage. (Reference to …?)


    Best wishes to your community in using your 2i2c managed Hub. The 2i2c Product and Services infrastructure team can be reached at [support@2i2c.org](mailto:support@2i2c.org) for additional guidance and configuration requests which we will try to resolve within two business days. 


    For events or other high impact workshops please contact 2i2c at least 2 weeks in advance if additional configuration requirements are needed.


    2i2c will offer regular and recurring training to members of our networks. We will advertise these sessions as they are scheduled.


    You can also reach out to 2i2c communities on [https://2i2c.discourse.org](https://2i2c.discourse.org) to connect with our global network of research and learning communities.


    Kind regards,


    2i2c


Once deployed, this cluster and its hub come under the active management of 2i2c’s Product and Service Team. 2i2c is responsible for



* Upgrading the version of JupyterHub as released
* Upgrading the version of AWS EKS
* Deploying any security patches as needed
* Monitoring the usage and costs incurred by all clusters and communicating promptly with communities when costs have exceeded or are projected to exceed historical norms.

2i2c is not responsible for



* Direct support or training of the users of community hubs.
* The configuration of community-maintained images. 2i2c is able to provide limited support on the images maintained through the JupyterHub Docker Stacks project
* Creating or managing S3 storage although a community is welcome to create and use these assets under their own billing account.

Communities are encouraged to either provide direct access to their infrastructure or use nbgitpuller style links to share content with their users.

2i2c will check in with Advanced Tier communities quarterly to ensure the hub are meeting their needs. This will be delivered through the Community Enablement service framework. 


## At the end of an engagement

About 60 days before the end of an engagement, BD will contact the community to begin the process of renewal.  If a renewal is not agreed to, PS will begin an orderly decommissioning of the infrastructure:



1. Hub infrastructure and clusters are decommissioned within two weeks following the end of non-renewed engagement.
2. The community is notified 2 weeks prior to the end of the engagement, at the end of the engagement, and two weeks after the end of the engagement that the infrastructure is being removed.
3. Data is backed up to to low cost S3 storage bucket for 90 days to minimize data loss