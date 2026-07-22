# Copilot instructions for NetApp Volume Caching documentation

## Repository overview

**Product:** NetApp Volume Caching 

NetApp Volume Caching is a NetApp Console service for creating remote cache volumes from ONTAP source volumes. The documentation in this repo focuses on how volume caching reduces WAN latency, improves access to read-intensive data, and supports cache relationships across Amazon FSx for NetApp ONTAP, Cloud Volumes ONTAP, and on-premises ONTAP environments.

## Repository structure

* `_include` - Reusable text blocks referenced in .adoc files in the root. 
* `media` - Images and diagrams that are elements of articles in the root directory. This includes .png and source files. 
* `_whatsnew` - Release notes in .adoc form that are aggregated in the whats-new.adoc file.
* `redirect` - .adoc files for retired pages and endpoints that redirect HTTPS requests to the appropriate endpoint.
* `support` - Support-related documentation pages including help and support registration tasks.
* `get-started` - Introductory content for learning about Volume Caching, reviewing prerequisites, setting up the service, accessing it in NetApp Console, and answering common questions.
* `use` - Task content for creating caches, managing cache settings, and monitoring jobs.
* `release-notes` - End-user release notes content, including what's new and known limitations.

## Product-specific context

* *NetApp Console* - The management interface through which users access Volume Caching and other NetApp data services. In this repo, users navigate in the Console to *Mobility* > *Volume caching*.
* *Console agent* - The NetApp Console component that provides connectivity between the Console and storage systems or NetApp data services. The docs treat agent setup as a prerequisite for using Volume Caching.
* *Cache volume* - The target volume created by the service. It is sparsely populated, retains hot or recently used data, and can be on the same cluster as or a different cluster than the source volume.
* *Source volume* - The original ONTAP volume whose data is cached. The cache serves client reads locally when data is already present and otherwise fetches data from the source.
* *Working environment* - The representation of a storage system in NetApp Console. The docs call out Amazon FSx for NetApp ONTAP, Cloud Volumes ONTAP, and on-premises ONTAP as supported working environments.
* *Cache access* - The option to replicate NFS export policy rules and SMB/CIFS share configuration from the source volume to the cache volume during cache creation.
* *Audit page* - The NetApp Console administration view used to monitor the progress of Volume Caching operations.


## Typical user workflows

* *Set up Volume Caching* - review prerequisites, creating a Console agent, and preparing supported source and target systems in NetApp Console. Access the service in NetApp Console and create a cache by selecting source and target environments, choosing eligible volumes, and defining cache settings.
* *Manage existing caches* - review cache details, editing settings, changing export policies, resizing caches, or deleting caches.
* *Monitor operations and ongoing product changes* - check the Console Audit page, release notes, limitations, and support content.
