
# Enhancement Explanations for Attended Automation Project

## Enhancement 1: Renaming Request Files with Timestamp

### Explanation

In this enhancement, the aim is to improve the organization and sorting of queries by appending a timestamp to the filename of processed request files before moving them to the Requests folder.

### Implementation Steps

1. After processing the request, we extract the current date and time timestamp.
2. We then rename the request file by combining the original name with the extracted timestamp (e.g., "Request_2023-08-21_152536.xlsx").
3. Finally, the renamed file is moved to the Requests folder.

## Enhancement 2: Capturing All Fields for Zoho Ticket Creation

### Explanation

This enhancement aims to provide a more comprehensive solution by capturing all available fields, not just the mandatory three, for creating a ticket in Zoho Desk.

### Implementation Steps

1. Modify the data collection process to include all relevant fields needed to create a Zoho Desk ticket.
2. Use these captured fields to populate the necessary data when creating the Zoho Desk ticket.

## Enhancement 3: Adding Stop Automation Hotkey

### Explanation

To enhance user control, we introduce the option to stop the attended automation using a designated hotkey combination.

### Implementation Steps

1. Assign a specific hotkey combination (e.g., Ctrl + Shift + S) to trigger the automation stop.
2. Continuously monitor for this hotkey combination during the automation execution.
3. If the hotkey combination is detected, gracefully stop the automation by completing ongoing processes and notifying the user.

## There are 3 types of xaml files used to create automation, these are as follows

Main.xaml
This is the main workflow which will invoke other workflows and orchestrate the automation.

### ReadRequest.xaml

This picks the Request Excel file from the folder we created, read the ticket data, and incorporate them in variables for the next workflow to process.

### SaaSAutomation.xaml

SaaS - Software as a Service Zoho application is used here to obtained/read data from Request file to create support ticket/job card.
