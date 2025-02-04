---
header-id: auto-deploy-to-all-nodes
---

# Auto Deploy to All Nodes

[TOC levels=1-4]

All modules and WAR files you deploy onto the cluster must be deployed to all
cluster nodes. Because @product@ 
[installs applications as OSGi bundles](/docs/7-2/frameworks/-/knowledge_base/f/using-the-wab-generator), 
you cannot rely on your application server's means of installing WAR files (even
if you only intend to install WAR files) to deploy an application to the entire
cluster. Instead, place the application in each node's auto deploy folder (e.g.,
`[Liferay Home]/deploy`). 

This, as you might imagine, can be done with a script. Write a shell script that
uploads applications to each node using sftp or some other service. This way,
when you deploy an application, it uploads to each node's auto deploy folder and
installs to @product@ on each node. 
