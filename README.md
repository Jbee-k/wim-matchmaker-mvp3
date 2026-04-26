# WIM Matchmaker MVP

**AI-Powered Mentor-Mentee Matching Platform for Women in Manufacturing**

A lightweight, browser-based application for the Kenya Association of Manufacturers (KAM) to match mentors with mentees using an intelligent 7-factor algorithm.

## 🎯 Overview

The WIM Matchmaker MVP is a standalone HTML/JavaScript application that:

- Imports participant data from Google Forms (via CSV)
- Runs a 7-factor compatibility algorithm
- Generates AI-powered rationales for each pairing
- Provides a human-in-the-loop review interface
- Exports data for email notifications and audit trails

**Key Principle:** AI suggests, humans decide. Every pairing requires admin approval.

## 🚀 Quick Start

### Option 1: Local Use (No Server Needed)

1. Download `index.html`
2. Double-click to open in your browser
3. Login with password: `kam2026`
4. Start matching!

### Option 2: Online Access

Visit: [Live URL will be provided after deployment]

## 📋 The 8-Phase Workflow

### Phase 1: Setup (35 minutes, one-time)
- Create Google Form with 17-question Right Seat Profile
- Create Google Sheet to collect responses
- Configure Matchmaker with Google Sheet URL
- Test with sample submission

### Phase 2: Participant Intake (5 working days)
- Email Google Form link to 30 confirmed participants
- Track submissions daily
- Send reminders on day 4
- Target: 80%+ submission rate (24 of 30)

### Phase 3: Import (90 seconds)
- Download CSV from Google Sheet
- Upload CSV into Matchmaker
- System dedupes and imports participants

### Phase 4: Run Matching (Instant)
- Click "Run Matching Algorithm"
- System scores all 225 combinations (15 mentors × 15 mentees)
- Generates top 3 options per mentee with AI rationale

### Phase 5: Human Review (30 minutes)
- Adline + Mercy sit together
- Review each of 15 proposed pairings
- Approve top match or alternative
- Reject if needed
- All decisions logged in audit trail

### Phase 6: Match Reveal (1 day)
- Export Mail Merge CSV
- Use Gmail YAMM to send personalized emails
- All 30 participants notified simultaneously

### Phase 7: Pair Activation (Within 7 days)
- Pairs reach out to schedule first Level 10 meeting
- Adline tracks follow-through
- Escalate if anyone unresponsive after 14 days

### Phase 8: Archive (1 minute)
- Export Audit JSON
- Save to KAM programme drive
- Complete record of all decisions

## 🧠 The 7-Factor Algorithm

| Factor | Weight | Description |
| :--- | :--- | :--- |
| **Focus Alignment** | 20 | Do they share the same focus area? |
| **Communication Style** | 15 | Are their mentoring styles compatible? |
| **Sector Match** | 25 | Are they in the same manufacturing sector? |
| **Strengths vs Ceiling** | 20 | Does mentor's strength address mentee's gap? |
| **Capacity Alignment** | 10 | Can they meet at compatible times? |
| **Deal Breakers** | Hard stop | Any disqualifying factors (e.g., same company)? |
| **Diversity Bonus** | 5 | Cross-sector perspective adds value |

**Total Score:** 0-100%

## 📊 Key Features

### Settings Tab
- Configure Google Form URL
- One-time setup

### Submissions Tab
- Import CSV from Google Forms
- View all participants
- Track mentor vs mentee count
- Deduplication on re-import

### Matching Tab
- Run the 7-factor algorithm
- Review AI-recommended pairings
- See compatibility breakdown
- Read AI-generated rationale
- Approve/Reject each pairing

### Approved Tab
- View all approved pairings
- Export Mail Merge CSV (for Gmail YAMM)
- Export Audit JSON (complete record)
- Trigger Match Reveal

### Audit Trail Tab
- Complete log of all actions
- Timestamps for all decisions
- Accountability and transparency

## 🔐 Security & Privacy

- **Local Storage:** All data stored in browser (no server)
- **No Cloud Upload:** Data never leaves your computer
- **Password Protected:** Simple password login (kam2026)
- **Audit Trail:** Every action logged with timestamp

## 📱 Browser Compatibility

Works on:
- Chrome / Chromium
- Firefox
- Safari
- Edge

Requires: Modern browser with JavaScript enabled

## 🛠️ Technical Details

- **Technology:** HTML5 + JavaScript (Vanilla)
- **Storage:** Browser localStorage
- **Dependencies:** None (standalone)
- **File Size:** ~150KB
- **Offline:** Works completely offline

## 📧 Email Integration

### Gmail YAMM Setup (One-Time, 5 minutes)

1. Install YAMM extension: https://yamm.com/
2. Open Gmail
3. Click YAMM → New Merge
4. Upload Mail Merge CSV from Matchmaker
5. Use email template with merge fields
6. Send to all participants

### Email Template Example

```
Subject: 🎉 Your WIM Mentorship Match is Ready!

Dear {{recipient_name}},

Welcome to Cohort 1 of the Women In Manufacturing Mentorship Programme!

After careful review, we are delighted to introduce you to your 
{{partner_role}}: {{partner_name}} from {{partner_company}} ({{partner_sector}}).

Why you've been paired:
{{rationale}}

Your first step:
{{suggested_first_step}}

Looking forward to your success!

Best regards,
Value Connect & KAM
```

## 📚 Documentation

See the accompanying guides:
- `Google_Form_Setup_Guide.md` - How to create the 17-question form
- `Admin_Workflow_Guide.md` - Step-by-step usage instructions
- `Email_Templates.md` - Ready-to-use email templates

## 🎯 Roles & Responsibilities

| Role | Responsibility |
| :--- | :--- |
| **Adline (KAM)** | Owns operational flow: form setup, CSV import, reveal send, tracking |
| **Mercy + Jay (Value Connect)** | Join 30-min review session; provide judgment on pairings |
| **Matchmaker App** | Scores combinations, generates rationale, logs decisions |

## 📊 Timeline

- **Total elapsed time:** ~10 working days (5 intake + 1 review + 1 setup + 3 buffer)
- **Adline hours:** ~4-5 hours total, spread over 10 days
- **Mercy hours:** ~30 minutes (review session)

## 🔄 Scalability

This MVP is designed for Cohort 1 (30 participants, 15 pairs).

For future cohorts:
- Simply repeat the 8-phase workflow
- No code changes needed
- Reuse the same Matchmaker
- Scale to 50+ participants if needed

## 💡 Key Principles

✅ **Human-in-the-loop** - AI suggests, humans decide
✅ **Transparent** - Every pairing has clear reasoning
✅ **Auditable** - Complete record of all decisions
✅ **Fair** - Multiple factors considered, not just one
✅ **Scalable** - Works for 30 or 300 people
✅ **Simple** - Minimal training needed
✅ **Practical** - Uses tools KAM already has

## 🚨 Important Notes

- **Password:** Default is `kam2026` - Change after first login
- **Data Backup:** Export Audit JSON regularly
- **Browser Cache:** Clear cache if issues occur
- **CSV Format:** Must match Google Forms export format

## 📞 Support

For issues or questions:
- Email: support@valueconnect.co.ke
- Contact: Value Connect Programme Manager

## 📄 License

© 2026 Value Connect Management Consultancy Ltd.
Built for Kenya Association of Manufacturers (KAM)

---

**Version:** 1.0  
**Last Updated:** May 2026  
**Status:** Production Ready
