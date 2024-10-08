Welcome to Context Aware Jenkins Job Transfers Documentation
=============================================================

**Context Aware Jenkins Job Transfers** provides a pythonic way of transferring jobs between two Jenkins Servers. It is essentially a Python wrapper for the Jenkins REST API, allowing users to transfer views (with jobs) or transfer jobs with its associated views and plugins, resulting in a **Context Aware Jenkins Job Transfer**.

Overview of Capabilities
------------------------

- **Transfer Job(s)**
- **Transfer View(s)**
- **Check for Plugin Dependencies** of Jobs/Views
- **Clean Up Jenkins Servers**
- **Visualize all functionalities** in a well-crafted terminal screen

For more details, check out the `Supported Functionalities <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html>`_ section, including information on how to install the project.

Contents
--------

- `Installation <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/installation.html>`_
- `Supported Functionalities <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html>`_
    - `Connect to Jenkins Servers <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html#connect-to-jenkins-servers>`_
    - `Transfer Jobs or Views <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html#transfer-jobs-or-views>`_
    - `Check Publish Standards <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html#check-publish-standards>`_
    - `Check Plugin Dependencies <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html#check-plugin-dependencies>`_
    - `Check and Install Plugin Dependencies <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html#check-and-install-plugin-dependencies>`_
    - `Clean Up Production <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html#clean-up-production>`_
    - `Clean Up Interim <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html#clean-up-interim>`_
    - `Set Console Size <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/usage.html#set-console-size>`_
- `Known Issues <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/knownIssues.html>`_
- `Change Log <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/changeLog.html>`_
- `Contributions <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/contribution.html>`_
- `Apache License <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/license.html>`_
- `FAQs <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/FAQs.html>`_
- `Contributors <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/contributors.html>`_
- `Contact the Author <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/contact.html>`_
- `Acknowledgements <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/acknowledgement.html>`_

Comparison with Other Jenkins Transfer Tools
--------------------------------------------

The current available methods of moving jobs among Jenkins servers are described `here <https://medium.com/@rajinikanthvadla9/jenkins-moving-from-one-server-to-another-server-methods-39437733b1e0>`_.

.. list-table::
   :header-rows: 1

   * - **Feature**
     - **Context Aware Jenkins Job Transfers**
     - **Other Jenkins Transfer Tools**
   * - **Job Transfer**
     - Seamless transfer of jobs between Jenkins servers with associated views and plugins.
     - Basic job transfer functionality; often lacks comprehensive job context.
   * - **View Transfer**
     - Transfers views (all jobs in views) in a single operation.
     - No support for transferring views.
   * - **Plugin Dependency Check**
     - Automatically checks for plugin dependencies and resolves them during the transfer.
     - No support for checking plugin dependencies.
   * - **Terminal Visualization**
     - Full visualization of transfer steps in the terminal for better user interaction.
     - Often lacks terminal-level feedback or logging.
   * - **Python Integration**
     - Written in Python for easy integration with other Python projects.
     - Often script-heavy or requires additional configuration files.
   * - **Scope for Workflows to be Built Pythonically**
     - Written in Python for easy integration with other Python projects.
     - Often script-heavy or requires additional configuration files.

Issue Tracking
--------------

Kindly check out the `Known Issues <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/knownIssues.html>`_ to keep track of known issues. If the issue is NOT found, kindly create a new ID at the `Issues <https://github.com/joelkariyalil/Jenkins-Transfers/issues>`_ page!

Contributors
------------

Check out the `List of Contributors <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/contributors.html>`_ who have helped build this project.

Contact the Author
------------------

Feel free to reach out via `Social Media Handles <https://context-aware-jenkins-transfers-documentation.readthedocs.io/en/latest/contact.html#social-media-handles>`_ for any questions or feedback.

Support the Author
------------------

Consider supporting the author through `Buy Me a Coffee <https://buymeacoffee.com/joelkariyalil>`_.
