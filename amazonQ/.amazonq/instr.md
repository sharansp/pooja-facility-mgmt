# Project: Pooja Facility Management — Professional Company Website

Act as a senior frontend developer, UI/UX designer, and software architect. Help me build a professional, modern, responsive website for **Pooja Facility Management**.

My current website prototype is:
https://sharansp.github.io/pooja-facility-mgmt/

My planned domain is:
https://poojafacilitymanagement.com/

## 1. Project objectives

Build a professional company website that:
- Presents our facility management services clearly.
- Builds trust with potential customers.
- Generates enquiries and quotation requests.
- Works smoothly on mobile, tablet, laptop, and desktop.
- Has a clean, premium corporate design.
- Can later be extended into a facility management system with customer login, staff management, attendance, work orders, and an admin dashboard.

The immediate priority is the public company website. Do not build the management dashboard in this phase.

## 2. Technology stack

Use the following stack:

- React
- Vite
- JavaScript
- HTML5
- CSS3
- React Router for navigation
- Lucide React for icons
- Git and GitHub for version control

Use functional React components and reusable UI components.

Avoid unnecessary libraries and dependencies. Keep the code easy to understand, maintain, and extend.

If my existing project already has a suitable technology stack, inspect it first and explain whether it should be retained or migrated before making major changes.

## 3. Website pages

Create these six main pages.

### Page 1: Home

Create an attractive homepage containing:

1. Header with company logo, navigation, and a prominent "Request a Quote" button.
2. Hero section with a professional facility management image, a strong headline, supporting text, and two call-to-action buttons.
3. Brief company introduction.
4. Services overview using clean cards with icons and descriptions.
5. Why Choose Us section highlighting verified company strengths.
6. Industries We Serve section.
7. How Our Service Works section.
8. Testimonials or client references only when genuine information is available.
9. Strong enquiry call-to-action section.
10. Professional footer with contact details, navigation links, and social links if available.

Suggested headline:
"Reliable Facility Management for Better-Managed Spaces"

Suggested supporting text:
"Professional facility management solutions designed to help businesses and properties operate smoothly, safely, and efficiently."

Primary CTA: "Request a Quote"

Secondary CTA: "Explore Our Services"

Do not invent company statistics, awards, certifications, customer testimonials, or client logos.

### Page 2: Services

Create a services page with a professional grid layout.

Include relevant service categories such as:
- Housekeeping and cleaning
- Building maintenance
- Electrical and plumbing maintenance
- Security services
- Landscaping and grounds maintenance
- Other facility management services confirmed by the business

Each service card should include:
- Icon or relevant image
- Service name
- Short description
- Benefits
- "Enquire About This Service" button

Only present services that the company actually offers or has confirmed it intends to offer. Mark unconfirmed services as content requiring approval rather than presenting them as established offerings.

Design the page so new services can be added easily.

### Page 3: About Us

Include:
- Company introduction
- Mission and vision
- Core values
- Our approach to facility management
- Leadership or team section, if verified information is available
- Quality, safety, and service commitments

Use a professional layout with appropriate images, clear headings, and readable text.

Do not fabricate employee names, company history, qualifications, or experience.

### Page 4: Industries We Serve

Create a page explaining the customer segments supported by the business.

Possible categories include:
- Corporate offices
- Residential apartments and gated communities
- Commercial buildings
- Educational institutions
- Retail and business spaces
- Industrial facilities

Treat these as proposed categories until the company confirms its actual target markets.

For each category, explain the relevant facility management needs and potential services.

Add a call to action encouraging visitors to request a customised quotation.

### Page 5: Contact Us

Create a professional contact page containing:
- Contact form
- Name
- Company name, optional
- Email address
- Phone number
- Service required
- Property or site type
- Location
- Message
- Privacy acknowledgement where appropriate
- Submit button

Also include verified company contact details, business address, WhatsApp link, and business hours when provided.

Requirements:
- Validate all required fields.
- Show clear validation errors.
- Show loading, success, and failure states.
- Prevent accidental duplicate submissions.
- Make the form accessible by keyboard.
- Do not pretend a message has been sent if no backend or form service is configured.
- Create a clear integration point for a future form service or backend API.
- Never place API secrets in frontend code.

### Page 6: Frequently Asked Questions

Create a clean FAQ page using expandable accordion components.

Cover questions such as:
- What services does Pooja Facility Management provide?
- Which types of properties do you support?
- How can I request a quotation?
- Can services be customised for a property?
- How does the onboarding process work?
- How can I contact your team?

Use truthful, editable answers and mark any answers requiring company confirmation.

Add a final CTA linking to the Contact Us page.

## 4. Design requirements

Use a premium corporate design suitable for a facility management company.

Suggested colour palette:
- Navy blue: #142D4E
- Teal: #168C8C
- White: #FFFFFF
- Light grey: #F3F6FA
- Dark text: #243247

Use:
- Modern, readable typography.
- Consistent spacing and alignment.
- Clean service cards.
- Subtle shadows and borders.
- Rounded corners used consistently.
- Professional facility management photography.
- Simple animations and hover effects.
- Consistent buttons and form styling.
- Clear visual hierarchy.
- Ample whitespace.

Avoid:
- Excessive animations.
- Overly bright colours.
- Cluttered layouts.
- Too many gradients.
- Generic AI-generated text presented as verified business facts.
- Placeholder links that look functional but do nothing.

Make the design look like a professionally developed corporate website rather than a basic student project.

## 5. Responsive design

The website must work properly on:
- Mobile phones
- Tablets
- Laptops
- Large desktop screens

Implement:
- Responsive navigation with a mobile menu.
- Responsive grids and images.
- Readable font sizes at every viewport.
- Touch-friendly buttons.
- Proper spacing on small screens.
- No horizontal overflow.
- Accessible form controls.

Test the main layouts at mobile, tablet, and desktop widths.

## 6. SEO and performance

Implement:
- Unique page titles.
- Meta descriptions for all six pages.
- Semantic HTML.
- Correct heading hierarchy.
- Descriptive image alt text.
- Clean navigation and URLs.
- Social sharing metadata where appropriate.
- Favicon support.
- Sitemap and robots.txt suitable for the production domain.
- Optimised images and lazy loading where appropriate.
- Good accessibility and Core Web Vitals practices.

Do not include unsupported claims in structured data or SEO metadata.

Prepare the website for Google Search Console and Google Analytics, but do not add tracking scripts without clearly identifying the configuration required.

## 7. Code structure

Use a clean, reusable structure similar to:

src/
  assets/
  components/
    Header.jsx
    Footer.jsx
    Button.jsx
    ServiceCard.jsx
    IndustryCard.jsx
    CTASection.jsx
    FAQAccordion.jsx
    ContactForm.jsx
  layouts/
    MainLayout.jsx
  pages/
    Home.jsx
    Services.jsx
    About.jsx
    Industries.jsx
    Contact.jsx
    FAQ.jsx
    NotFound.jsx
  data/
    services.js
    industries.js
    faqs.js
  styles/
    global.css
    variables.css
  App.jsx
  main.jsx

public/
  favicon
  robots.txt
  sitemap.xml

You may adjust the structure if you have a better architectural reason. Keep components reusable and business content separate from presentation where practical.

Use React Router for navigation and ensure direct navigation to each page works with the chosen hosting setup.

## 8. Future dashboard readiness

Prepare the project for future expansion without building the dashboard now.

Keep the public website separate from future authenticated application functionality.

Plan for possible future modules:
- Admin dashboard
- Staff database and staff portal
- Attendance and shift management
- Salary and payroll management
- Customer and property management
- Work orders and maintenance tickets
- Asset management
- Reports and notifications

Do not implement fake login screens or store staff/customer records in browser storage.

Do not build authentication, payroll, or a database in this phase. Provide a short future architecture recommendation describing how these could be added securely.

## 9. Development and quality requirements

Before coding:
1. Inspect the current repository and its files.
2. Identify the existing framework and dependencies.
3. Review the current website and list what should be retained or improved.
4. Explain the implementation plan.
5. Identify any missing company information that must be supplied.

Then implement the website in manageable steps.

After implementation:
- Run the production build.
- Fix compilation errors and warnings.
- Test all six routes.
- Test navigation and responsive layouts.
- Test the contact form's validation and its configured submission behaviour.
- Check images, links, and browser console errors.
- Explain how to run the project locally.
- Explain how to deploy it to GitHub Pages and connect the custom domain.
- List any external services or environment variables that still need configuration.

Do not claim that the website, contact form, domain, or deployment works until it has actually been tested.

## 10. How I want you to work

I am learning web development, so explain the important decisions in beginner-friendly language.

Do not just give me sample snippets or a design description. Work with the files in my existing project and implement the changes where your environment permits.

Do not overwrite the project blindly. Review the existing code first and preserve useful functionality.

Start by inspecting the repository, explaining the current structure, and presenting the implementation plan. Then build and test the website step by step.
