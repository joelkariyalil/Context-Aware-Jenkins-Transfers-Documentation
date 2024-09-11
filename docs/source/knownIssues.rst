Known Issues
============

This page tracks known issues, defects, and enhancements for the **Context Aware Jenkins Job Transfers** module. If you encounter any other issues, feel free to report them via our GitHub repository.

.. contents:: Table of Contents
   :local:
   :depth: 1

Defects
-------

.. list-table:: Defects
   :header-rows: 1
   :widths: 20 50 15 15

   * - Defect ID
     - Description
     - Status
     - Workaround

   * - #D001
     - Views associated with jobs are not appearing on the target Jenkins server.
     - Fixed (v1.2.1)
     - Update to the latest version.

   * - #D002
     - Incorrect job configurations after transfer in some cases.
     - Investigating
     - Manually reconfigure affected jobs.

Issues
------

.. list-table:: Issues
   :header-rows: 1
   :widths: 20 50 15 15

   * - Issue ID
     - Description
     - Status
     - Workaround

   * - #IS001
     - Transfer fails when Jenkins Server is down.
     - Open
     - Ensure both servers are up and reachable.

   * - #IS002
     - Slow transfer speeds when transferring large jobs with numerous builds.
     - Open
     - Temporarily transfer jobs in smaller batches.

   * - #IS003
     - Error when trying to transfer a job with missing credentials.
     - Open
     - Ensure credentials are set up before transferring the job.

Enhancements
------------

.. list-table:: Enhancements
   :header-rows: 1
   :widths: 20 50 15 15

   * - Enhancement ID
     - Description
     - Status
     - Notes

   * - #EH001
     - Add support for parallel job transfers.
     - Open
     - Awaiting feedback.

   * - #EH002
     - Improve error logging for better troubleshooting.
     - Open
     - To be implemented in v1.3.0.

How to Report an Issue
----------------------

If you encounter an issue not listed here, please report it on our GitHub repository under the **Issues** section.

Thank you for your contributions in helping us improve this module!
