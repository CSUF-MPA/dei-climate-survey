# dei-climate-survey

# DEI Faculty Climate Survey

## Overview

This repository hosts an anonymous, **fully accessible** climate survey for faculty in the Public Administration department. The survey is designed to assess departmental climate, diversity, equity, inclusion, and belonging (DEIB) efforts, experiences with discrimination, and professional support within the department.

## Purpose

The survey aims to:

- Gather honest feedback about departmental climate and culture
- Identify areas of strength and opportunities for improvement
- Assess faculty experiences with DEIB initiatives
- Understand professional development and support needs
- Foster a more inclusive and supportive academic environment

## Accessibility Features

This survey is **100% accessibility compliant** and meets WCAG 2.1 AA standards:

### ✅ **Universal Design**
- Semantic HTML5 structure with proper landmarks (`<main>`, `<section>`, `<header>`)
- Skip-to-content link for keyboard navigation
- Logical heading hierarchy (h1 → h2)
- Screen reader optimized

### ✅ **Form Accessibility**
- `<fieldset>` and `<legend>` elements for question grouping
- Proper `<label>` associations for all form controls
- ARIA attributes (`role="radiogroup"`, `aria-required`, `aria-describedby`)
- Clear required field indicators with proper labeling
- Error message containers with `role="alert"`

### ✅ **Visual & Motor Accessibility**
- High contrast color scheme (#1a1a1a text on white background)
- Increased font sizes (18px base, larger headings)
- Minimum 48px touch targets for mobile accessibility
- Enhanced focus indicators with 3px visible outlines
- Hover states for better interactivity feedback

### ✅ **Assistive Technology Support**
- Screen reader only text with `.sr-only` class
- Comprehensive ARIA labels and descriptions
- Form instructions provided via `aria-describedby`
- Proper radio button grouping with `role="radiogroup"`

### ✅ **User Preferences**
- High contrast mode support (`@media (prefers-contrast: high)`)
- Reduced motion support (`@media (prefers-reduced-motion: reduce)`)
- Responsive design for all screen sizes
- No JavaScript required (works with any browser configuration)

## Survey Sections

The survey consists of four main sections with Likert scale questions and open-ended responses:

1. **General Climate & Belonging** (5 questions)
   - Comfort sharing perspectives
   - Voice in faculty meetings
   - Value of contributions
   - Fear of retaliation
   - Department community support

2. **Diversity, Equity & Inclusion Culture** (6 questions)
   - Department DEIB values
   - Recognition of DEIB achievements
   - Faculty diversity satisfaction
   - Leadership diversity
   - Access to DEIB training

3. **Experiences of Discrimination & Exclusion** (4 questions)
   - Confidence intervening against bias
   - Reporting mechanisms knowledge
   - Trust in investigation processes
   - Personal discrimination experiences

4. **Professional Support & Development** (5 questions)
   - Collaboration opportunities
   - Professional development support
   - Work-life balance
   - Scheduling preferences
   - Service workload equity

5. **Open-Ended Questions** (4 questions)
   - Assigned time positions
   - Teaching opportunities
   - Inclusion best practices
   - Improvement suggestions

## Technical Details

### Hosting

- **Platform**: GitHub Pages
- **File**: `index.html`
- **URL**: `https://CSUF-MPA.github.io/dei-climate-survey/`
- **Accessibility**: WCAG 2.1 AA compliant
- **Browser Support**: All modern browsers with full accessibility features

### Form Submission

- **Service**: Formspree
- **Endpoint**: `https://formspree.io/f/xnngwgrb`
- **Method**: Anonymous submission (no IP tracking)
- **Data Collection**: All responses are sent to the configured email address

### Browser Compatibility

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile responsive design with accessibility features
- Screen reader compatible (NVDA, JAWS, VoiceOver, TalkBack)
- High contrast mode support
- Keyboard navigation optimized
- No JavaScript required (pure HTML/CSS)

### Accessibility Testing

The survey has been tested with:
- **Screen readers**: NVDA, JAWS, VoiceOver
- **Keyboard navigation**: Full tab order and focus management
- **Color contrast**: AAA level compliance
- **Mobile accessibility**: Touch target sizes and responsive design
- **Browser zoom**: Up to 200% zoom level support

## Setup Instructions

1. **Fork or download this repository**

   ```bash
   git clone https://github.com/CSUF-MPA/dei-climate-survey.git
   ```

2. **Rename the survey file for GitHub Pages**

   ```bash
   mv dei_climate_survey.html index.html
   ```

3. **Enable GitHub Pages**
   - Go to Settings → Pages
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click Save

4. **Access your survey**
   - Survey will be available at: `https://CSUF-MPA.github.io/dei-climate-survey/`
   - Share this link with faculty members

## Privacy & Anonymity

- ✅ **No personal information collected**
- ✅ **No IP addresses tracked**
- ✅ **No cookies or browser storage used**
- ✅ **SSL encryption via GitHub Pages HTTPS**
- ✅ **Responses sent directly to Formspree**

## Data Management

### Receiving Responses

- Responses are emailed to the address configured in Formspree
- Each submission includes timestamp and all survey responses
- Data can be exported from Formspree dashboard

### Best Practices

1. Download and backup responses regularly
2. Store data securely and limit access
3. Aggregate results before sharing to maintain anonymity
4. Delete individual responses after analysis if needed
5. Follow institutional IRB guidelines if applicable

## Customization

### Modifying Questions

Edit the `index.html` file to update questions. Each Likert question follows this **accessible** structure:

```html
<fieldset class="question-fieldset">
    <legend class="question-legend">
        Your question here
        <span class="required-indicator" aria-label="required">*</span>
    </legend>
    <div class="likert-scale" role="radiogroup" aria-required="true">
        <div class="likert-option">
            <input type="radio" id="unique_id" name="question_name" value="Option" required>
            <label for="unique_id">Option Text</label>
        </div>
        <!-- Additional options -->
    </div>
    <div id="error-id" class="error-message" role="alert"></div>
</fieldset>
```

### Accessibility Requirements When Customizing

When modifying the survey, maintain accessibility by:

1. **Always use proper `<fieldset>` and `<legend>` for question groups**
2. **Ensure unique IDs for all form controls**
3. **Maintain proper `<label>` associations**
4. **Keep ARIA attributes intact**
5. **Test with keyboard navigation after changes**
6. **Verify color contrast meets AA standards**
7. **Ensure touch targets remain 48px minimum**

### Styling Changes

CSS is embedded in the `<style>` section with accessibility features:

- **Color contrast**: Text color `#1a1a1a` ensures AAA compliance
- **Focus indicators**: 3px outlines for keyboard navigation
- **Touch targets**: Minimum 48px for mobile accessibility
- **Font sizes**: 18px base for better readability
- **Motion**: Respects `prefers-reduced-motion` setting

### Changing Form Endpoint

To use your own Formspree endpoint:

1. Sign up at [Formspree.io](https://formspree.io)
2. Create a new form
3. Replace the action URL in the HTML:

   ```html
   <form action="https://formspree.io/f/YOUR-FORM-ID" method="POST">
   ```

## Testing

Before deploying, test for both functionality and accessibility:

### Functional Testing
1. Test all radio buttons and text areas
2. Submit a test response
3. Verify receipt of test submission
4. Check mobile responsiveness
5. Test in multiple browsers

### Accessibility Testing
1. **Keyboard navigation**: Tab through entire form
2. **Screen reader**: Test with at least one screen reader
3. **Color contrast**: Verify with contrast checking tools
4. **Zoom test**: Ensure usability at 200% zoom
5. **Focus indicators**: Verify all interactive elements have visible focus
6. **Form validation**: Test error messages with assistive technology

### Recommended Testing Tools
- **axe DevTools**: Browser extension for accessibility auditing
- **WAVE**: Web accessibility evaluation tool
- **Lighthouse**: Built-in Chrome accessibility audit
- **Keyboard**: Navigate entire form using only Tab, Enter, and arrow keys
- **Screen reader**: NVDA (free), VoiceOver (Mac), or TalkBack (Android)

## Support & Maintenance

### Common Issues

- **Form not submitting**: Check Formspree endpoint is active
- **Styling issues**: Clear browser cache
- **404 error**: Ensure file is named `index.html` and GitHub Pages is enabled

### Accessibility Maintenance

- **Regular audits**: Run accessibility tests quarterly
- **User feedback**: Provide contact for accessibility concerns
- **Updates**: Test accessibility after any content changes
- **Training**: Ensure content editors understand accessibility requirements

### Updates

- Survey questions can be updated anytime by editing the HTML
- Changes typically appear within 5-10 minutes on GitHub Pages
- No need to reconfigure Formspree for content changes

## Compliance Statement

This survey meets the following accessibility standards:

- **WCAG 2.1 Level AA**: Web Content Accessibility Guidelines
- **Section 508**: U.S. federal accessibility requirements
- **ADA Title III**: Americans with Disabilities Act compliance
- **EN 301 549**: European accessibility standard

## License

This survey template is provided as-is for academic use. Feel free to modify and adapt for your institution's needs.

## Acknowledgments

Created for the Public Administration department faculty climate assessment initiative with full accessibility compliance to ensure equal access for all faculty members.

---

**Accessibility Note**: This survey is designed to be fully accessible to users with disabilities. If you encounter any accessibility barriers, please contact [accessibility-contact@institution.edu] for assistance.

**Participation Note**: This survey is designed to collect anonymous feedback. Please ensure all faculty understand that participation is voluntary and responses cannot be traced back to individuals.
