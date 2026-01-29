# State Affairs Help Center Documentation

Complete help center documentation for State Affairs, ready to deploy on Documentation.AI.

## 📚 Contents

- **13 MDX files** organized into 3 categories
- **Customer Guides** (7 documents)
- **Internal Resources** (3 documents)  
- **Reference Materials** (3 documents)
- Complete navigation configuration

## 📁 Repository Structure

```
state-affairs-docs/
├── docs/
│   ├── documentation.json          # Navigation & site config
│   ├── customer-guides/
│   │   ├── faq.mdx
│   │   ├── billing-issues.mdx
│   │   ├── multiple-charges.mdx
│   │   ├── subscription-management.mdx
│   │   ├── access-credentials.mdx
│   │   ├── self-service-portal.mdx
│   │   └── quick-reference.mdx
│   ├── internal/
│   │   ├── response-templates.mdx
│   │   ├── ticket-analysis.mdx
│   │   └── deep-analysis.mdx
│   └── reference/
│       ├── help-center-structure.mdx
│       ├── scribe-guides.mdx
│       └── screenshots.mdx
└── README.md                        # This file
```

## 🚀 Quick Start

### Option 1: Deploy to Documentation.AI (Recommended)

1. **Create Account**
   ```bash
   # Sign up at https://dashboard.documentation.ai/signup
   # Create a new project: "State Affairs Help Center"
   ```

2. **Connect GitHub Repository**
   - Go to Settings → Integrations in Documentation.AI
   - Click "Connect GitHub"
   - Authorize Documentation.AI
   - Select this repository
   - Choose `main` branch for deployment

3. **Push This Repository**
   ```bash
   # Initialize git (if not already done)
   git init
   git add .
   git commit -m "Initial State Affairs documentation"
   
   # Add your GitHub remote
   git remote add origin https://github.com/YOUR-USERNAME/state-affairs-docs.git
   git branch -M main
   git push -u origin main
   ```

4. **Automatic Deployment**
   - Documentation.AI will automatically detect your push
   - Build and deploy your documentation
   - Your site will be live at: `https://your-project.documentationai.io`

### Option 2: Manual Upload via Web Editor

1. Sign up at Documentation.AI
2. Create new project
3. Use Web Editor to create pages manually
4. Copy/paste content from each MDX file
5. Organize navigation to match documentation.json structure

## 📝 Editing Documentation

### Using Code Editor (Git-based)

```bash
# Clone the repository
git clone https://github.com/YOUR-USERNAME/state-affairs-docs.git
cd state-affairs-docs

# Create a feature branch
git checkout -b update-faq

# Edit files in docs/
# Example: vim docs/customer-guides/faq.mdx

# Commit and push
git add .
git commit -m "Update FAQ with new billing information"
git push origin update-faq

# Create pull request on GitHub
# Documentation.AI will create a preview build
# Merge to main to deploy to production
```

### MDX File Format

Each file has frontmatter and content:

```mdx
---
title: "Page Title"
description: "Page description for SEO"
---

# Page Title

Your markdown content here...

## Subheading

- Bullet point
- Another point

[Link text](/path/to/page)
```

## 🎨 Customization

### Colors

Edit `docs/documentation.json`:

```json
"colors": {
  "primary": "#2c5aa0",    // Main brand color
  "light": "#4a7bc8",      // Lighter variant
  "dark": "#1a3a6b"        // Darker variant
}
```

### Logo

Add logo files to `docs/` directory:
- `logo.png` - Your logo (recommended: 200x50px)
- `favicon.png` - Favicon (32x32px)

Update `documentation.json`:

```json
"logo": {
  "light": "/logo.png",
  "dark": "/logo-dark.png"  // Optional: separate dark mode logo
}
```

### Navigation

Edit `docs/documentation.json` to:
- Reorder pages
- Add/remove sections
- Change group names
- Update icons (Font Awesome icon names)

## 🔍 Enhanced Components

You can upgrade plain markdown to use Documentation.AI components:

### Callouts

```mdx
<Callout kind="info">
Important information for users
</Callout>

<Callout kind="warning">
Warning about potential issues
</Callout>

<Callout kind="success">
Success message or confirmation
</Callout>
```

### Steps

```mdx
<Steps>
  <Step title="First step" icon="1">
    Do this first
  </Step>
  <Step title="Second step" icon="2">
    Then do this
  </Step>
</Steps>
```

### Code Groups

```mdx
<CodeGroup tabs="Email,Phone,Web">
  ```text
  support@stateaffairs.com
  ```
  ```text
  (786) 363-9990
  ```
  ```text
  https://stateaffairs.com/contact
  ```
</CodeGroup>
```

### Expandables

```mdx
<Expandable title="Click to expand">
  Hidden content that expands on click
</Expandable>
```

## 📊 Features After Deployment

Once deployed to Documentation.AI, you'll get:

### 1. AI-Powered Search
- Natural language search across all docs
- Fast, relevant results
- Intelligent ranking

### 2. AI Assistant
- In-page AI chat
- Answers questions from your docs
- Contextual help for users

### 3. MCP Server
- URL: `https://docs.yourdomain.com/_mcp`
- External AI tools can query your docs
- Works with Claude, ChatGPT, Cursor, etc.

### 4. Analytics
- View traffic and popular pages
- Track search queries
- Understand user behavior

### 5. Custom Domain
- Set up `docs.stateaffairs.com`
- Professional branded URL
- SSL certificate included

## 🔧 Troubleshooting

### Build Fails

Check:
- All MDX files have valid frontmatter
- No unclosed JSX tags
- documentation.json is valid JSON
- All paths in documentation.json match actual files

### Pages Not Appearing

Verify:
- File path matches what's in documentation.json
- File has .mdx extension
- Frontmatter is properly formatted

### Navigation Issues

Ensure:
- All page paths in documentation.json are correct
- No duplicate paths
- Groups are properly structured

## 📞 Support

**State Affairs Help Center Support:**
- Email: support@stateaffairs.com
- Billing: billing@stateaffairs.com  
- Phone: (786) 363-9990

**Documentation.AI Support:**
- Visit: https://documentation.ai/docs/help/contact-us
- Chat support in dashboard

## 🔄 Updating Content

### Quick Updates

1. Edit file locally
2. Commit and push to main
3. Documentation.AI auto-deploys (1-2 minutes)

### Major Changes

1. Create feature branch
2. Make changes
3. Push branch
4. Review preview build
5. Create pull request
6. Merge to main when ready

## 📈 Next Steps

After deploying:

1. **Set up custom domain**
   - Configure DNS
   - Point to Documentation.AI
   - Enable SSL

2. **Add team members**
   - Invite to GitHub repo
   - Set permissions (read/write)
   - Train on editing process

3. **Monitor analytics**
   - Track popular pages
   - Identify gaps in documentation
   - Update based on search queries

4. **Enhance content**
   - Add callouts where helpful
   - Include more examples
   - Add video tutorials

5. **Integrate with support**
   - Link from support emails
   - Reference in tickets
   - Train team to use MCP server

## 📚 Resources

- **Documentation.AI Docs:** https://documentation.ai/docs
- **MDX Syntax:** https://mdxjs.com/
- **Components Reference:** https://documentation.ai/docs/components
- **Git Workflow:** https://documentation.ai/docs/write-and-publish/code-editor

---

**Generated:** January 29, 2026  
**Format:** Documentation.AI MDX  
**Total Files:** 13 documents + 1 config file
