Usage
=====

.. _installation:

Installation
------------

To use the Context-Aware Jenkins Job Transfers module, first install it using pip:

.. code-block:: console

   (.venv) $ pip install context-aware-jenkins-job-transfers

Supported Functionalities
-------------------------

1. **Connect to Jenkins Servers**

   To connect to the production and interim Jenkins servers, use the `connect` function:

   .. autofunction:: context_aware_jenkins_job_transfers.connect

   Parameters:
   - `production_machine_url`: URL of the production Jenkins server.
   - `interim_machine_url`: URL of the interim Jenkins server.
   - `production_username`: Username for the production server.
   - `interim_username`: Username for the interim server.
   - `production_password`: Password for the production server.
   - `interim_password`: Password for the interim server.
   - `mode`: Output mode, either `"console"` or `"quiet"`.

   Example usage:

   >>> from context_aware_jenkins_job_transfers import connect
   >>> connect("http://prod.example.com", "http://int.example.com", "prod_user", "int_user", "prod_pass", "int_pass")

2. **Transfer Jobs or Views**

   To transfer jobs or views from interim to production, use the `transfer` function:

   .. autofunction:: context_aware_jenkins_job_transfers.transfer

   Parameters:
   - `publish_list`: List of jobs or views to be transferred.
   - `ftype`: Type of transfer, either `"job"` or `"view"`.
   - `mode`: Output mode, either `"console"` or `"quiet"`.
   - `allowDuplicates`: Boolean to allow duplicate jobs.

   Example usage:

   >>> from context_aware_jenkins_job_transfers import transfer
   >>> transfer(["job1", "job2"], ftype="job", mode="console", allowDuplicates=True)

3. **Check Publish Standards**

   To verify if the jobs or views meet the publish standards, use the `check_publish_standards` function:

   .. autofunction:: context_aware_jenkins_job_transfers.check_publish_standards

   Parameters:
   - `publish_list`: List of jobs or views to check.
   - `ftype`: Type of check, either `"job"` or `"view"`.
   - `mode`: Output mode, either `"console"` or `"quiet"`.
   - `allowDuplicates`: Boolean to allow duplicate jobs.

   Example usage:

   >>> from context_aware_jenkins_job_transfers import check_publish_standards
   >>> check_publish_standards(["job1", "job2"], ftype="job", mode="console")

4. **Check Plugin Dependencies**

   To check plugin dependencies for jobs or views, use the `check_plugin_dependencies` function:

   .. autofunction:: context_aware_jenkins_job_transfers.check_plugin_dependencies

   Parameters:
   - `publish_list`: List of jobs or views to check.
   - `ftype`: Type of check, either `"job"` or `"view"`.
   - `mode`: Output mode, either `"console"` or `"quiet"`.

   Example usage:

   >>> from context_aware_jenkins_job_transfers import check_plugin_dependencies
   >>> check_plugin_dependencies(["job1", "view1"], ftype="view", mode="console")

5. **Check and Install Plugin Dependencies**

   To check and install missing plugin dependencies, use the `check_and_install_plugin_dependencies` function:

   .. autofunction:: context_aware_jenkins_job_transfers.check_and_install_plugin_dependencies

   Parameters:
   - `publish_list`: List of jobs or views to check and install dependencies for.
   - `ftype`: Type of check, either `"job"` or `"view"`.
   - `mode`: Output mode, either `"console"` or `"quiet"`.

   Example usage:

   >>> from context_aware_jenkins_job_transfers import check_and_install_plugin_dependencies
   >>> check_and_install_plugin_dependencies(["job1", "view1"], ftype="job", mode="console")

6. **Clean Up Production**

   To clean up the production Jenkins server, use the `production_cleanup` function:

   .. autofunction:: context_aware_jenkins_job_transfers.production_cleanup

   Parameters:
   - `mode`: Output mode, either `"console"` or `"quiet"`.

   Example usage:

   >>> from context_aware_jenkins_job_transfers import production_cleanup
   >>> production_cleanup(mode="console")

7. **Clean Up Interim**

   To clean up the interim Jenkins server, use the `interim_cleanup` function:

   .. autofunction:: context_aware_jenkins_job_transfers.interim_cleanup

   Parameters:
   - `mode`: Output mode, either `"console"` or `"quiet"`.

   Example usage:

   >>> from context_aware_jenkins_job_transfers import interim_cleanup
   >>> interim_cleanup(mode="console")

8. **Set Console Size**

   To set the width of the console output, use the `set_console_size` function:

   .. autofunction:: context_aware_jenkins_job_transfers.set_console_size

   Parameters:
   - `width`: Desired console width.

   Example usage:

   >>> from context_aware_jenkins_job_transfers import set_console_size
   >>> set_console_size(120)
