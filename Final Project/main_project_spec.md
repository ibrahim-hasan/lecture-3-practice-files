# Project Specification: Event Registration Platform

## 1. Overview

Develop a comprehensive, multi-page event platform for a professional marketing conference. The platform must provide a public-facing interface for users to browse event details, register for sessions, and view resources. The application must be built using HTML, CSS, JavaScript, and jQuery, simulating a real-world company project in a software development team.

## 2. Pages & Features

| Page                | Purpose                                                                 |
|---------------------|-------------------------------------------------------------------------|
| index.html          | Landing page with event overview, hero section, and featured sessions   |
| register.html       | Full registration form with dynamic validation and confirmation         |
| schedule.html       | Day-by-day conference schedule using a table layout                     |
| speakers.html       | Profile grid of speakers with modals or dynamic bios                    |
| resources.html      | Downloads, PDFs, and articles with filtering and accordion sections     |
| faq.html            | Frequently asked questions in toggle format                             |
| confirmation.html   | Thank-you page or success message after submission                      |

## 3. Detailed Page Description

### Home (index.html)
- Navbar + logo
- Hero section with title, CTA to Register
- About the event (1–2 paragraphs)
- Featured sessions (3 cards)
- Scroll-animated FAQ teaser

### Register (register.html)
- Form includes:
  - Name, Email, Phone
  - Radio: Select one session
  - Checkbox: Topics of interest
  - Select menu: Occupation (e.g., Student, Freelancer, Manager)
  - Consent checkbox (Terms & Privacy)
  - Optional message
- Show form summary below upon submit
- Confirm page (confirmation.html) shown after successful registration

### Schedule (schedule.html)
- Use <table> for day-by-day session blocks
- Responsive layout and styled for readability
- Filter by date or session type (using jQuery)

### Speakers (speakers.html)
- Speaker cards: Name, photo, short bio
- “Read More” opens bio in modal (jQuery)
- Filter speakers by category (e.g., Marketing, Tech, Leadership)

### Resources (resources.html)
- List of downloadable files
- Category filtering
- Accordion-style toggle for additional info (with jQuery)

### FAQ (faq.html)
- Accordion-style questions using jQuery
- Search field to live-filter FAQ list

## 4. Technical Requirements

### Frontend
- Semantic HTML5 and ARIA roles
- Responsive design (Flexbox / Grid + media queries)
- Clean and modular CSS (with comments)
- Minimal reset or normalize style at the top

### JavaScript + jQuery
- DOM manipulation and event listeners
- Form validation
- Dynamic DOM rendering (e.g., modals, filtered lists)
- jQuery:
  - .slideToggle(), .fadeIn(), .addClass(), etc.
  - Form handling and UI animations
  - Simulate AJAX calls using JSON and setTimeout

## 5. Styling Requirements

- Consistent design (colors, typography, buttons)
- Responsive navbar and collapsible menu for mobile
- Custom hover and focus states
- Animated transitions (slide/fade)

## 6. Folder Structure

```
event-platform/
├── index.html
├── register.html
├── schedule.html
├── speakers.html
├── resources.html
├── faq.html
├── confirmation.html
├── css/
│   └── style.css
├── js/
│   ├── script.js
│   └── jquery.min.js
├── data/
│   └── sessions.json
└── assets/
    ├── images/
    └── docs/
```

## 7. Evaluation Criteria

| Criterion                        | Weight |
|----------------------------------|--------|
| Semantic HTML Structure          | 10%    |
| Responsive & Accessible Layout   | 15%    |
| CSS Layout, Grid/Flexbox usage   | 15%    |
| JavaScript Logic (Validation, DOM)| 20%    |
| jQuery (Animations, Events)      | 15%    |
| Visual Design & UX Consistency   | 15%    |
| File Structure and Code Comments | 10%    |

## 8. Estimated Timeline

| Week | Focus Areas                                  |
|------|----------------------------------------------|
| 1    | Homepage, Register page, Form validation     |
| 2    | Schedule, Speakers, Resources, Interactivity |