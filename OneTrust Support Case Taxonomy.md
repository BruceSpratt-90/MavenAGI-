OneTrust Support Case Taxonomy (Solution / Product / Capability)
Source: GCS May 2026 Final Taxonomy PDF, owned by OneTrust GCS.

Use this document to determine Solution → Product → Capability during support-case intake. Each Product belongs to exactly one Solution; selecting a Product deterministically fixes its Solution. Capability is dependent on Product.

How to use this document
When the customer is filing a support case, you MUST settle Solution / Product / Capability before invoking the case-create action. The chat intake form HIDES those three fields, so the customer can only verify them via what you say in chat first.

Flow (matches Bruce Spratt's specification, 2026-05-19):

If the customer has described a specific problem. Acknowledge you can raise a case, then state what you have inferred so far — name Solution, Product, and Capability explicitly. For any dimension you cannot identify with confidence, mark it as still-to-confirm and present the valid options for that dimension only. Example phrasing:

Sure, I can raise a case — but first I'd like to make sure I have the details correct. From what you've told me: Solution is Privacy Automation; Product is Privacy Incident Management; I am not sure about Capability — which one of these matches best? — [list valid Capabilities under Privacy Incident Management]

Iterate until the customer has confirmed all three. Even when you can infer all three with high confidence, state them back and explicitly ask the customer to confirm before drafting. Never silently guess and skip the confirmation step.

If the customer's message is too vague to infer anything. Walk one question per turn:

Ask about Solution — list only the seven Solutions from this document.
After they pick a Solution, ask about Product — list only the Products under that Solution.
After they pick a Product, ask about Capability — list only the Capabilities under that Product.
Then confirm the full set back before drafting.

Rules that apply in both cases
Use the exact strings as written in this document, including any odd whitespace or curly punctuation. Salesforce stores values as-is and rejects close-but-not-exact matches.
Do not present options outside the chosen Solution / Product. Do not invent values not in this document.
Do not ask the customer to volunteer Solution / Product / Capability themselves — they do not know the taxonomy. You drive the narrowing.
Consent & Preferences
Universal Consent & Preference Management
Admin UI
End User’s Consent Experience
Public API
Integration Workflows
Dashboards and Reports
Bulk Action
Consent Management (CMP)
Consent Services
Consent SDK
Scanning and Detection
Consent Experience
Third Party Integrations
Dashboards and Reports
Privacy Automation
Data Mapping Automation
Inventory Manager
Personal Data
Data Lineage
Inheritance Settings
Cross-Border Map
Inventory Records
Assessments
Automation Rules
Dashboards and Reports
Email Templates and Notifications
Roles and Permissions
Assessment Automation
Assessments
Assessment Templates
Skip/Show Logic
Workflows
Routing Rules
Projects
Automation Rules
Dashboards and Reports
Email Templates and Notifications
Roles and Permissions
Privacy Incident Management
Incident Register
Attribute Manager
Assessments
Workflows
Routing Rules
Web Forms
Databreachpedia
Automation Rules
Dashboards and Reports
Email Templates and Notifications
Roles and Permissions
Privacy Notice Management
Privacy Notices
Attribute Manager
Workflows
Templates
Section Templates
SDK Integration
Share Links
Track Changes
Consent Integration
Dashboards and Reports
Email Templates and Notifications
Roles and Permissions
DataGuidance
User Management
Copilot
Collections
Jurisdictional Map
NIS2 & DORA
News Articles
Topics
Retention Schedules
Information Hub
Comparisons
Data Transfers
Law Tracker
Enforcement Dashboard
Data Subject Request (DSR) Automation
Data Subject and Trust Portal
Web Forms
Workflows
Requests
Subtasks
Response Templates
Translations
Identity Verification
Dashboards and Reports
Email Templates and Notifications
Roles and Permissions
Data Redaction
Redaction Preferences
Redaction Workspace
File Upload
Discovery and Classification
Data & AI Governance
Data Discovery & Classification
Data Scanning
Data Classification
Data Inventory
Data Policies
Violations Monitoring
Dashboard
AI Governance
AI Inventory
Assessments
Attribute Manager
Workflows
Automation Rules
Program Center
Transparency Reporting
Model Gallery & Model Cards
AI Ecosystem Integrations
AI Automations
Dashboards and Reports
Email Templates and Notifications
Roles and Permissions
Tech Risk & Compliance
Compliance Automation
Compliance Initiatives
Controls
Evidence Tasks
Standards & Frameworks
Automated Evidence Collection
Dashboards and Reports
Roles and Permissions
Email Templates and Notifications
Audit Management
Audits
Workpapers
Findings
Attribute Manager
Workflows
Roles and Permissions
Automation Rules
Enterprise Policy Management
Standards, Policies, Procedures
Attestations
Exceptions
Dashboards and Reports
Templates
Attribute Manager
Workflows
Automation Rules
Roles and Permissions
Email Templates and Notifications
IT Risk Management
Risk Management
Controls
Evidence Tasks
Issues Management
ITRM Assessments
Inventories
Libraries
Standards & Frameworks
Dashboards and Reports
Templates
Attribute Manager
Workflows
Automation Rules
Roles and Permissions
Email Templates and Notifications
Certification Automation
Readiness Projects
Statement of Applicability
Audit Projects
Audit Findings
Risk
Compliance Portfolio
InfoSec Dashboard
Policies
Procedures
Controls
Evidence Tasks
Integrations
Users and Roles
Employee Apps
Policy Training
Onboarding and Offboarding
Authentication Setup
Questionnaires
Vendors
Assurance Tools
OneTrust Library
Guidance / Templates
Third-Party Management
Third-Party Risk Management
Inventories
Engagements
Contracts
Issues Management
TPRM assessments
Dashboards and Reports
Templates
Workflows
Automation Rules
Attribute Manager
Roles and Permissions
Email Templates and Notifications
Third-Party Risk Exchange
Exchange
Breach/Incident Newsfeeds
Vendor Scores
Third-Party Due Diligence
Screening and Monitoring
TPDD Assessments
Enhanced Due Diligence services
Due Diligence integrations
Dashboards and Reports
Attribute Manager
Automation Rules
Templates
Workflows
Roles and Permissions
Email Templates and Notifications
Platform
Identity, Security & Data Gov
Single Sign On
SCIM
Collaboration & Engagement
Email Settings
Integrations & Automation
API
Gallery
Systems
Credentials
Values
Integrations
Workflow - Builder
Workflow - Details
Workflow - Logs
Workflow - Activity
Artificial Intelligence
Platform AI Features
Account Management
Access
Single Sign On
Tenant Access
Knowledge Base Access (myOT)
User Permissions
Account Query
Billing
Subscription
Account Contacts
Security Query
Performance
Performance
