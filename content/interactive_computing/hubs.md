# Interactive Computing Hubs

As part of our Managed Iteractive Computing service we design, deploy, and mantain JupyterHub instances ("Hubs") on behalf our commuities.

JupyterHub is project of Jupyter.  2i2c deploys configurations of JupyterHubs on cloud infrastracture for research and education communities.  JupyterHub is flexible and can support many different use cases. 2i2c has identified the following hub types which are useful configurations for most of the communities we serve.


Right to Replicate.

## 2i2c Community Hub


## 2i2c Workshop Hub

A workshop hub is used short period, event style workshops where the data needs to persist only for the duration of the workshop event (could be multi-day).  As well, the users on a workshop hub are not permanent, ongoing members of the community. Their identities on a workshop hub only need to persist for the duration of the workshop.

The advantage of a workshop hub, is that distinguishes between the home directories of persistent JupyterHub where I, as workshop participant, may have separate projects created before the workshop or completely independent from the workshop.  It allows communities representatives to delete data on a workshop hub with additional degree of safety because the contents of the files on a home directory on a workshop hub only have meaning during the workshop or in the immediate days afterwards.  A community can reset a workshop hub back to clean state without needing to sort between users who were invited to participate in a workshop style event and users who are long time, on going users of a community hub.
A workshop home is not ephemeral because files may need to persist between separate sessions of a workshop.

A community would periodically request that the data and the accounts on the the workshop hub be removed entirely.

Depending on the community, it may or may not have the same profile or authentication method the community hub. The distinguishing feature is how long the data is intended to persist on the workshop hub.

## 2i2c Binder Hub



## Other hub types

2i2c is also able to design and maintain other hub configurations but the configuration listed above are most commonly used by our communities.

