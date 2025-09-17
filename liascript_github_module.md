# LiaScript & GitHub Integration: Self-Learning Module for Academics

## Welcome to Your Learning Journey! 🎓

This self-paced module will guide you through implementing LiaScript files into GitHub, empowering you to create interactive educational content for your students and research community.

---

## Table of Contents

1. [Module Overview](#module-overview)
2. [Learning Objectives](#learning-objectives)
3. [What is LiaScript?](#what-is-liascript)
4. [Getting Started with GitHub](#getting-started-with-github)
5. [Creating Your First LiaScript File](#creating-your-first-liascript-file)
6. [Advanced LiaScript Features](#advanced-liascript-features)
7. [Publishing with GitHub Pages](#publishing-with-github-pages)
8. [Collaboration and Version Control](#collaboration-and-version-control)
9. [Best Practices for Academic Content](#best-practices-for-academic-content)
10. [Troubleshooting Common Issues](#troubleshooting-common-issues)
11. [Resources and Next Steps](#resources-and-next-steps)

---

## Module Overview

**Duration:** 2-3 hours  
**Difficulty:** Beginner to Intermediate  
**Prerequisites:** Basic computer literacy, familiarity with text editing

This module combines theoretical knowledge with hands-on practice, ensuring you can confidently create and deploy interactive educational content using LiaScript and GitHub.

---

## Learning Objectives

By the end of this module, you will be able to:

- ✅ Understand what LiaScript is and its benefits for academic content
- ✅ Set up a GitHub repository for LiaScript projects
- ✅ Create interactive LiaScript documents with multimedia elements
- ✅ Publish LiaScript content using GitHub Pages
- ✅ Collaborate with colleagues using GitHub's version control features
- ✅ Apply best practices for creating engaging academic content

---

## What is LiaScript?

### Definition
LiaScript is an extension of Markdown that enables the creation of interactive, multimedia-rich educational content. Think of it as PowerPoint meets Jupyter Notebook, but entirely text-based and web-friendly.

### Key Features for Academics

**Interactive Elements:**
- Quizzes with immediate feedback
- Surveys for student engagement
- Interactive code execution
- Mathematical formula rendering
- Audio narration capabilities

**Content Types:**
- Course materials and lectures
- Interactive textbooks
- Research presentations
- Tutorial documentation
- Student assignments

### Why Choose LiaScript?

| Traditional Methods | LiaScript Advantages |
|-------------------|-------------------|
| Static PDFs/PowerPoints | Interactive, engaging content |
| Platform dependency | Works on any device with a browser |
| Version control challenges | Git-based version management |
| Limited collaboration | Easy sharing and collaborative editing |
| No analytics | Built-in progress tracking |

---

## Getting Started with GitHub

### Step 1: Create a GitHub Account

1. Visit [github.com](https://github.com)
2. Click "Sign up"
3. Choose a professional username (e.g., dr-smith-biology)
4. Use your academic email address
5. Verify your account

**💡 Tip:** Many universities offer GitHub Pro accounts for free to educators.

### Step 2: Understanding Repository Basics

A **repository** (repo) is like a project folder that contains:
- Your LiaScript files
- Images, videos, and other assets
- Version history of all changes
- Collaboration tools

### Step 3: Creating Your First Repository

1. Click the "+" icon in the top right corner
2. Select "New repository"
3. Choose a descriptive name: `intro-to-research-methods`
4. Add a description: "Interactive course materials for Research Methods 101"
5. Make it **Public** (for GitHub Pages compatibility)
6. Initialize with a README
7. Click "Create repository"

---

## Creating Your First LiaScript File

### Step 1: Basic File Structure

LiaScript files use the `.md` extension. Let's create `lesson-1.md`:

```markdown
<!--
author: Dr. Jane Smith
email: jane.smith@university.edu
version: 1.0.0
language: en
narrator: US English Female

comment: This is an introduction to research methods using LiaScript

link: https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css
script: https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js
-->

# Research Methods 101: Introduction

Welcome to our interactive research methods course!

## Learning Objectives

After this lesson, you will understand:

- [x] What research methods are
- [ ] Different types of research approaches
- [ ] How to formulate research questions

## What is Research?

Research is the systematic investigation of a topic to discover facts, test hypotheses, or develop new knowledge.

### Quick Quiz

What is the primary goal of research?

[( )] To prove existing theories
[( )] To challenge professors
[(X)] To discover new knowledge
[( )] To complete assignments

### Research Types

``` ascii
Scientific Research
├── Quantitative
│   ├── Experimental
│   └── Survey
└── Qualitative
    ├── Ethnographic
    └── Case Study
```

## Interactive Example: Hypothesis Formation

Let's practice creating a research hypothesis!

**Research Question:** Does coffee consumption affect student performance?

**Your Hypothesis:**

[[hypothesis]]

**Explanation:**

[hypothesis](A good hypothesis might be: "Students who consume moderate amounts of coffee will show improved test scores compared to those who consume no coffee or excessive amounts.")

## Summary

Research methods provide the foundation for generating reliable knowledge. In our next lesson, we'll explore specific methodological approaches.

---

**Navigation:**
- Previous: [Course Introduction](README.md)
- Next: [Lesson 2: Research Design](lesson-2.md)
```

### Step 2: Understanding LiaScript Syntax

**Headers and Navigation:**
- Use `#` for main headings (become slides)
- Use `##` and `###` for subsections

**Interactive Elements:**
- `[( )] Option` - Single choice quiz
- `[(X)] Correct Answer` - Correct option
- `[[input_field]]` - Text input
- `[x]` - Completed checklist item
- `[ ]` - Uncompleted checklist item

**Multimedia:**
- Images: `![alt text](image.png)`
- Audio: `?[audio description](audio.mp3)`
- Videos: `!?[video description](video.mp4)`

### Step 3: Uploading Your File

1. In your repository, click "Add file" → "Create new file"
2. Name it `lesson-1.md`
3. Paste your LiaScript content
4. Scroll down to "Commit new file"
5. Add a commit message: "Add first lesson on research methods"
6. Click "Commit new file"

---

## Advanced LiaScript Features

### Mathematical Formulas

LiaScript supports LaTeX math rendering:

```markdown
The correlation coefficient is calculated as:

$$r = \frac{\sum_{i=1}^{n}(x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum_{i=1}^{n}(x_i - \bar{x})^2 \sum_{i=1}^{n}(y_i - \bar{y})^2}}$$
```

### Code Execution

Students can run code directly in the browser:

```markdown
Try this Python code:

```python
import numpy as np
import matplotlib.pyplot as plt

# Generate sample data
data = np.random.normal(100, 15, 1000)

# Create histogram
plt.hist(data, bins=30, alpha=0.7)
plt.title('Sample Distribution')
plt.show()
```
```

### Surveys and Data Collection

```markdown
Please rate your confidence level:

[( )] Very Low
[( )] Low
[( )] Moderate
[( )] High
[( )] Very High

Additional comments:

[[feedback]]
```

### Audio Narration

Add the `narrator` property in your header to enable text-to-speech:

```markdown
<!--
narrator: US English Female
-->

# This content will be read aloud!

Click the speaker icon to hear the narration.
```

---

## Publishing with GitHub Pages

### Step 1: Enable GitHub Pages

1. Go to your repository
2. Click "Settings" tab
3. Scroll to "Pages" section
4. Under "Source," select "Deploy from a branch"
5. Choose "main" branch
6. Click "Save"

### Step 2: Access Your Content

Your LiaScript content will be available at:
`https://yourusername.github.io/repository-name/filename.md`

**But wait!** GitHub Pages serves raw Markdown. To render LiaScript properly:

### Step 3: Using LiaScript's CDN

Access your content through LiaScript's viewer:
`https://liascript.github.io/course/?https://yourusername.github.io/repository-name/filename.md`

### Step 4: Creating a Custom Domain (Optional)

For a professional URL like `courses.yourname.com`:

1. Purchase a domain
2. In repository settings, add your custom domain
3. Configure DNS settings with your provider
4. Enable HTTPS

---

## Collaboration and Version Control

### Working with Colleagues

**Adding Collaborators:**
1. Repository Settings → Manage access
2. Click "Invite a collaborator"
3. Enter their GitHub username or email
4. Set permissions (Read, Write, or Admin)

**Branch Workflow for Course Development:**

```
main branch (published content)
├── development (work-in-progress)
├── feature/new-quiz-module
└── hotfix/typo-corrections
```

### Version Control Best Practices

**Commit Messages:**
- ✅ "Add interactive quiz to Lesson 3"
- ✅ "Fix mathematical formula in statistics section"
- ❌ "Update stuff"
- ❌ "Changes"

**File Organization:**
```
repository/
├── README.md (course overview)
├── syllabus.md
├── lessons/
│   ├── lesson-01.md
│   ├── lesson-02.md
│   └── ...
├── resources/
│   ├── images/
│   ├── videos/
│   └── datasets/
└── assignments/
    ├── assignment-01.md
    └── ...
```

### Using Issues and Discussions

**Issues** - Track bugs, improvements, and tasks:
- "Add more examples to statistical analysis lesson"
- "Video not loading in Lesson 5"
- "Request: Interactive timeline for history course"

**Discussions** - Engage with students and colleagues:
- Q&A about course content
- Feature requests
- General course announcements

---

## Best Practices for Academic Content

### Content Structure

**Start with Clear Objectives:**
```markdown
## Learning Objectives

By the end of this lesson, you will be able to:
- Define key concepts
- Apply theoretical frameworks
- Analyze case studies
```

**Use Progressive Disclosure:**
- Start with overview
- Build complexity gradually  
- Provide multiple examples
- Include practice opportunities

### Engagement Strategies

**Frequent Interaction:**
- Quiz every 5-7 minutes
- Think-pair-share prompts
- Reflection questions
- Real-world applications

**Multimedia Balance:**
- 60% text content
- 25% interactive elements
- 15% multimedia (images, videos, audio)

### Accessibility Considerations

**Visual:**
- Use high contrast colors
- Provide alt text for images
- Ensure readable font sizes

**Cognitive:**
- Break content into chunks
- Provide clear navigation
- Include progress indicators
- Offer multiple content formats

### Assessment Integration

```markdown
### Knowledge Check

Which research method is best for exploring a new phenomenon?

[( )] Quantitative survey
[( )] Experimental design
[(X)] Qualitative exploration
[( )] Meta-analysis

**Explanation:** When little is known about a topic, qualitative methods help researchers understand the complexity and nuances before developing structured measurements.
```

---

## Troubleshooting Common Issues

### Problem 1: Content Not Displaying Properly

**Symptoms:** Raw Markdown showing instead of interactive content

**Solution:** Ensure you're accessing content through LiaScript viewer:
`https://liascript.github.io/course/?[YOUR-GITHUB-PAGES-URL]`

### Problem 2: Images Not Loading

**Symptoms:** Broken image icons

**Solutions:**
1. Check image paths (case-sensitive)
2. Ensure images are uploaded to repository
3. Use relative paths: `![description](./images/chart.png)`

### Problem 3: Math Formulas Not Rendering

**Symptoms:** Raw LaTeX code visible

**Solutions:**
1. Wrap inline math in `$...$`
2. Wrap block math in `$$...$$`
3. Escape special characters if needed

### Problem 4: Audio/Video Issues

**Common Issues and Fixes:**
- File format compatibility (use MP3 for audio, MP4 for video)
- File size limits (keep under 100MB)
- HTTPS requirements for embedded content

### Problem 5: Collaboration Conflicts

**Symptoms:** Merge conflicts when multiple people edit

**Prevention:**
1. Communicate about who's editing what
2. Use branches for major changes
3. Pull latest changes before starting work
4. Make frequent, small commits

---

## Resources and Next Steps

### Essential Links

**LiaScript Documentation:**
- Official Guide: [liascript.github.io](https://liascript.github.io)
- Syntax Reference: [github.com/liaScript/docs](https://github.com/liaScript/docs)
- Example Courses: [github.com/liaScript/courses](https://github.com/liaScript/courses)

**GitHub Resources:**
- GitHub Education: [education.github.com](https://education.github.com)
- Git Handbook: [guides.github.com/introduction/git-handbook](https://guides.github.com/introduction/git-handbook)
- Markdown Guide: [guides.github.com/features/mastering-markdown](https://guides.github.com/features/mastering-markdown)

### Community Support

**Forums and Help:**
- LiaScript Discussions: GitHub Discussions on LiaScript repo
- Academic GitHub Community: [github.com/education/community](https://github.com/education/community)
- Stack Overflow: Tag your questions with `liascript` and `github-pages`

### Advanced Learning Paths

**Next Steps:**
1. **Custom Styling:** Learn CSS to brand your courses
2. **Advanced Interactions:** Integrate external APIs and databases
3. **Analytics:** Track student engagement and progress
4. **Mobile Optimization:** Ensure excellent mobile experience
5. **Automated Deployment:** Set up CI/CD for course updates

### Course Template Repository

Create a template for quick course setup:

```markdown
template-repository/
├── README.md (setup instructions)
├── course-info.md (syllabus template)
├── lesson-template.md
├── resources/
│   ├── style.css
│   └── images/
├── assignments/
│   └── assignment-template.md
└── .github/
    └── workflows/
        └── deploy.yml (auto-deployment)
```

---

## Conclusion

Congratulations! You've completed the LiaScript and GitHub integration module. You now have the knowledge and tools to:

- Create engaging, interactive educational content
- Collaborate effectively with colleagues
- Publish professional-looking courses
- Maintain version control of your educational materials

### Your Action Plan

**Week 1:** Set up your first repository and create a simple lesson
**Week 2:** Add interactive elements and multimedia content  
**Week 3:** Publish using GitHub Pages and gather feedback
**Week 4:** Collaborate with colleagues and refine your content

### Final Thoughts

The combination of LiaScript and GitHub provides a powerful, free platform for creating world-class educational content. Start small, experiment often, and don't hesitate to reach out to the community for support.

**Happy teaching and learning! 🚀**

---

*This module was created with ❤️ for the academic community. Feel free to adapt, share, and improve upon it.*

---

**License:** Creative Commons Attribution 4.0 International  
**Last Updated:** September 2025  
**Version:** 1.0