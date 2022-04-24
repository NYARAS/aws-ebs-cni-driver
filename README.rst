eks-ebs-cni-driver-addons
===============

This config file create a cluster using a config file instead of flags.

It also adds Amazon EBS CSI driver addon.

The Amazon Elastic Block Store (Amazon EBS) Container Storage Interface (CSI) driver allows Amazon Elastic Kubernetes Service (Amazon EKS) clusters to manage the lifecycle of Amazon EBS volumes for persistent volumes.

How to use this config
----------------------
Prerequisites
~~~~~~~~~~~~~
Make sure you have imported an SSH key to your AWS account and you have access to that key.
In the config file replace `"<YOUR_KEY_NAME>"` with your key name.

Make sure you have the following libraries installed before beginning:

- composer (`Installing eksctl`_)
- git (`Configuring ssh`_)

Cloning from github
~~~~~~~~~~~~~~~~~~~
From your terminal go to the directory you want to clone the project into.

.. code:: bash

	$ cd path/to/your/directory

Clone the project.

.. code:: bash

	$ git@github.com:NYARAS/eks-ebs-cni-driver-addons.git

Creating the cluster
~~~~~~~~~~~~~~~~~~~~~
To create the cluster:

.. code:: bash

	(env)$ eksctl create cluster -f eks-cluster.yaml


Credits
--------
Developed by `Calvine Otieno`_ | developer@calvineotieno.com

.. _Configuring ssh: https://docs.gitlab.com/ee/ssh/
.. _Installing eksctl: https://docs.aws.amazon.com/eks/latest/userguide/eksctl.html

