# Personal Assistant with Strands Agents

This sample implements a personal assistant agent using Strands' [agents as tools](https://strandsagents.com/latest/user-guide/concepts/multi-agent/agents-as-tools/) functionality.


## 🏗️ Architecture Overview
![architecture](images/multi-agent-architecture.png)

## 🌟 Agent tools

### 📅 Calendar Assistant
- **Create Appointments**: Schedule new appointments with date, time, location, and descriptions
- **List All Appointments**: View all scheduled appointments in a formatted list
- **Update Appointments**: Modify existing appointments by ID
- **Daily Agenda**: Get a formatted agenda for any specific date
- **Time Awareness**: Built-in current time functionality

## 🛠️ Usage Examples

### Calendar Agent


### output :

```
============================================================
🗓️  WELCOME TO YOUR PERSONAL CALENDAR ASSISTANT  🗓️
============================================================
✨ I can help you with:
   📅 Create new appointments
   📋 List all your appointments
   🔄 Update existing appointments
   📆 Get your daily agenda
   🕐 Check current time

💡 Tips:
   • Use dates in format: YYYY-MM-DD HH:MM
   • I'll always provide appointment IDs for updates
   • Try: 'What's my agenda for today?' or 'Book a meeting'

🚪 Type 'exit' to quit anytime
============================================================

👤 You: 🗓️ Appointment 1 

Title: Team Standup Meeting
Date: 15 March 2025
Time: 10:00 AM – 10:30 AM
Location: Zoom
Notes: Daily project sync with the development team
Appointment ID: apt-001
🤖 CalendarBot: I'd be happy to help you create your first appointment! To set up "Appointment 1" for you, I'll need a few details:

1. **Date and time** - When would you like to schedule this appointment? (format: YYYY-MM-DD HH:MM)
2. **Location** - Where will this appointment take place?
3. **Description** - What is this appointment for?

Once you provide these details, I can create the appointment and give you the appointment ID for future reference.


👤 You: 💭 Please enter a message or type 'exit' to quit
👤 You: 🤖 CalendarBot: Great! I have the title "Team Standup Meeting" for your appointment. I still need a few more details to create it:

1. **Date and time** - When would you like to schedule this meeting? (format: YYYY-MM-DD HH:MM)
2. **Location** - Where will this meeting take place?
3. **Description** - Any additional details about the standup meeting?

Once you provide these details, I can create the appointment for you.


👤 You: 🤖 CalendarBot: Perfect! I have:
- **Title**: Team Standup Meeting  
- **Date**: 15 March 2025

I still need two more details:

1. **Time** - What time should the meeting be scheduled? (format: HH:MM, e.g., 09:00, 14:30)
2. **Location** - Where will this meeting take place?
3. **Description** - Any additional details about the standup meeting?

Once you provide the time, location, and description, I can create the appointment for you.


👤 You: 🤖 CalendarBot: Excellent! I now have:
- **Title**: Team Standup Meeting
- **Date**: March 15, 2025
- **Time**: 10:00 AM – 10:30 AM

I still need two more details to create the appointment:

1. **Location** - Where will this meeting take place? (e.g., Conference Room A, Zoom, Office Building, etc.)
2. **Description** - Any additional details about the standup meeting? (e.g., "Daily team sync to discuss progress and blockers")

Once you provide the location and description, I'll create the appointment and give you the appointment ID.


👤 You: 🤖 CalendarBot: Perfect! I now have:
- **Title**: Team Standup Meeting
- **Date**: March 15, 2025
- **Time**: 10:00 AM – 10:30 AM
- **Location**: Zoom

I just need one more detail:

**Description** - Any additional details about the standup meeting? (e.g., "Daily team sync to discuss progress and blockers", "Weekly team check-in", etc.)

Once you provide the description, I'll create the appointment and give you the appointment ID.


👤 You: 🤖 CalendarBot: Perfect! Now I have all the details needed. Let me create your appointment:
Tool #1: create_appointment
✅ Your "Team Standup Meeting" has been successfully created!

**Appointment Details:**
- **ID**: f26299be-a87f-44c9-8e16-82bff6b39e56
- **Date**: March 15, 2025
- **Time**: 10:00 AM
- **Location**: Zoom
- **Description**: Daily project sync with the development team

Save the appointment ID (f26299be-a87f-44c9-8e16-82bff6b39e56) if you need to update this appointment later!


👤 You: 🤖 CalendarBot: I understand you'd like to reference this appointment as "apt-001", but the system has automatically assigned it the ID: **f26299be-a87f-44c9-8e16-82bff6b39e56**

This is the ID that's stored in the database and what you'll need to use if you want to update or modify this appointment later.

Would you like me to:
1. Help you create another appointment?
2. Show you all your appointments?
3. Update this existing appointment with any changes?

Just let me know how else I can help with your calendar management!


👤 You: exit

=======================================
👋 Thanks for using Calendar Assistant!
🎉 Have a great day ahead!
=======================================
```




### Installation

1. **Clone the repository**:
```bash
git clone https://github.com/strands-agents/samples.git
cd 02-samples/05-personal-assistant
```

2. **Set up Python virtual environment**:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

2. **Install dependencies**:
```bash
pip install -r requirements.txt
```

3. **Configure AWS credentials**:
```bash
aws configure
# OR set environment variables
export AWS_ACCESS_KEY_ID=your_access_key
export AWS_SECRET_ACCESS_KEY=your_secret_key
export AWS_DEFAULT_REGION=us-east-1
```



### Quick Start

#### Calendar Assistant
```bash
python -u calendar_assistant.py
```

#### Personal Assistant (multi-agent collaboration)
```bash
python -u personal_assistant.py
```







**Happy Assisting!** 🤖✨