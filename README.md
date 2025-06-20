# Portfolio Website Maintenance Guide

## Overview

This document provides comprehensive instructions for maintaining and updating your GitHub Pages portfolio website. The site is built with Jekyll and automatically deploys from your GitHub repository.

## Repository Information

- **Repository**: https://github.com/ralphwarrand/portfolio
- **Live Site**: https://ralphwarrand.github.io/portfolio/
- **Framework**: Jekyll (GitHub Pages compatible)
- **Theme**: Custom responsive design based on Minima

## Site Structure

```
portfolio/
├── _config.yml          # Site configuration
├── _layouts/            # Page templates
│   ├── home.html       # Homepage layout
│   └── project.html    # Project page layout
├── _projects/          # Project pages (Year 2 blocks)
│   ├── y2a.md         # Year 2 Block A
│   ├── y2b.md         # Year 2 Block B
│   ├── y2c.md         # Year 2 Block C
│   └── y2d.md         # Year 2 Block D
├── assets/images/      # All extracted images
├── contact.md          # Contact page
├── index.md           # Homepage content
├── Gemfile            # Ruby dependencies
└── README.md          # This documentation
```

## Adding New Year/Block Content

### Method 1: Using PowerPoint Extraction (Recommended)

1. **Prepare your PowerPoint files**
   - Save your learning logs as `.pptx` files
   - Name them consistently (e.g., `Y3A.pptx`, `Y3B.pptx`)

2. **Extract content using the provided script**
   ```bash
   # Update the script with new file paths
   python3 extract_pptx_data.py
   ```

3. **Generate new project pages**
   ```bash
   # Update the script to include new blocks
   python3 create_project_pages.py
   ```

4. **Copy images to assets**
   ```bash
   cp extracted_pptx_data/Y3A/*.png assets/images/
   cp extracted_pptx_data/Y3A/*.jpg assets/images/
   ```

### Method 2: Manual Creation

1. **Create a new project file**
   - Create `_projects/y3a.md` (or appropriate name)
   - Use the existing project files as templates

2. **Follow the front matter format**
   ```yaml
   ---
   layout: project
   title: "Year 3 Block A - [Your Focus Area]"
   period: "[Start Date] - [End Date]"
   tags: ["Tag1", "Tag2", "Tag3"]
   ---
   ```

3. **Add your content using Markdown**
   - Use the same structure as existing projects
   - Include sections for Overview, Goals, Progress, Reflection

## Updating Existing Content

1. **Edit project files directly**
   - Navigate to `_projects/` folder
   - Edit the relevant `.md` file
   - Use Markdown syntax for formatting

2. **Add new images**
   - Upload images to `assets/images/` folder
   - Reference them in your content: `![Description]({{ '/assets/images/filename.png' | relative_url }})`

3. **Update contact information**
   - Edit `contact.md` to update your details
   - Modify `_config.yml` for site-wide information

## Deployment Process

The site automatically deploys when you push changes to the `main` branch:

1. **Make your changes locally or via GitHub web interface**

2. **Commit and push changes**
   ```bash
   git add .
   git commit -m "Add Year 3 content"
   git push origin main
   ```

3. **GitHub Pages will automatically rebuild**
   - Usually takes 1-5 minutes
   - Check the Actions tab for build status

## Customization Options

### Changing Colors and Styling

1. **Edit the CSS in layout files**
   - Modify `_layouts/home.html` for homepage styling
   - Modify `_layouts/project.html` for project page styling

2. **Update site configuration**
   - Edit `_config.yml` for site title, description, etc.

### Adding New Page Types

1. **Create new layout in `_layouts/`**
2. **Create content files using the new layout**
3. **Add navigation links if needed**

## Troubleshooting

### Site Not Loading
- Check GitHub Pages settings in repository settings
- Verify the site is enabled and building from `main` branch
- Check the Actions tab for build errors

### Images Not Displaying
- Ensure images are in `assets/images/` folder
- Use relative URLs: `{{ '/assets/images/filename.png' | relative_url }}`
- Check file extensions match exactly

### Layout Issues
- Validate your Markdown syntax
- Check front matter formatting (YAML)
- Ensure proper indentation in YAML

## Best Practices

1. **Consistent Naming**
   - Use lowercase for file names
   - Use hyphens instead of spaces
   - Follow existing naming conventions

2. **Image Optimization**
   - Compress large images before uploading
   - Use appropriate formats (PNG for screenshots, JPG for photos)
   - Consider file size limits (GitHub recommends <50MB per file)

3. **Content Organization**
   - Keep project files focused and concise
   - Use clear headings and sections
   - Include relevant tags for categorization

4. **Regular Updates**
   - Update content regularly as you progress
   - Keep contact information current
   - Archive or reorganize old content as needed

## Future Enhancements

Consider these improvements for your portfolio:

1. **Blog Section**
   - Add `_posts/` folder for blog entries
   - Create blog layout and index page

2. **Project Galleries**
   - Implement image galleries for projects
   - Add lightbox functionality for images

3. **Search Functionality**
   - Add search capability for projects
   - Implement tag-based filtering

4. **Analytics**
   - Add Google Analytics for visitor tracking
   - Monitor popular content and pages

## Support and Resources

- **Jekyll Documentation**: https://jekyllrb.com/docs/
- **GitHub Pages Documentation**: https://docs.github.com/en/pages
- **Markdown Guide**: https://www.markdownguide.org/
- **YAML Syntax**: https://yaml.org/spec/1.2/spec.html

## Contact for Technical Issues

If you encounter technical issues with the site:
1. Check the GitHub repository's Issues tab
2. Review GitHub Pages build logs
3. Consult Jekyll documentation
4. Consider reaching out to web development communities

---

*This documentation was created as part of your portfolio setup. Keep it updated as you make changes to your site structure or workflow.*

