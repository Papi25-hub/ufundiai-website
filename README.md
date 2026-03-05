# UfundiAI - CAPS & ATP Aligned Teaching Material Generator

🇿🇦 **Proudly South African** | AI-Powered Lesson Planning for Teachers

## 🎯 Project Overview

UfundiAI is a web-based platform that helps South African teachers generate professional, CAPS-aligned teaching materials in seconds. Instead of spending hours on lesson planning, teachers can use our structured, ATP-compliant system to create:

- 📝 **Lesson Plans** - Complete with objectives, activities, and resources
- 📄 **Worksheets** - Print-ready with marking memorandums
- 📊 **PowerPoint Presentations** - Engaging slide decks with visuals
- ✅ **Assessments** - Tests and exams with rubrics and memos

## ✨ Key Features

### 1. **100% CAPS & ATP Aligned**
- Follows the official South African Curriculum and Assessment Policy Statement (CAPS)
- Aligned with Annual Teaching Plans (ATP) week-by-week
- Ensures curriculum compliance across all grades and subjects

### 2. **Structured Selection System**
Unlike free-text search systems, UfundiAI uses a **7-step cascading dropdown approach**:

1. **Phase Selection** - Foundation (R-3), Intermediate (4-6), Senior (7-9), FET (10-12)
2. **Grade Selection** - Specific grade within chosen phase
3. **Subject Selection** - CAPS-approved subjects for that grade
4. **Term Selection** - Term 1, 2, 3, or 4
5. **ATP Week Selection** - Week 1-10 with specific topics
6. **Language Selection** - All 11 official SA languages
7. **Material Type** - Lesson Plan, Worksheet, PPT, or Assessment

### 3. **Multi-Language Support**
Generate materials in all 11 South African official languages:
- English
- Afrikaans
- isiZulu
- isiXhosa
- Sepedi
- Setswana
- Sesotho
- Xitsonga
- siSwati
- Tshivenda
- isiNdebele

### 4. **Smart Topic Preview**
The system shows the exact CAPS topic for the selected week, so teachers know exactly what content will be generated.

## 🏗️ Technical Architecture

### Frontend Stack
- **HTML5** - Semantic structure
- **CSS3** - Custom styling with Poppins font family
- **Vanilla JavaScript** - No framework dependencies
- **Responsive Design** - Mobile-friendly interface

### Data Structure

```javascript
curriculumData = {
  phase: {
    grades: {
      grade-id: {
        name: "Grade Name",
        subjects: ["Subject 1", "Subject 2", ...]
      }
    }
  }
}

atpTopics = {
  "Subject Name": {
    "grade-id": {
      "term-id": {
        "week-id": "CAPS topic for this week"
      }
    }
  }
}
```

### User Flow

```
1. Select Phase → 2. Select Grade → 3. Select Subject
                                    ↓
4. Select Term → 5. Select Week → 6. Select Language
                                    ↓
            7. Choose Material Type → Generate
```

## 📚 CAPS Coverage

### Current Sample Data Includes:
- **Mathematics Grade 5** - All 4 terms, 10 weeks each
- **Natural Sciences Grade 7** - Complete term breakdown
- **Life Sciences Grade 11** - Full ATP coverage

### Phases Covered:
- ✅ Foundation Phase (Grade R-3)
- ✅ Intermediate Phase (Grade 4-6)
- ✅ Senior Phase (Grade 7-9)
- ✅ FET Phase (Grade 10-12)

## 🎨 Design Philosophy

### UI/UX Principles:
1. **Guided Experience** - Cascading dropdowns prevent errors
2. **Visual Feedback** - Clear indicators for active selections
3. **Progressive Disclosure** - Options appear as prerequisites are met
4. **Color Psychology** - Green gradients (trust, growth, education)
5. **Accessibility** - High contrast, clear labels, keyboard navigation

### Why Dropdowns Over Search?
- ✅ **Guaranteed CAPS Compliance** - Can't select non-existent topics
- ✅ **No Typos** - Eliminates spelling errors
- ✅ **ATP Alignment** - Follows exact weekly structure
- ✅ **Reduced Cognitive Load** - Don't need to remember topic names
- ✅ **Better UX** - Clear progression through selections

## 📂 Project Structure

```
ufundiai/
├── index.html              # Main landing page with material generator
├── pricing.html            # Dedicated pricing page (accessed via nav)
├── faq.html               # Comprehensive FAQ page (accessed via Product menu)
├── ai-limitations.html    # AI limitations & best practices (accessed via Product menu)
├── login.html              # User login page
├── signup.html             # User registration page
└── README.md              # This file
```

## 📄 Page Overview

### index.html - Landing Page (Decluttered)
The main landing page focuses on the core value proposition:
- **Hero Section** - Material generator with 7-step dropdown system
- **Features Section** - Key benefits and features
- **Worksheets Examples** - Sample materials showcase
- **CTA Section** - Call to action
- **Export Options** - PowerPoint, Google Slides, PDF
- **Unique Content** - Sample worksheet preview
- **Teacher Reviews** - Social proof from SA teachers
- **Feedback CTA** - User feedback collection

**Note:** Pricing and FAQ sections have been removed from the landing page to reduce clutter. Users can access them via navigation.

### pricing.html - Pricing Page
Dedicated page for pricing information:
- Monthly/Yearly toggle
- Three pricing tiers (Free, Pro, Schools)
- Feature comparison
- FAQ specific to pricing/subscriptions

### faq.html - FAQ Page
Comprehensive FAQ organized by categories:
- Getting started
- Features & planning
- Curriculum support
- Pricing & trials
- Security & compliance
- Contact form footer

### ai-limitations.html - AI Guide
Educational page explaining:
- AI as assistant philosophy
- What AI does best
- AI limitations
- Best practices for teachers

## 🧭 Navigation Structure

The website features a clean navigation with a dropdown "Product" menu:

**Main Navigation:**
- Features (scrolls to #features on landing page)
- Examples (scrolls to #worksheets on landing page)  
- Pricing → **Links to pricing.html**
- **Product** (dropdown menu)
  - FAQ → **Links to faq.html**
  - AI Limitations & Best Practices → **Links to ai-limitations.html**

This structure keeps the landing page focused on conversion while providing easy access to detailed information through separate pages.

## 🚀 Features Implementation Status

### ✅ Completed Features
- [x] Phase-based grade organization
- [x] Cascading dropdown system
- [x] ATP week-by-week selection
- [x] Topic preview display
- [x] Material type selector (4 types)
- [x] All 11 SA language options
- [x] Responsive design
- [x] Sample ATP data for 3 subjects
- [x] Generate button with validation
- [x] Loading states and feedback
- [x] Login/Signup pages (Chalkie-inspired)
- [x] Dedicated pricing page with monthly/yearly toggle
- [x] Three-tier pricing structure (Free, Pro, Schools)
- [x] Comprehensive FAQ page
- [x] AI Limitations & Best Practices guide
- [x] Dropdown navigation menu
- [x] Teacher review section
- [x] Export options showcase (PPT, Google Slides, PDF)
- [x] Social media links (Facebook, Instagram, TikTok, LinkedIn)
- [x] Professional "Righteous" font for branding
- [x] Differentiation options for worksheets

### 🔄 In Progress
- [ ] Backend API integration
- [ ] Complete ATP database for all subjects/grades
- [ ] Actual material generation (AI integration)
- [ ] Save/download generated materials

### 📋 Planned Features
- [ ] Material preview before download
- [ ] Edit generated content
- [ ] Save to personal library
- [ ] Share materials with colleagues
- [ ] School admin dashboard
- [ ] Usage analytics
- [ ] Curriculum update notifications
- [ ] Custom topic addition (reviewed by admin)

## 🤖 AI Philosophy: Assistant, Not Replacement

UfundiAI is designed with a clear philosophy: **AI should assist teachers, not replace them**.

### What UfundiAI Does Best:
- ✅ Automates time-consuming administrative tasks
- ✅ Generates curriculum-aligned starting points
- ✅ Provides professional formatting
- ✅ Ensures CAPS & ATP compliance
- ✅ Supports differentiation

### What Teachers Bring:
- 💡 Knowledge of their specific learners
- ❤️ Personal connection and empathy
- 🎯 Contextual adaptation and customization
- 🌟 Creative teaching approaches
- 🔍 Professional judgment and expertise

### Best Practices:
1. Always review generated materials
2. Personalize content for your class
3. Adapt examples to local context
4. Use as a professional first draft
5. Combine with your pedagogical expertise

For detailed information, see the [AI Limitations & Best Practices](ai-limitations.html) page.

## 🎓 Educational Alignment

### CAPS Compliance
All materials generated follow:
- ✅ Content specification per grade
- ✅ Cognitive level requirements
- ✅ Assessment standards
- ✅ Time allocation guidelines
- ✅ Resource recommendations

### ATP Integration
- Week-by-week topic breakdown
- Term pacing guides
- Assessment scheduling
- Revision periods
- Exam preparation coverage

## 💡 Usage Example

**Scenario**: Grade 7 teacher needs a worksheet on Food Chains for Term 3, Week 6

**Steps**:
1. Select **Senior Phase** (Grade 7-9)
2. Select **Grade 7**
3. Select **Natural Sciences**
4. Select **Term 3**
5. Select **Week 6** → Topic auto-displays: "Food chains and food webs"
6. Select **English** (or any other language)
7. Click **Worksheet** button
8. Click **Generate Material**
9. Download ready-to-print worksheet with memo

**Time saved**: From 2-3 hours → 30 seconds! ⚡

## 🔒 Future Enhancements

### Technical
- RESTful API backend
- Database for ATP data
- AI integration (GPT/Claude for generation)
- PDF generation and export
- Cloud storage integration

### Educational
- Differentiation levels (support/extension)
- IEB curriculum support
- Vocational subject coverage
- Special education adaptations
- Parent communication materials

### Business
- Subscription tiers (Free, Educator, School)
- Department of Education partnerships
- Teacher training resources
- Community sharing platform

## 📊 Curriculum Data Expansion

To make this production-ready, we need to expand the ATP topics database:

**Current Status**: 3 subjects × 3 grades × 4 terms × 10 weeks = ~120 topics

**Target**: 15+ subjects × 13 grades × 4 terms × 10 weeks = **7,800+ topics**

This comprehensive database would cover:
- All CAPS subjects across all grades
- Week-by-week learning outcomes
- Assessment tasks per term
- Resource requirements
- Cognitive level distribution

## 🤝 Contributing

This is a proof-of-concept demonstrating the structured approach to CAPS-aligned material generation. The actual ATP database would need to be:

1. Verified by CAPS curriculum experts
2. Updated annually per DBE guidelines
3. Reviewed by subject matter teachers
4. Aligned with latest policy documents

## 📞 Contact & Support

For more information about implementing UfundiAI in your school or district, contact us through the website.

## 📄 License

© 2026 UfundiAI. All rights reserved.

---

**Made with ❤️ for South African Teachers 🇿🇦**

*"Making lesson planning something teachers fall in love with"*
