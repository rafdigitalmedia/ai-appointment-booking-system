🤖 AI Appointment Booking System





An intelligent automation that books appointments from Google Sheets to Google Calendar — checking availability, creating events, and sending emails automatically.
See It In Action
✨ Features
🤖 AI-Powered Data Extraction — Extracts appointment details from unstructured messages
📅 Smart Calendar Checking — Real-time availability verification before booking
✅ Auto-Booking — Creates calendar events when slots are available
📧 Alternative Slots Email — Sends alternative times when requested slot is busy
🔄 Two-Way Sync — Updates both Google Calendar and Sheets automatically
⚡ Instant Processing — Under 2 minutes from request to confirmation
🛠️ Tech Stack
Tool
Purpose
n8n
Workflow automation engine
Google Gemini AI
Intelligent data extraction from booking requests
JavaScript
Custom date/time processing and event counting
Google Calendar
Event creation and availability checking
Google Sheets
Booking request storage and status tracking
Gmail
Automated email notifications
Business Impact
Metric
Before
After
Booking processing time
15-30 minutes per request
< 2 minutes
Double-booking errors
10-15%
0%
Response time
2-24 hours
Instant
Manual hours/week
5-10 hours
< 30 minutes
🚀 How It Works

Google Sheets (New Booking Request)
    ↓
AI Analysis (Extract appointment details)
    ↓
JavaScript (Process & format data)
    ↓
Check Calendar Availability
    ↓
Count Events (JavaScript)
    ↓
IF Router (Is Slot Available?)
    ├─ True → Send Alternative Slots Email
    └─ False → Book Calendar → Update Sheet

    Screenshots
Full Workflow
Google Sheets Trigger
AI Analysis & Data Extraction
Process Appointment Data
Check Calendar Availability
Count Events Logic
IF Router - Slot Availability
Send Alternative Slots Email
Book Appointment in Calendar
Update Booking Status
Calendar Event Created
Updated Sheet Status
Installation
Import AI Lead Qualification.json to your n8n instance
Configure Google Sheets credentials (for trigger and updates)
Configure Google Calendar credentials
Set up Google Gemini API key for AI analysis
Configure Gmail credentials for email notifications
Create Google Sheet with required columns (see below)
Activate workflow and test with a new row!
Required Google Sheets Columns:
Full Name
Email
Phone
Service Type
Requested Date
Requested Time
Time Zone
Message
Booking Status
Calendar Event ID
Confirmation Sent
💼 Use Cases
🏢 Consulting Firms — Automate client appointment scheduling
Service Providers — Book consultations without manual work
🏥 Healthcare Clinics — Manage patient appointments
💇 Salons & Spas — Handle booking requests 24/7
🎓 Tutors & Coaches — Schedule sessions automatically
🏡 Real Estate Agents — Book property viewings
🔧 Customization
Business Hours: Modify the IF condition to check business hours
Buffer Time: Add buffer before/after appointments in JavaScript node
Email Templates: Customize the alternative slots email in Gmail node
AI Prompts: Adjust the AI analysis prompt for your specific service types
📝 License
MIT License — free to use and modify for personal or commercial projects.
Built with ❤️ using n8n and Google AI
For inquiries or custom automation projects, feel free to reach out!
