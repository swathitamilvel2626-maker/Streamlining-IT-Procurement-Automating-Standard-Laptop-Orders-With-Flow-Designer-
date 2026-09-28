#Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

Project Overview

This project automates the standard laptop procurement process in ServiceNow using Flow Designer.

The workflow automatically creates and assigns a Catalog Task to the Hardware team after the standard laptop request is approved. This helps ensure that laptops are configured promptly and reduces manual intervention in the IT procurement process.

Problem Statement

The existing IT procurement process involves manual activities that can cause delays when handling standard laptop requests.

Standard laptop requests require configuration, but manual handling can result in oversight, delays, increased workload, and inefficient resource allocation.

Project Objective

The main objective is to implement an automated workflow using ServiceNow Flow Designer to streamline the procurement and configuration of standard laptops.

The project aims to:

- Provide a seamless laptop-request experience.
- Automatically generate configuration tasks.
- Reduce manual intervention and errors.
- Assign tasks to the Hardware team automatically.
- Improve resource utilization.
- Reduce user waiting time.
- Improve IT procurement efficiency.

User Story

«As a member of the IT procurement team, I want a streamlined process for ordering standard laptops so that tasks are automatically generated and assigned to the Hardware team for configuration.»

This ensures that laptops can be configured promptly after arrival and minimizes manual intervention.

Technology Used

- ServiceNow
- Flow Designer
- Service Catalog
- Catalog Tasks
- ServiceNow Workflow Automation

Workflow

The automated process follows these steps:

User requests Standard Laptop
          ↓
Service Catalog Request
          ↓
Request Approval
          ↓
Approval = Approved
          ↓
Flow Designer Trigger
          ↓
Create Catalog Task
          ↓
Short Description:
"Laptop need to Configured"
          ↓
Assignment Group:
"Hardware"
          ↓
Hardware Team Configures Laptop

Milestone 1: Create the Flow

A Flow named Standard Laptop Task is created in ServiceNow Flow Designer.

Flow Configuration

- Flow Name: Standard Laptop Task
- Application: Global
- Run As: System User
- Trigger: Service Catalog
- Action: Create Catalog Task

Catalog Task Configuration

The Catalog Task is configured with:

- Requested Item Record
- Short Description: "Laptop need to Configured"
- Description: "Laptop need to Configured"
- Assignment Group: "Hardware"
- Approval: "Approved"

After configuration, the Flow is saved and activated.

Milestone 2: Assign the Flow to Standard Laptop

The created Flow is assigned to the Standard Laptop Service Catalog item.

Steps

1. Open ServiceNow.
2. Navigate to Maintain Items.
3. Search for Standard Laptop.
4. Open the Standard Laptop record.
5. Go to Process Engine.
6. Remove the existing automations if required.
7. Add the Flow named Standard Laptop Task.
8. Save the record.

Milestone 3: Place a Standard Laptop Order

The Standard Laptop request is submitted through the Service Catalog.

Steps

1. Open Service Catalog.
2. Navigate to Hardware.
3. Select Standard Laptop.
4. Click Order Now.
5. Check the order status.
6. Open the Request Number.
7. Navigate to the Approvers section.
8. Approve the request.
9. Open the Requested Item.
10. Scroll to the Catalog Tasks section.
11. Open the generated Catalog Task.

Expected Result

After the request is approved, Flow Designer automatically creates a Catalog Task.

The generated task should contain:

Field| Expected Value
Short Description| Laptop need to Configured
Description| Laptop need to Configured
Assignment Group| Hardware
Approval| Approved

This allows the Hardware team to receive the configuration task automatically.

Benefits

1. Automation

The process automatically creates the required Catalog Task after approval.

2. Reduced Manual Work

Manual task creation and assignment are reduced.

3. Faster Laptop Configuration

The Hardware team receives the configuration task promptly.

4. Improved Resource Utilization

Tasks are automatically routed to the appropriate Hardware team.

5. Better User Experience

Users experience less waiting time during the laptop procurement process.

Conclusion

The Standard Laptop Procurement Automation project demonstrates how ServiceNow Flow Designer can automate IT procurement activities.

By automatically creating and assigning a Catalog Task to the Hardware team after approval, the workflow reduces manual overhead, improves task allocation, and supports timely laptop configuration.

The solution provides a streamlined and efficient process for standard laptop procurement within the IT department.
