# 🎫 Discord Modmail Bot - User Documentation

**Welcome to the Modmail Bot!** This documentation explains how to use all the features of our Discord modmail system.

**Developer:** <img src="https://img.shields.io/badge/demondev_-7289DA?style=flat&logo=discord&logoColor=white" alt="demondev_">  
**Built with:** <img src="https://img.shields.io/badge/Discord.js-14.0.0-blue?style=flat&logo=discord" alt="Discord.js"> <img src="https://img.shields.io/badge/Node.js-18.0.0+-green?style=flat&logo=node.js" alt="Node.js"> <img src="https://img.shields.io/badge/SQLite-3.0+-orange?style=flat&logo=sqlite" alt="SQLite">  
**Version:** 1.0.0 • Last Updated: January 2025

## 📋 What is Modmail?

Modmail is a system that allows users to privately message server staff through Discord DMs. When you send a message to the bot, it creates a private channel where staff can respond to you while keeping your identity private.

## 🚀 Getting Started

### How to Contact Staff
1. **Send a DM** to the bot with your message
2. **A ticket will be created** automatically
3. **Staff will respond** through the ticket system
4. **You'll receive responses** via DM from the bot

### What Happens When You DM the Bot
- ✅ **Automatic ticket creation** - No need to wait
- ✅ **Staff notification** - Team is alerted immediately
- ✅ **Private communication** - Your identity stays private
- ✅ **File support** - Send images, videos, and files
- ✅ **Message history** - Complete conversation log

## 🎮 Available Commands

### For All Users
| Command | Description | Usage |
|---------|-------------|-------|
| `/help` | Show help menu | `/help` |
| `/stats` | View bot statistics | `/stats` |
| `/status` | Check system status | `/status` |
| `/info` | Bot information | `/info` |
| `/ping` | Check bot latency | `/ping` |

### For Staff Members
| Command | Description | Usage |
|---------|-------------|-------|
| `/tickets` | List all tickets | `/tickets list` |
| `/close` | Close a ticket | `/close ticket_id reason` |
| `/claim` | Claim ticket exclusively | `/claim ticket_id` |
| `/unclaim` | Unclaim a ticket | `/unclaim ticket_id` |
| `/assign` | Assign to another staff | `/assign ticket_id @user` |
| `/block` | Block user from tickets | `/block @user reason` |
| `/unblock` | Unblock a user | `/unblock @user` |

### For Staff - Documentation
| Command | Description | Usage |
|---------|-------------|-------|
| `/note` | Add internal note | `/note ticket_id content` |
| `/notes` | View all notes | `/notes ticket_id` |
| `/transcript` | Generate transcript | `/transcript ticket_id` |

### For Staff - Moderation
| Command | Description | Usage |
|---------|-------------|-------|
| `/blacklist` | Manage blacklists | `/blacklist user add @user reason` |
| `/auto-response` | Set auto replies | `/auto-response add trigger response` |

### For Administrators
| Command | Description | Usage |
|---------|-------------|-------|
| `/setup` | Configure modmail | `/setup auto` or `/setup manual` |
| `/config` | View/edit settings | `/config` |
| `/reset` | Reset configuration | `/reset confirm:RESET` |

## 🎨 Features Explained

### 🎫 Ticket System
**How it works:**
- **User sends DM** → Bot creates ticket
- **Staff responds** → User gets DM reply
- **File sharing** → Images, videos, files supported
- **Message history** → Complete conversation saved

**Ticket Status:**
- 🟢 **Open** - Active ticket
- 🔴 **Closed** - Resolved ticket
- 🟡 **Pending** - Waiting for response

### 🛡️ Blacklist System
**User Blacklist:**
- Staff can block users from creating tickets
- Blocked users get a message explaining why
- Easy unblocking system available

**Word Blacklist:**
- Automatic filtering of messages
- Actions: `block`, `flag`, `warn`
- Staff review for flagged content

### ⚡ Auto-Responses
**Automatic replies** for common questions:
- **Password reset** - Automatic link to reset page
- **FAQ answers** - Quick responses to common questions
- **Welcome messages** - Greeting new users
- **Closing messages** - Thank you notes

**Response Types:**
- `reply` - Send automatic response
- `close` - Close ticket automatically
- `flag` - Flag for staff review

### 📊 Statistics & Analytics
**Live statistics** showing:
- Total tickets created
- Open vs closed tickets
- Average response times
- Staff performance metrics
- Daily/weekly/monthly trends

### 📋 Staff Notes
**Internal communication:**
- Add notes visible only to staff
- Track important information
- Share context with team
- Maintain ticket history

### 📄 Transcripts
**Complete conversation records:**
- Generate detailed transcripts
- Include all messages and files
- Perfect for record keeping
- Export for external use

## 🎯 How to Use the Bot

### For Users
1. **Send a DM** to the bot with your question/issue
2. **Wait for response** - Staff will reply through the system
3. **Continue conversation** - Reply to bot messages to continue
4. **Send files** - Attach images, videos, or documents
5. **Ticket closes** - Staff will close when resolved

### For Staff
1. **Check tickets** - Use `/tickets list` to see open tickets
2. **Claim tickets** - Use `/claim ticket_id` to take responsibility
3. **Respond to users** - Type in the ticket channel
4. **Add notes** - Use `/note` for internal information
5. **Close tickets** - Use `/close` when resolved

### For Administrators
1. **Setup system** - Use `/setup auto` for quick setup
2. **Configure settings** - Use `/config` to customize
3. **Manage staff** - Assign roles and permissions
4. **Monitor system** - Check statistics and logs
5. **Backup data** - Use `/backup` for safety

## 🎨 Customization Options

### Welcome Messages
Customize the message users see when their ticket is created:
- Personal greeting
- What to expect
- Response time estimates
- Contact information

### Close Messages
Customize the message when tickets are closed:
- Thank you notes
- Follow-up information
- Survey links
- Future contact details

### Ticket Categories
Organize tickets by type:
- 🚀 **Support** - General help
- 🐛 **Bug Report** - Technical issues
- 💡 **Feature Request** - New ideas
- ⚠️ **Complaint** - Issues to address
- ❓ **Question** - General questions

### Priority Levels
Set ticket importance:
- 🔴 **Urgent** - Immediate attention needed
- 🟡 **High** - Important but not urgent
- 🟢 **Medium** - Normal priority
- 🔵 **Low** - Can wait

## 🚨 Common Scenarios

### User Can't Create Ticket
**Possible reasons:**
- User is blacklisted
- Bot is offline
- System is under maintenance
- User has too many open tickets

**Solutions:**
- Contact server administrator
- Check bot status with `/status`
- Wait and try again later

### Staff Can't Respond
**Possible reasons:**
- Missing permissions
- Ticket already claimed
- System error
- Bot offline

**Solutions:**
- Check role permissions
- Use `/unclaim` if needed
- Contact administrator
- Check bot status

### Files Not Sending
**Supported formats:**
- Images: PNG, JPG, GIF, WebP
- Videos: MP4, MOV, AVI
- Documents: PDF, DOC, TXT
- Archives: ZIP, RAR

**File size limits:**
- Maximum 25MB per file
- Multiple files per message
- Automatic compression for large files

## 📞 Getting Help

### For Users
- **Check this documentation** - Most questions answered here
- **Contact staff** - Send a DM to the bot
- **Check bot status** - Use `/status` command
- **Server support** - Ask in the main server

### For Staff
- **Review commands** - Use `/help` for command list
- **Check logs** - Use `/logs` for ticket history
- **Contact admin** - For technical issues
- **Training available** - Ask for staff training

### For Administrators
- **System monitoring** - Regular status checks
- **Backup procedures** - Weekly backups recommended
- **Staff training** - Regular training sessions
- **System updates** - Keep bot updated

## 🔄 System Status

### Bot Status Indicators
- 🟢 **Online** - Bot is working normally
- 🟡 **Maintenance** - System under maintenance
- 🔴 **Offline** - Bot is not responding
- 🔵 **Limited** - Some features disabled

### Maintenance Schedule
- **Daily** - Status checks and statistics
- **Weekly** - Database cleanup and backups
- **Monthly** - System updates and optimization
- **As needed** - Emergency maintenance

## 📋 Best Practices

### For Users
- **Be clear** - Explain your issue clearly
- **Be patient** - Staff will respond as soon as possible
- **Provide details** - Include relevant information
- **One issue per ticket** - Keep topics focused
- **Respect staff** - Be polite and cooperative

### For Staff
- **Respond quickly** - Aim for timely responses
- **Be professional** - Maintain professional tone
- **Use notes** - Add internal notes for context
- **Close properly** - Ensure issues are resolved
- **Follow up** - Check on resolved tickets

### For Administrators
- **Monitor system** - Regular status checks
- **Train staff** - Provide proper training
- **Backup regularly** - Protect important data
- **Update system** - Keep bot current
- **Gather feedback** - Improve user experience

---

**🎫 Modmail Bot - Professional Discord Support System**

*This documentation is regularly updated. Last updated: January 2025* 

Copyright © 2025 DEMON. All rights reserved.
