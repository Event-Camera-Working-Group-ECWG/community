# Event Camera Working Group

This document defines the scope and governance of the Working Group (WG).

**Mission:** The Event Camera Working Group's mission is to increase adoption of event camera sensors and their use cases in aerial robotic systems using the open source ROS 2 stack. The ECWG leverages embedded hardware such as the
AMD Kria KV260, AMD Kria KD240, NVIDIA Jetson Orin Nano series, NVIDIA Jetson Orin NX series, and Raspberry Pi 4/5 to test proof-of-concept software leveraging event camera sensors.


**Scope:** The ECWG scope software focuses on the ROS 2 stack, third-party ROS 2 packages, and the Prophesee Metavision SDK. The primary hardware focus is on widely available embedded arm64 boards to include the Jetson Nano Orin/Orin NX, AMD Kria KV260/KV240, and Raspberry Pi 4/5.

## Subprojects

This Working Group owns and maintains the following Subprojects.
Its meetings and membership are largely focused on the direction, design, and work on the projects.

### Subproject List

The following subprojects are owned by the Working Group:

*  **Establishing awareness and presence of the ECWG in the wider robotics community**
    * Description: Establish official OSRF ROS event Camera Working Group and documentation

* **Event Camera Driver for Nvidia Jetson Orin**
  * Description: Working on kernel module, DKMS, and the Nvidia camera core development library interface to get an event camera working on the Jetson Orin Nano/Orin NX via MIPI CSI interface
  * Repositories
    * [linux-sensor-drivers](https://github.com/TOTON95/linux-sensor-drivers-prophesee)

* **Metavision SDK Installer Package for AMD Kria development using Petalinux**
  * Description: Make the petalinux installer and Prophesee petalinux tools repos easier to install
  *  Respositories:
     * [metavision-sdk-installer](https://github.com/dirksavage88/metavision-sdk-installer)

*  **Metavision Embedded Markers Example Adapt to ROS 2**
   * Description: Adapt the existing pose markers example from Prophesee to a ROS 2 package
    * Repositories:
      * TODO

### Standards for subprojects

Subprojects must meet the following criteria (and the WG agrees to maintain them upon adoption).

* Build passes against ROS 2 master
* The ROS 2 standard linter set is enabled and adhered to
* If packages are part of nightly builds on the ROS build farm, there are no reported warnings or test failures
* Quality builds are green (address sanitizer, thread sanitizer, clang thread safety analysis)
* Test suite passes
* Code coverage is measured, and non-decreasing level is enforced in PRs
* Issues and pull requests receive prompt responses
* Releases go out regularly when bugfixes or new features are introduced
* The backlog is maintained, avoiding longstanding stale issues

### Adding new subprojects

To request introduction of a new subproject, add a list item to the "Subprojects" section and open a Pull Request to this repository, following the default Pull Request Template to populate the text of the PR.

PR will be merged on unanimous approval from Approvers.

### Subproject changes

Modify the relevant list item in the "Subprojects" section and open a Pull Request to this repository, following the default Pull Request Template to populate the text of the PR.

PR will be merged on unanimous approval from Approvers.

### Deprecating subprojects

Projects cease to be useful, or the WG can decide it is no longer in their interest to maintain.
We do not commit to maintaining every subproject in perpetuity.

To suggest removal of a subproject, remove the relevant list item in the "Subprojects" section and open a Pull Request in this repository, following instructions in the Pull Request Template to populate the text of the PR.

PR will be merged on unanimous approval from Approvers.

If the repositories of the subproject are under the WG's GitHub organization, they will be transferred out of the organization or deleted at this time.

## Governance

### Meetings

* Regular WG Meeting: bi-weekly on Wednesday, 0800 UTC
  * Meetings through Google Meet, coordinated via email
  * Artifacts updated will include meeting minutes, transcribing of the meeting.

### Communication Channels

Discord, Google Meet

### Backlog Management

{{Is any project management software/site used to track work for this Working Group? How can new members discover the highest impact tasks they could take on? GitHub Projects, ZenHub, etc.}}

### Membership, Roles and Organization Management

Working Group members may act in one or more of the following roles:

* **Member**
  * Prerequisite: Attend at least one out of the last three Working Group meetings
  * Responsible for triaging issues
* **Reviewer**
  * All reviewers are members
  * Prerequisite: Proven track record of high-quality reviews to WG Subprojects
  * Responsible for reviewing pull requests
* **Approver**
  * All approvers are reviewers
  * Prerequisite: Proven track record of high-quality contributions and reviews to WG Subprojects
  * Responsible for approving and merging pull requests
  * Responsible for vetting and accepting new projects into the Working Group
* **Lead**
  * TSC member or their delegate
  * Responsible for organizing and moderating working group meetings
  * Responsible for posting meeting materials (minutes, recordings, etc.)
  * Responsible for breaking ties

To become a member or change role, create an issue in this repository using the appropriate issue template.
Such applications are accepted upon unanimous agreement from Approvers, and are typically based on the applicant's history with the subprojects of the Working Group.
The Lead role cannot be applied for, as it is an appointee of the ROS 2 TSC.

### Modifying this governance document

Changes to this document will be made via Pull Request.
The PR will be merged on unanimous agreement from Approvers.
