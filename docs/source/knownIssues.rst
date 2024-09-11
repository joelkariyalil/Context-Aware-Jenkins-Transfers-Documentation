Known Issues
============

This page tracks known issues and their status for the **Context Aware Jenkins Job Transfers** module. If you encounter any other issues, feel free to report them via our GitHub repository.

.. list-table:: Known Issues
   :header-rows: 1
   :widths: 20 50 15 15

   * - Issue ID
     - Description
     - Status
     - Workaround

   * - #001
     - Transfer fails when Jenkins Server is down.
     - Open
     - Ensure that both servers are up and reachable.

   * - #002
     - Plugin dependencies are not transferred correctly in some cases.
     - Investigating
     - Manually verify plugin versions on both servers.

   * - #003
     - Views associated with jobs are not appearing on the target Jenkins server.
     - Fixed (v1.2.1)
     - Update the module to the latest version.

   * - #004
     - Slow transfer speeds when transferring large jobs with numerous builds.
     - Open
     - Temporarily transfer jobs in smaller batches.

   * - #005
     - Error when trying to transfer a job with missing credentials.
     - Open
     - Ensure credentials are set up correctly before transferring the job.

How to Report an Issue
----------------------

If you encounter an issue not listed here, please report it on our GitHub repository under the **Issues** section.

Thank you for your contributions in helping us improve this module!
