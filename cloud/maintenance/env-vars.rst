.. _orocloud-maintenance-env-vars:

How to Add/Remove Environment Variables
=======================================

|Environment variable| can be configured for application usage, as illustrated below:

.. code-block:: none
    :linenos:

    ---
    orocloud_options:
      application:
        env_vars:
          'var1': 'value1'
          'var1': 'value2'
          'varN': 'valueN'

* **env_vars** — the hash where the key is an environment variable name, and the value is the environment variable value.

Environment Type Based Application Configuration
------------------------------------------------

.. code-block:: none
   :linenos:

    ---
    orocloud_options:
      application:
        env_vars:
          'ORO_DEPLOYMENT_TYPE': 'local'

* **local** - deployment_type, which will be set to parameters.yml for deployed application as

.. code-block:: none
   :linenos:

    deployment_type: local

.. include:: /include/include-links-cloud.rst
   :start-after: begin
