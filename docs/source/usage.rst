Supported Functionalities
-------------------------

Connect to Jenkins Servers
___________________

To connect to the production and interim Jenkins servers, use the `connect` function:

**Function Syntax:**

.. code-block:: console

    import jenkins_job_transfers as jt

    jt.connect(
        production_machine_url,
        interim_machine_url,
        production_username,
        interim_username,
        production_password,
        interim_password
    )

**Parameters:**

    - `production_machine_url`: URL of the production Jenkins server.
    - `interim_machine_url`: URL of the interim Jenkins server.
    - `production_username`: Username for the production server.
    - `interim_username`: Username for the interim server.
    - `production_password`: Password for the production server.
    - `interim_password`: Password for the interim server.
    - `mode`: Output mode, either “console” or “quiet”.

Example usage:

.. code-block:: console

    import jenkins_job_transfers as jt

    jt.connect(
        production_machine_url='http://127.0.0.1:8080',
        interim_machine_url='http://127.0.0.1:8081',
        production_username='production_username',
        interim_username='interim_username',
        production_password='production_password',
        interim_password='interim_password,
        mode='quiet'
        )


.. warning::

    Connecting both Jenkins servers at the beginning is necessary.

Transfer Jobs or Views

To transfer jobs or views from interim to production, use the `transfer` function:

Parameters:
    - `publish_list`: List of jobs or views to be transferred.
    - `ftype`: Type of transfer, either “job” or “view”.
    - `mode`: Output mode, either “console” or “quiet”.
    - `allowDuplicates`: Boolean to allow duplicate jobs.

**Example usage**:

from context_aware_jenkins_job_transfers import transfer

transfer(
    ["job1", "job2"], 
    ftype="job", 
    mode="console", 
    allowDuplicates=True
)

Check Publish Standards

To verify if the jobs or views meet the publish standards, use the `check_publish_standards` function:

Parameters:
- `publish_list`: List of jobs or views to check.
- `ftype`: Type of check, either “job” or “view”.
- `mode`: Output mode, either “console” or “quiet”.
- `allowDuplicates`: Boolean to allow duplicate jobs.

Example usage:

from context_aware_jenkins_job_transfers import check_publish_standards

check_publish_standards(
    ["job1", "job2"], 
    ftype="job", 
    mode="console"
)

Check Plugin Dependencies

To check plugin dependencies for jobs or views, use the `check_plugin_dependencies` function:

Parameters:
- `publish_list`: List of jobs or views to check.
- `ftype`: Type of check, either “job” or “view”.
- `mode`: Output mode, either “console” or “quiet”.

Example usage:

from context_aware_jenkins_job_transfers import check_plugin_dependencies

check_plugin_dependencies(
    ["job1", "view1"], 
    ftype="view", 
    mode="console"
)

Check and Install Plugin Dependencies

To check and install missing plugin dependencies, use the `check_and_install_plugin_dependencies` function:

Parameters:
- `publish_list`: List of jobs or views to check and install dependencies for.
- `ftype`: Type of check, either “job” or “view”.
- `mode`: Output mode, either “console” or “quiet”.

Example usage:

from context_aware_jenkins_job_transfers import check_and_install_plugin_dependencies

check_and_install_plugin_dependencies(
    ["job1", "view1"], 
    ftype="job", 
    mode="console"
)

Clean Up Production

To clean up the production Jenkins server, use the `production_cleanup` function:

Parameters:
- `mode`: Output mode, either “console” or “quiet”.

Example usage:

from context_aware_jenkins_job_transfers import production_cleanup

production_cleanup(mode="console")

Clean Up Interim

To clean up the interim Jenkins server, use the `interim_cleanup` function:

Parameters:
- `mode`: Output mode, either “console” or “quiet”.

Example usage:

from context_aware_jenkins_job_transfers import interim_cleanup

interim_cleanup(mode="console")

Set Console Size

To set the width of the console output, use the `set_console_size` function:

Parameters:
- `width`: Desired console width.

Example usage:

from context_aware_jenkins_job_transfers import set_console_size

set_console_size(120)