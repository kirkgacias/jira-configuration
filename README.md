![Jira-Service-Management-logo](https://github.com/kirkgacias/jira-configuration/assets/158519921/0194198d-10a4-4ee1-b66b-929dc902f07d)

<h1> Jira Service Management: Configuration, Workflows and Automation </h1>

<p> This project is designed to optimize IT support processes using Jira's powerful features. I will focus on the meticulous configuration of Jira settings, the creation of efficient workflows, and the implementation of smart automation rules. By customizing issue types, fields, screens, and automation rules, we establish a clear and efficient pathway for each ticket from the moment it is reported until it is resolved.</p>

</p>

<h2>Objectives</h2>

<h4> Streamline Ticket Management: </h4>

- Simplify the process of creating, tracking, and managing tickets through customized workflows and fields tailored to various types of IT support requests.

<h4> Automate Routine Tasks: </h4>

- Implement automation rules to handle repetitive tasks such as ticket assignments, status updates, and notifications.

<h4> Enhance Communication: </h4>

- Facilitate better communication within the support team and with end-users through automated notifications and updates.

</p>

<h2> Environments and Technologies Used </h2>

- Jira Service Management 
- Windows 11

<h2> Customizing Issue Types </h2>

<p>Jira allows you to customize the types of issues that can be created within your project. This is essential for categorizing the different kinds of requests and problems your help desk will handle.</p>

![Issue types](https://github.com/kirkgacias/jira-configuration/assets/158519921/867d729a-9b0c-488c-a4d5-d95091091b04)

<p><strong>.</strong></p>
<p><strong>.</strong></p>

<h3> Standard Issue Types for IT Help Desk: </h3>

<p><strong> 1. Bug Report </strong></p>

![Bug report](https://github.com/kirkgacias/jira-configuration/assets/158519921/5e1419e4-0594-49d5-aaf8-947b14586e37)

</p>
</p>

<p><strong> 2. Hardware Request </strong></p>


![Hardware Req](https://github.com/kirkgacias/jira-configuration/assets/158519921/7cc5adeb-3fab-47b4-a4cb-9fdae6a04270)


</p>
</p>

<p><strong> 3. Software Installation </strong></p>

![Software](https://github.com/kirkgacias/jira-configuration/assets/158519921/42dc09e8-3ffa-4c84-a843-7bb6df76925a)

</p>
</p>

<p><strong> 4. Network Issue  </strong></p>

![Network](https://github.com/kirkgacias/jira-configuration/assets/158519921/74d7ac7f-4dc7-4b96-9ec0-8e09a529912a)

</p>
</p>

<p><strong> 4. Access Request  </strong></p>

![access](https://github.com/kirkgacias/jira-configuration/assets/158519921/57f58605-06ab-43d7-8137-b8ef6563607e)

<br>

<h2> Defining a Workflow </h2>

<p> A workflow defines the lifecycle of an issue, from creation to resolution. Customizing the workflow allows you to mirror your organization's process for handling IT support requests.</p>

<img width="1003" alt="workflow" src="https://github.com/kirkgacias/jira-configuration/assets/158519921/30175a22-aac9-4e50-835b-6f925a36159c">

<p><strong>.</strong></p>
<p><strong>.</strong></p>

<h3>Standard Workflow Stages for IT Help Desk: </h3>

<img width="624" alt="diagram" src="https://github.com/kirkgacias/jira-configuration/assets/158519921/7287e9aa-b839-4f1f-aa6b-938d53065d2c">

<br>
<br>

<p><strong>Open:</strong> The initial status of a new issue.</p>
<p><strong>In Progress:</strong>The issue is being worked on by IT staff.</p>
<p><strong>Awaiting User:</strong> Waiting for more information or confirmation from the user.</p>
<p><strong>Resolved:</strong> The issue has been addressed, awaiting closure.</p>
<p><strong>Closed:</strong> The issue is fully resolved and closed.</p>

<br>

![diagram border](https://github.com/kirkgacias/jira-configuration/assets/158519921/508601c9-c371-4c27-84d7-ce58a088c6cb)

<p><strong>.</strong></p>
<p><strong>.</strong></p>
<p><strong>.</strong></p>

<h2>Custom Fields</h2>

<p>Custom fields allow you to capture specific information related to different issue types. </p>

![custom fields](https://github.com/kirkgacias/jira-configuration/assets/158519921/af1d3f3b-cf92-470f-b07b-8d9c5931905d)


<p><strong>Severity Level:</strong> Helps prioritize issues based on their impact on the business.</p>

<p><strong>Affected System:</strong> Identifies which system or application is impacted by the issue. </p>

<p><strong>Reported By:</strong> Captures whether the issue was reported by an employee, customer, or vendor. </p>
  
<p><strong>Expected Resolution Time:</strong> Provides an estimate of how long it will take to resolve the issue, which can be crucial for managing expectations.</p>

<p><strong>Root Cause Analysis:</strong> A text field for documenting the underlying cause of the issue once it has been identified. This is valuable for preventing future occurrences.</p>

<br>

<h2>Customizing Screens</h2>

<p>Screens in Jira determine which fields are displayed to users when they create, view, or edit an issue. Customizing these screens allows you to ensure that users are prompted for all relevant information when reporting an issue or moving it through its lifecycle.</p>


![Screens](https://github.com/kirkgacias/jira-configuration/assets/158519921/a9691806-e6e3-41bc-8b72-7c50cde30cd5)

<h2>Understanding Jira Automation</h2>

<p>Jira Automation is a powerful tool that allows you to create rules based on triggers, conditions, and actions. These rules can automate various aspects of your workflow, from issue assignment to notifications and field updates.</p>


<img width="1178" alt="Automation" src="https://github.com/kirkgacias/jira-configuration/assets/158519921/ef13fd36-8de7-44e8-a8c7-f7fba152a86e">

<p><strong>.</strong></p>
<p><strong>.</strong></p>

<h3>Key Concepts for Automation</h3>


<p><strong>Triggers:</strong> What initiates the automation rule. For example, creating an issue, updating an issue, or transitioning an issue could be triggers.</p>

<p><strong>Conditions:</strong>  Criteria that must be met for the automation rule to execute. 
Conditions help ensure that actions are taken only when relevant.</p>

<p><strong>Actions:</strong>  The operations performed when the trigger fires and the conditions are met. Actions can include updating an issue, sending an email, or transitioning an issue to a different status.</p>

<h3>Examples of Automation Rules for an IT Help Desk</h3>

<p><strong>Auto-Assigning Issues Based on Severity or Type</strong></p>

- Trigger: Issue created.
- Condition: Check the issue's severity or type (e.g., "Critical" severity or "Network Issue" type).
- Action: Assign the issue to a specific user or group responsible for that type of issue.

<img width="403" alt="Example 1" src="https://github.com/kirkgacias/jira-configuration/assets/158519921/3a1792b1-9bba-432b-9b3f-a8afa2f37bec">

<p><strong>.</strong></p>
<p><strong>.</strong></p>


<p><strong>Notifying Team Members of High-Severity Issues</strong></p>

- Trigger: Issue created with a "Critical" severity.
- Condition: Issue severity is set to "Critical."
- Action: Send an email notification to the Admins

<img width="624" alt="Example 2" src="https://github.com/kirkgacias/jira-configuration/assets/158519921/545e840c-c7ee-4cbc-9fc1-2597003b9213">

<p><strong>.</strong></p>
<p><strong>.</strong></p>

<p><strong>Automated Reminders for Pending Issues</strong></p>

- Trigger: Scheduled trigger (e.g., run daily).
- Condition: Check for issues in "In Progress" status for more than a specified time (e.g., 3 days).
- Action: Send a reminder to the assignee or post a comment on the issue.

<img width="624" alt="pending issues" src="https://github.com/kirkgacias/jira-configuration/assets/158519921/58321453-d43a-460a-b9e1-861fa8fdf4ac">


<h2> Conclusion</h2>

<p>The "Jira Service Management: Configuration, Workflows, and Automation" project showcases the various features of Jira that optimize IT service management processes. By carefully configuring Jira Service Management, designing efficient workflows, and implementing smart automation, organizations can significantly improve the speed, accuracy, and quality of their IT services.</p>


<h2>Future Directions</h2>

<p>In the following project, we will look at example scenarios and study the lifecycle of a ticket from creation to resolution. </p>

<h1>Thank you! &#127881; </h1>


