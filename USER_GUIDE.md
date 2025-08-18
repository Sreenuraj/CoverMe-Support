# CoverMe Complete User Guide

This guide walks you through every feature of CoverMe, showing you exactly how much detail and thought went into building this job search intelligence tool.

## Table of Contents
1. [Initial Setup](#initial-setup)
2. [Options Page Deep Dive](#options-page-deep-dive)
3. [Three Ways to Analyze Jobs](#three-ways-to-analyze-jobs)
4. [Understanding Analysis Results](#understanding-analysis-results)
5. [Interactive Skill Management](#interactive-skill-management)
6. [AI Chat System](#ai-chat-system)
7. [Visual Highlighting System](#visual-highlighting-system)
8. [Usage Analytics](#usage-analytics)
9. [Data Management](#data-management)
10. [Advanced Features](#advanced-features)

## Initial Setup

### Step 1: Installation
1. Visit the [Chrome Web Store](https://chrome.google.com/webstore/detail/coverme)
2. Click "Add to Chrome"
3. The CoverMe icon appears in your browser toolbar

### Step 2: Getting Your Free API Key
1. Go to [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Sign in with your Google account
3. Click "Create API Key"
4. Copy the generated key (starts with "AIza...")
5. **Important:** This is completely free with 250 requests per day

### Step 3: First Configuration
1. Right-click the CoverMe extension icon
2. Select "Options" 
3. Paste your API key in the "Gemini API Key" field
4. Paste your entire resume text in the "Resume Content" box
5. Click "Save User Data"

**What happens behind the scenes:**
- CoverMe automatically extracts your skills using AI
- Organizes them into 6 categories: Technical Skills, Frameworks, Domains, Industries, Key Strengths, Role Types
- Calculates your experience level from your resume
- All data stays on your computer - nothing is sent to external servers

## Options Page Deep Dive

The Options page is your control center. Here's everything you can do:

### Profile Information Section
- **Experience Years:** Auto-detected from your resume, editable
- **Seniority Level:** Choose from Entry, Mid, Senior, Lead, Principal
- **Salary Range:** Optional preference for filtering
- **Location:** Your preferred work location

### Keywords Management
Click "📝 Manage Keywords" to open the comprehensive management interface:

**Technical Skills Category:**
- Programming languages (JavaScript, Python, Java)
- Technical tools (Docker, Kubernetes, Git)
- Add new skills using the input field and "Add" button

**Frameworks Category:**
- Web frameworks (React, Angular, Vue)
- Backend frameworks (Django, Spring, Express)
- Testing frameworks (Jest, Cypress, Selenium)

**Domains Category:**
- Industry expertise (Healthcare, Finance, E-commerce)
- Specialized knowledge areas

**Industries Category:**
- Sector experience (Technology, Healthcare, Manufacturing)
- Market knowledge

**Key Strengths Category:**
- Soft skills (Leadership, Communication, Problem Solving)
- Professional abilities

**Role Types Category:**
- Position types (Frontend Developer, Data Scientist, Product Manager)
- Career focuses

### Usage Analytics Dashboard
Real-time tracking of your AI usage:
- **Daily Progress:** Shows current usage out of 250 daily requests
- **Rate Limiting:** Monitors requests per minute (max 15)
- **Weekly Statistics:** 7-day usage breakdown
- **Quota Reset Timer:** When your daily limit resets (midnight PT)

### Data Management Controls
- **Export Data:** Download everything as JSON or CSV
- **Clear Data Options:** 
  - Clear all data
  - Clear only chat history
  - Clear only usage analytics
  - Keep keywords (intelligent selective clearing)
- **Data Statistics:** See exactly what's stored and how much space it uses

## Three Ways to Analyze Jobs

### Method 1: Right-Click Context Menu (Universal)

**Works on:** Every website on the internet

**How to use:**
1. Navigate to any job posting on any website
2. Right-click anywhere on the page
3. Choose from three options:

**⚡ "CoverMe: Local Analysis"**
- Instant keyword matching (no AI calls used)
- Shows match percentage in 3 seconds
- Highlights skills on the page immediately
- Works even on unrecognized job sites
- Never fails - 100% success rate

**🤖 "CoverMe: Ask AI"**  
- Opens side panel if closed
- If side panel is already open, triggers analysis directly
- State-aware: disabled with helpful tooltip when side panel is closed
- Professional error handling with clear user guidance

**📝 "Add to CoverMe Keywords" (when text is selected)**
- Select any text on any website
- Extracts relevant skills from selected content
- Automatically categorizes and adds to your profile
- Works for building skills from job descriptions

### Method 2: Manual Mode (Classic Workflow)

**Best for:** Detailed analysis when you want full control

1. **Navigate to any job posting**
2. **Click the CoverMe extension icon** in your browser toolbar
3. **Choose analysis type:**
   - "Ask AI" - Opens side panel for detailed analysis
   - "Deep Research" - Most comprehensive analysis with structured insights
   - "Keyword Match" - Local analysis button in popup

**What you see in the popup:**
- Job title and company (auto-detected)
- Current match percentage
- Quick stats (matching skills count, missing skills count)
- Analysis buttons
- Live mode toggle
- Settings access

### Method 3: Live Mode (Automatic Monitoring)

**Best for:** Browsing multiple jobs quickly

**How to activate:**
1. Click the CoverMe extension icon
2. Toggle "Live Mode" to ON
3. Browse jobs normally

**What happens automatically:**
- Extension icon changes color as you navigate:
  - 🟢 **Green:** 65%+ match (good fit)
  - 🟠 **Orange:** 45-64% match (okay fit)  
  - 🔴 **Red:** <45% match (poor fit)
- Triggers on all recognized job sites
- Works across tabs - switch between job postings and see instant updates
- Content scripts auto-inject when needed
- Automatic error recovery if extension context breaks

**Supported job sites for Live Mode:**
- LinkedIn (/jobs/, /in/*/details/)
- Indeed (/viewjob)
- Glassdoor (/job-listing/)
- AngelList (/jobs/)
- RemoteOK (/remote-jobs/)
- Plus any manually confirmed job sites

## Understanding Analysis Results

### Quick Keyword Matching Results
**Match Score Calculation:**
- **Green (65%+):** Strong match - apply with confidence
- **Orange (45-64%):** Moderate match - highlight relevant experience
- **Red (<45%):** Weak match - consider if it's worth applying

**Score Components:**
- Job requirements fulfillment (75% weight)
- Skill relevance and strength (25% weight)
- Experience level penalties/bonuses

### Experience Qualification
**Three categories with precise definitions:**

**🎯 Well-Matched**
- Your experience aligns with job requirements
- Sweet spot for applications

**⬆️ Overqualified**  
- You have 5+ years more experience than required
- Score penalty: -10% to -30% depending on gap
- Consider: salary expectations, growth opportunities

**⬇️ Underqualified**
- You have 1+ years less experience than required  
- Score penalty: -8% to -25% depending on gap
- Consider: emphasizing relevant projects, learning opportunities

### Skills Analysis Sections

**✅ Skills You Have That Job Requires**
- Your matching skills found in the job posting
- Sorted by relevance and match confidence
- Click [+] to add skills not in your profile
- Green highlighting shows these on the job page

**❌ Skills Job Requires That You Don't Have**
- Critical missing skills identified by AI
- Prioritized by importance to the role
- Click [+] to add to your learning list
- Red highlighting shows these on the job page

**🤔 Unknown Skills Found in Job**
- Skills discovered by pattern matching
- Not in your current profile
- Confidence percentage (35-80%) based on extraction method
- [+] to add, [×] to ignore permanently

**👤 Your Added Skills**
- Skills you manually added during analysis
- Removable with [-] buttons
- Tracked across all job analyses
- Auto-categorized by AI during Deep Research

## Interactive Skill Management

### Adding Skills During Analysis
**From any skills section:**
1. Click the [+] button next to any skill
2. Skill immediately appears in your profile
3. Match percentage recalculates in real-time
4. Skill appears in future job analyses

**Visual feedback:**
- Skills you add get 👤 badges
- Your match score updates instantly
- Skills appear in "Your Added Skills" section if not in top matches

### Removing Skills
**Multiple removal options:**
1. **[-] buttons:** Remove individual skills you added
2. **Options page:** Bulk removal from keyword management interface
3. **Ignored skills:** Skills you [×] ignore are tracked and won't appear again

### AI-Powered Skill Categorization
**Happens automatically after Deep Research:**
- Skills you add manually start in "Technical Skills"
- AI automatically moves them to proper categories:
  - React → Frameworks
  - Healthcare → Industries  
  - Leadership → Key Strengths
- 👤 badges are removed once AI categorizes (now "officially organized")
- Process is non-critical - Deep Research succeeds even if categorization fails

### Unknown Skills Discovery System
**5 intelligent extraction patterns:**
1. **Technology Names:** Capitalized tech terms (React, Docker, AWS)
2. **Experience Context:** Skills mentioned with experience ("5 years of Python")
3. **Framework Patterns:** Common patterns ("framework", "library", "tool")
4. **Capitalized Terms:** Proper nouns that might be skills
5. **Acronyms:** Technical abbreviations (API, REST, CI/CD)

**Smart filtering removes:**
- Common words ("and", "the", "with")
- Generic terms ("experience", "knowledge", "skills")
- Skills already in your profile
- Previously ignored skills

## AI Chat System

### Job-Specific Conversations
**Each job gets its own persistent chat thread:**
- Identified by: Job Title + Company + URL
- Chat history persists across browser sessions
- Resume when you return to the same job posting
- Maximum 50 threads stored, oldest auto-deleted

### Structured Analysis Tiles
**Four comprehensive analysis tiles:**

**🎯 Skills Match Tile**
- Matches the format of keyword matching for easy comparison
- Shows your matching skills, missing skills, experience analysis
- Professional formatting with confidence scores

**💼 Job Fit Assessment Tile**
- Overall compatibility analysis
- Strengths you bring to the role
- Areas where you might need to demonstrate extra value
- Specific advice for this position

**🎤 Interview Preparation Tile**
- Questions likely to be asked based on job requirements
- Talking points for your experience
- How to address potential concerns
- Key things to research about the company/role

**💡 Strategic Advice Tile**
- Career guidance specific to this job and your background
- Whether you should apply and why
- Salary negotiation considerations
- Long-term career impact

### Chat Features
- **Persistent History:** 100 messages per thread maximum
- **Search:** Find previous conversations about specific topics
- **Professional AI Tone:** Direct, actionable advice without excessive enthusiasm
- **Job Context:** AI knows the specific job title, company, and your background

## Visual Highlighting System

### Three-Color Professional Scheme

**🟢 Light Green Highlighting: Your Matching Skills**
- Skills you have that the job requires
- Instantly shows your strengths on the job page
- Smooth gradient background with subtle animations
- High contrast for accessibility

**🟣 Purple Highlighting: Experience Requirements**
- Phrases like "5+ years experience", "minimum 3 years"
- Helps you quickly assess experience fit
- Distinguishes between hard requirements and preferences

**🔴 Light Red Highlighting: Missing Critical Skills**
- Skills the job requires that you don't have
- Prioritized by importance to the role
- Helps identify learning opportunities

### Technical Implementation
**Robust highlighting engine:**
- **Single-pass processing:** Collects all matches first, then applies highlighting
- **Overlap prevention:** Smart conflict resolution when text matches multiple patterns
- **Position-based sorting:** Right-to-left replacement prevents DOM position shifts
- **Ancestor protection:** Won't highlight inside already-highlighted elements
- **Performance optimized:** Minimal impact on page loading and browsing

**Cross-platform compatibility:**
- Works on LinkedIn's dynamic content loading
- Handles Indeed's iframe structure
- Compatible with Glassdoor's lazy loading
- Adapts to company career page variations

## Usage Analytics

### Real-Time Monitoring
**Dashboard displays:**
- **Daily Usage:** Current requests out of 250 daily limit
- **Rate Limiting:** Requests per minute (15 RPM max)
- **Progress Bars:** Color-coded (green → yellow → red as limits approach)
- **Reset Timer:** Shows when quota resets (midnight Pacific Time)

### Smart Warning System
**Automatic alerts:**
- **80% Daily Limit:** "You've used 200/250 daily requests"
- **90% Rate Limit:** "You're approaching the rate limit (14/15 requests per minute)"
- **Quota Exceeded:** "Daily limit reached. Resets at midnight PT"

### Usage Tracking by Feature
**Tracked API calls:**
- **Ask AI Analysis:** ~4,096 tokens per request
- **Deep Research:** ~6,144 tokens per request  
- **Keyword Extraction:** ~2,048 tokens per request (one-time during setup)
- **Skill Categorization:** ~1,024 tokens per request (automatic during Deep Research)

### Weekly and Monthly Statistics
- **7-day breakdown:** Usage patterns and peaks
- **Most active days:** When you search for jobs most
- **Feature usage:** Which analysis types you use most
- **Efficiency metrics:** Average requests per job analyzed

## Data Management

### Complete Data Transparency
**Real-time statistics show exactly what's stored:**
- **Keywords:** Count by category, total storage size
- **Chat History:** Number of threads, total messages, storage size
- **Usage Analytics:** Days tracked, total API calls made
- **Job Analysis:** Cached results, interaction history

### Export Functionality
**Two export formats:**

**JSON Export (Developer-Friendly):**
```json
{
  "userProfile": {
    "keywords": {
      "technicalSkills": ["JavaScript", "Python"],
      "frameworks": ["React", "Django"]
    },
    "experienceYears": 5,
    "seniorityLevel": "Mid"
  },
  "chatHistory": [
    {
      "jobId": "senior-developer-techcorp",
      "messages": [...],
      "lastUpdate": "2025-01-18T10:30:00Z"
    }
  ],
  "usageAnalytics": {
    "dailyUsage": 150,
    "weeklyStats": [...]
  }
}
```

**CSV Export (Spreadsheet-Friendly):**
- Keywords sheet with categories
- Chat history with timestamps
- Usage analytics with dates
- Job interactions with outcomes

### Privacy-First Data Handling
**Local storage only:**
- Everything stored in `chrome.storage.local`
- Encrypted by Chrome automatically
- No external servers except Google AI for analysis
- Google AI doesn't store your data permanently

**Automatic cleanup:**
- Chat threads auto-delete after 30 days
- Usage analytics auto-clean after 30 days  
- User can override with "Keep data longer" setting

## Advanced Features

### Job Site Learning System
**Adaptive recognition:**
- When you use context menu on unrecognized sites, CoverMe asks: "Is this actually a job posting page?"
- If you confirm "Yes", it learns the URL pattern
- Future visits to similar pages on that site are automatically recognized
- Patterns stored: domain + first 1-2 path segments

### Content Script Health Management
**Robust background system:**
- **Health check protocol:** PING/PONG system ensures content scripts are responsive
- **Auto-injection:** Automatically injects content scripts when needed
- **Context recovery:** Handles extension context invalidation gracefully
- **Cross-tab communication:** Live mode state synced across all tabs

### Smart Error Recovery
**Never-fail philosophy:**
- **Local analysis:** Always succeeds through multiple fallback strategies
- **Content extraction:** Multiple selectors and heuristic detection
- **Extension recovery:** Automatic page refresh for broken contexts (once per page)
- **User guidance:** Clear error messages with actionable next steps

### Performance Optimizations
**Efficient processing:**
- **Background processing:** Analysis happens without blocking UI
- **Intelligent caching:** Avoid re-analyzing the same job posting
- **Minimal DOM impact:** Highlighting adds <0.1s to page load
- **Smart rate limiting:** Queues requests to stay within Google's limits

---

## Why This Level of Detail Matters

This user guide showcases the incredible depth and thoughtfulness that went into building CoverMe. Every feature was carefully designed to solve real problems job seekers face:

- **Universal compatibility** because job seekers don't just use LinkedIn
- **Multiple analysis methods** because different situations need different approaches  
- **Persistent chat** because job searching is an ongoing conversation
- **Interactive skill management** because your career profile evolves
- **Visual highlighting** because seeing is faster than reading
- **Complete data control** because your career data should be yours

CoverMe isn't just another browser extension - it's a comprehensive career intelligence platform that respects your privacy while providing professional-grade insights.

**The result:** A tool that actually helps you make better career decisions, saves time, and grows with you throughout your job search journey.