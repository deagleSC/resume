# LaTeX Resume Template

A clean, professional, and ATS-friendly LaTeX resume template for full-stack developers.

## Overview

This resume template is designed to create a polished, single-page resume that is both human-readable and ATS (Applicant Tracking System) friendly. It features a clean layout with well-organized sections for education, experience, projects, and technical skills.

## Features

- **ATS-Friendly**: Configured with proper PDF encoding and machine-readable formatting
- **Clean Layout**: Professional single-page design with optimized margins
- **Customizable**: Easy-to-use LaTeX commands for consistent formatting
- **Font Options**: Multiple font choices available (commented in the template)
- **Hyperlinks**: Clickable links for email, website, LinkedIn, and GitHub

## Requirements

To compile this resume, you need:

- A LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Required LaTeX packages (most are standard):
  - `article` (document class)
  - `fullpage`
  - `titlesec`
  - `marvosym`
  - `color` / `xcolor`
  - `enumitem`
  - `hyperref`
  - `fancyhdr`
  - `babel`
  - `tabularx`

## Usage

1. **Clone or download** this repository

2. **Edit** `full-stack.tex` with your information:
   - Update the heading section with your name and contact details
   - Fill in your education details
   - Add your work experience
   - List your projects
   - Update your technical skills

3. **Compile** the LaTeX file:
   ```bash
   pdflatex full-stack.tex
   ```

   Or use your preferred LaTeX editor (Overleaf, TeXShop, TeXstudio, etc.)

4. **View** the generated PDF

## Template Structure

### Custom Commands

The template includes several custom commands for consistent formatting:

- `\resumeItem{text}` - Bullet point item
- `\resumeSubheading{title}{dates}{company}{location}` - Work/education entry
- `\resumeSubSubheading{title}{dates}` - Sub-entry
- `\resumeProjectHeading{title}{link}` - Project entry
- `\resumeSubHeadingListStart` / `\resumeSubHeadingListEnd` - List containers

### Sections

1. **Heading**: Name and contact information (email, phone, website, LinkedIn, GitHub)
2. **Education**: Academic background
3. **Experience**: Work history with detailed bullet points
4. **Projects**: Personal or professional projects
5. **Technical Skills**: Programming languages, frameworks, and tools

## Customization

### Changing Fonts

Uncomment one of the font options in the template (lines 24-33):

```latex
% sans-serif options:
% \usepackage[sfdefault]{FiraSans}
% \usepackage[sfdefault]{roboto}
% \usepackage[sfdefault]{noto-sans}
% \usepackage[default]{sourcesanspro}

% serif options:
% \usepackage{CormorantGaramond}
% \usepackage{charter}
```

### Adjusting Margins

Modify the margin settings (lines 42-47) to fit more or less content:

```latex
\addtolength{\oddsidemargin}{-0.5in}
\addtolength{\evensidemargin}{-0.5in}
\addtolength{\textwidth}{1in}
\addtolength{\topmargin}{-.5in}
\addtolength{\textheight}{1.0in}
```

### Adding Sections

To add new sections, follow the pattern:

```latex
\section{Section Name}
  \resumeSubHeadingListStart
    % Your content here
  \resumeSubHeadingListEnd
```

## Credits

- **Author**: Supratik Chakraborty
- **Based on**: [sb2nov/resume](https://github.com/sb2nov/resume)
- **License**: MIT

## License

MIT License - feel free to use and modify this template for your own resume.

## Tips

- Keep bullet points concise and action-oriented
- Use quantifiable metrics when possible
- Ensure the resume fits on one page
- Test the PDF with ATS systems if applying online
- Keep formatting consistent throughout

---

**Note**: Make sure to update the `glyphtounicode` file reference if you encounter compilation issues. This file is typically included with modern LaTeX distributions for proper PDF encoding.
