# In-House Order Processing Automation

## Overview
This project automates the order processing workflow using SharePoint and Power Automate. The system ensures timely approvals and facilitates the creation of orders in the system.

## Key Features
- **Approval Workflow**: Includes approvals from Department VP, Finance Manager (for DAR funded orders), and Finance VP.
- **Order Creation**: Once all approvals are received, the order is processed and entered into the system.
- **Notifications**: Automated emails to the requestor with order confirmation and status updates.
- **Reminder Mechanism**: Sends reminders if approvals are delayed beyond three days.

## System Requirements
- **SharePoint**: Used for storing and tracking order data.
- **Power Automate**: Automates the approval workflow and email notifications.
- **Email Integration**: Sends emails for approvals and notifications at key steps.

## Process Flow
1. **Order Creation**: User creates an order in the SharePoint list.
2. **Department VP Approval**: Power Automate sends an approval request email to the Department VP.
3. **Finance Manager Review (if DAR Funded)**: Finance Manager reviews the order and assigns a DAR Account Number.
4. **Finance VP Approval**: Power Automate sends an approval request email to the Finance VP.
5. **Order Creation in System**: In-house team creates the order in the system.
6. **Notification to Requestor**: Requestor receives an email with the order number.
7. **Approval Reminder**: Power Automate sends reminder emails if approvals are pending for more than three days.

## SharePoint List Configuration
- **Title**: A unique identifier for the order.
- **Cost Center**: The department or business unit requesting the order.
- **Business Justification**: A description of the reason for the order.
- **Delivery Address and Attention To**: The delivery destination and the recipient of the order.
- **Status**: The current status of the order.
- **SKU and Per Unit Cost**: The SKU and per unit cost of the ordered product.
- **Total Cost**: The calculated total cost of the order.
- **DAR Funded**: Indicates if the order is DAR funded.
- **DAR Account Number**: The DAR account number assigned by Finance.
- **Order Number from In-house**: The order number assigned by the In-house team.
- **Approval Info from Dept VP**: Contains the approval information from the Department VP.
- **Approval Info from Finance**: Contains the approval information from the Finance VP.
- **Attachment(s) if Any**: Any attachments related to the order.

## Appendices
- **Troubleshooting Common Issues**
  - Approval emails not being sent to the right person.
  - Requestor not receiving the order confirmation email.
- **Contact Information**
  - For support, contact the IT support team i.e. Hamad Ullah
