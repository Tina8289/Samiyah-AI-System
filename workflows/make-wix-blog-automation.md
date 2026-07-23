---
name: Samiyah Make Wix Blog Automation

description:
Automation workflow defining how Samiyah generates and publishes
AI-powered blog content using Google Sheets, Make, AI models, and Wix CMS.

version: 1.0

---

# Samiyah Make Wix Blog Automation


## Purpose


This workflow automates blog production:


Keyword

↓

AI Content Generation

↓

Image Generation

↓

CMS Data Processing

↓

Wix Blog Publishing



# Automation Architecture


Main tools:


Google Sheets

+

Make

+

AI Model

+

Image Generation

+

Wix CMS



# Workflow Overview


## Step 1: Content Input


Platform:


Google Sheets



Input fields:


- Blog Topic
- Primary Keyword
- Secondary Keywords
- Category
- Content Status



Purpose:


Content planning database.



---

# Step 2: Make Trigger


Module:


Google Sheets - Watch Rows



Trigger:


When a new content task is added
or status changes.



Output:


Send content request to AI.



---

# Step 3: AI Content Generation


Module:


AI Chat Model



Input:


Reference:


- Blog CMS Template
- SEO Rules
- Content Strategy



Generate:


- Blog Title
- SEO Title
- Meta Description
- Blog Body
- FAQ
- CTA
- Related Product Category



---

# Step 4: Image Generation


Input:


AI generated image prompts.



Generate:


Cover Image

+

Content Image



Required output:


- Image filename
- ALT text
- Description



---

# Step 5: Data Processing


Make processes:


AI response

↓

Extract fields

↓

Match Google Sheet columns

↓

Prepare Wix CMS data



---

# Step 6: Wix Blog CMS Upload


Destination:


Wix Blog CMS



Mapping:


Google Sheet / AI output


↓

Wix Fields



Required fields:


Blog Title

Primary Keyword

SEO Title

Meta Description

Category

Images

Blog Body

Related Product Category



---

# Status Management


Google Sheet status:


Pending


↓

Generating


↓

Review


↓

Published



---

# Error Handling


If generation fails:


Action:


Mark status:

Error


Record:


- Error message
- Failed step
- Time



---

# Human Review


Before automatic publishing,
optional review stage:


Check:


- Product accuracy
- Brand consistency
- SEO quality
- Image quality



---

# Future Expansion


This workflow can extend to:


Product CMS automation

↓

Solution page automation

↓

Catalog generation

↓

Customer proposal generation
