# dei-climate-survey

# DEI Faculty Climate Survey

## Overview

This repository hosts an anonymous climate survey for faculty in the Public Administration department. The survey is designed to assess departmental climate, diversity, equity, inclusion, and belonging (DEIB) efforts, experiences with discrimination, and professional support within the department.

## Purpose

The survey aims to:

- Gather honest feedback about departmental climate and culture
- Identify areas of strength and opportunities for improvement
- Assess faculty experiences with DEIB initiatives
- Understand professional development and support needs
- Foster a more inclusive and supportive academic environment

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
- **File**: `index.html` (rename `dei_climate_survey.html` to `index.html` for GitHub Pages)
- **URL**: `https://[your-username].github.io/[repository-name]/`

### Form Submission

- **Service**: Formspree
- **Endpoint**: `https://formspree.io/f/xnngwgrb`
- **Method**: Anonymous submission (no IP tracking)
- **Data Collection**: All responses are sent to the configured email address

### Browser Compatibility

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile responsive design
- No JavaScript required (pure HTML/CSS)

## Setup Instructions

1. **Fork or download this repository**

   ```bash
   git clone https://github.com/[your-username]/[repository-name].git
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
   - Survey will be available at: `https://[your-username].github.io/[repository-name]/`
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

Edit the `index.html` file to update questions. Each Likert question follows this structure:

```html
<div class="question-group">
    <div class="question-text">Your question here</div>
    <div class="likert-scale">
        <!-- Radio button options -->
    </div>
</div>
```

### Styling Changes

CSS is embedded in the `<style>` section of the HTML file. Key variables:

- Primary colors: `#667eea` and `#764ba2` (gradient)
- Font family: System fonts stack
- Border radius: 10px for containers, 5px for inputs

### Changing Form Endpoint

To use your own Formspree endpoint:

1. Sign up at [Formspree.io](https://formspree.io)
2. Create a new form
3. Replace the action URL in the HTML:

   ```html
   <form action="https://formspree.io/f/YOUR-FORM-ID" method="POST">
   ```

## Testing

Before deploying:

1. Test all radio buttons and text areas
2. Submit a test response
3. Verify receipt of test submission
4. Check mobile responsiveness
5. Test in multiple browsers

## Support & Maintenance

### Common Issues

- **Form not submitting**: Check Formspree endpoint is active
- **Styling issues**: Clear browser cache
- **404 error**: Ensure file is named `index.html` and GitHub Pages is enabled

### Updates

- Survey questions can be updated anytime by editing the HTML
- Changes typically appear within 5-10 minutes on GitHub Pages
- No need to reconfigure Formspree for content changes

## License

This survey template is provided as-is for academic use. Feel free to modify and adapt for your institution's needs.

## Acknowledgments

Created for the Public Administration department faculty climate assessment initiative.

---

**Note**: This survey is designed to collect anonymous feedback. Please ensure all faculty understand that participation is voluntary and responses cannot be traced back to individuals.
