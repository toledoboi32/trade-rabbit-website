# Trade Rabbit Website - Vercel Deployment Guide

## Overview
This is the Trade Rabbit website with integrated AI assistant demo videos. The website showcases an AI-powered platform for home services with professional video demonstrations.

## Files Included
- `index.html` - Main website file
- `package.json` - Project configuration
- `vercel.json` - Vercel deployment configuration
- Video files:
  - `hook_segment.mp4` - Opening hook video
  - `problem_segment.mp4` - Problem setup video
  - `scenario1_segment.mp4` - New customer demo
  - `scenario2_segment.mp4` - Returning customer demo
  - `results_segment.mp4` - Business results video

## Deployment to Vercel

### Method 1: Vercel CLI (Recommended)

1. **Install Vercel CLI** (if not already installed):
   ```bash
   npm install -g vercel
   ```

2. **Login to Vercel**:
   ```bash
   vercel login
   ```

3. **Deploy from the project directory**:
   ```bash
   cd /path/to/trade-rabbit-website
   vercel
   ```

4. **Follow the prompts**:
   - Set up and deploy? **Y**
   - Which scope? Choose your account
   - Link to existing project? **N** (for new deployment)
   - What's your project's name? **trade-rabbit-website**
   - In which directory is your code located? **./** (current directory)

5. **Production deployment**:
   ```bash
   vercel --prod
   ```

### Method 2: Vercel Web Interface

1. **Go to** [vercel.com](https://vercel.com) and sign in
2. **Click "New Project"**
3. **Import from Git** or **Upload files**
4. **If uploading files**: Zip the entire `trade-rabbit-website` folder and upload
5. **Configure project**:
   - Project Name: `trade-rabbit-website`
   - Framework Preset: `Other`
   - Root Directory: `./`
   - Build Command: Leave empty (static site)
   - Output Directory: Leave empty
   - Install Command: Leave empty
6. **Click "Deploy"**

### Method 3: Drag and Drop

1. **Go to** [vercel.com](https://vercel.com) and sign in
2. **Drag and drop** the entire `trade-rabbit-website` folder onto the Vercel dashboard
3. **Wait for deployment** to complete

## Configuration Details

### vercel.json Configuration
The `vercel.json` file is configured for:
- Static file serving
- Proper caching headers for videos and HTML
- Route handling for single-page application

### Video Files
- All video files are optimized for web delivery
- Total size: ~12MB (acceptable for modern web)
- Format: MP4 with web-compatible encoding

## Post-Deployment

After successful deployment, you'll receive:
- **Production URL**: Your live website URL
- **Preview URLs**: For testing before production
- **Analytics**: Available in Vercel dashboard

## Features Included

1. **Professional Design**: Modern, responsive layout
2. **Video Integration**: 5 demo videos showcasing AI assistant capabilities
3. **Mobile Responsive**: Works on all device sizes
4. **Fast Loading**: Optimized for performance
5. **SEO Friendly**: Proper meta tags and structure

## Troubleshooting

### Large File Sizes
If you encounter issues with video file sizes:
- Vercel has a 100MB limit per deployment
- Current total is ~12MB, well within limits
- If needed, videos can be hosted on external CDN

### Build Errors
- This is a static site with no build process
- If errors occur, ensure all files are present
- Check that `vercel.json` is properly formatted

### Domain Configuration
After deployment, you can:
- Add custom domain in Vercel dashboard
- Configure DNS settings
- Set up SSL (automatic with Vercel)

## Support
For deployment issues:
1. Check Vercel documentation
2. Verify all files are uploaded
3. Ensure proper project configuration
4. Contact support if needed

## Live Demo
Once deployed, your website will showcase:
- AI assistant capabilities
- Professional video demonstrations
- Customer testimonials
- Lead capture forms
- Responsive design across all devices

