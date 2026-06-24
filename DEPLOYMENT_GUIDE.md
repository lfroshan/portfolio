# Portfolio Website - Deployment Guide

## Navigation Structure - All Relative Paths ✅

### Main Portfolio (index.html)

- **Navbar Links**: All use anchor links (#about, #experience, etc.)
- **Blog Card 1**: `blogs/contents/blog-powerapps-ai.html`
- **Blog Card 2**: `blogs/contents/blog-powerplatform-procode.html`
- **View All Blogs Button**: `blogs/index.html`

### Blogs Index (blogs/index.html)

- **Logo/Home**: `../index.html` (back to main portfolio)
- **Blog Card 1**: `contents/blog-powerapps-ai.html`
- **Blog Card 2**: `contents/blog-powerplatform-procode.html`

### Blog Content Pages (blogs/contents/blog-\*.html)

- **Home Breadcrumb**: `../../index.html` (back to main portfolio)
- **Blogs Breadcrumb**: `../index.html` (back to blogs index)
- **Stylesheet**: `../../style.css`

## Deployment Compatibility

### ✅ Works on Both Domains:

1. **Local Development**
   - `file:///Users/roshanshrestha/Documents/portfolio/index.html`
   - All relative paths work correctly

2. **GitHub Pages**
   - Base URL: `https://lfroshan.github.io/portfolio/`
   - Relative paths automatically resolve with the base URL
   - No hardcoded paths needed

3. **Custom Domain**
   - Base URL: `https://roshanshrestha394.com.np/`
   - Relative paths work seamlessly
   - No hardcoded paths needed

## Testing Checklist ✅

- [x] Main page navbar navigation working
- [x] Blog section links navigate to correct pages
- [x] "View All Blogs" button works
- [x] Blog cards are clickable
- [x] Breadcrumb navigation in blog posts works
- [x] Back-to-home navigation works
- [x] No hardcoded URLs (except external links)
- [x] All paths are relative (portable)

## No Changes Needed For:

- ✅ style.css - No path issues found
- ✅ script.js - All functionality working (no hardcoded paths)
- ✅ Responsive navbar toggle - Working correctly
- ✅ Smooth scrolling - Enabled via CSS
- ✅ Intersection observer for reveal animations - Active

## Deployment Steps

1. Ensure all files maintain the current folder structure:

   ```
   index.html
   style.css
   script.js
   blogs/
     index.html
     contents/
       blog-powerapps-ai.html
       blog-powerplatform-procode.html
   ```

2. Deploy to chosen domain (no modifications needed)

3. Test all navigation links on the deployed site

## Notes

- All external links (email, LinkedIn, GitHub) use absolute URLs ✓
- All internal navigation uses relative paths ✓
- Website is fully portable between environments ✓
