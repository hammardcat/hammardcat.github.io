# Deploying HammerDCat Website with CatDrone to GitHub Pages

This guide will walk you through deploying the HammerDCat flattened stuffed cat and CatDrone conversion website to GitHub Pages.

## Step 1: Create a GitHub Account

If you don't already have a GitHub account:
1. Go to [github.com](https://github.com)
2. Click "Sign Up" in the top-right corner
3. Follow the instructions to create your account
4. Verify your email address when prompted

## Step 2: Create a New Repository

1. After logging into GitHub, click the "+" icon in the top-right corner
2. Select "New repository"
3. Name your repository: `yourusername.github.io`
   - Replace "yourusername" with your actual GitHub username
   - This special name will automatically enable GitHub Pages
4. Make the repository "Public"
5. Click "Create repository"

## Step 3: Upload Your Website Files

1. In your new repository, click the "Add file" button
2. Select "Upload files"
3. Upload these files:
   - `hammerdcat-website-with-catdrone.html` (rename it to `index.html` before uploading)
   - `flattened-cat.svg`
   - `catdrone-conversion.svg`
   - `catdrone-interactive-demo.html`
4. Scroll down and click "Commit changes"

## Step 4: Update Image Links in Your Website

You'll need to update the paths to the SVG images in your website:

1. In your repository, click on the `index.html` file
2. Click the pencil icon to edit it
3. Find these lines (around lines 577 and 703):
   ```html
   <img src="https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/flattened-cat.svg" alt="Flattened Cat"...
   
   <img src="https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/catdrone-conversion.svg" alt="CatDrone Conversion"...
   ```
4. Replace `YOUR_USERNAME` with your GitHub username and `YOUR_REPO` with `yourusername.github.io`
   For example: 
   ```html
   <img src="https://raw.githubusercontent.com/johndoe/johndoe.github.io/main/flattened-cat.svg" alt="Flattened Cat"...
   
   <img src="https://raw.githubusercontent.com/johndoe/johndoe.github.io/main/catdrone-conversion.svg" alt="CatDrone Conversion"...
   ```
5. Scroll down and click "Commit changes"

## Step 5: Create a Navigation Page (Optional but Recommended)

For better organization, you might want to create a simple navigation page that links to both your main website and the interactive CatDrone demo:

1. In your repository, click "Add file" > "Create new file"
2. Name the file: `catdrone-demo.html`
3. Paste the following code:

```html
<!DOCTYPE html>
<html>
<head>
    <title>HammerDCat CatDrone Demo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            margin: 0;
            padding: 40px;
            text-align: center;
        }
        h1 {
            color: #5d4037;
        }
        h1 span {
            color: #ff9800;
        }
        .button {
            display: inline-block;
            background-color: #ff9800;
            color: white;
            padding: 15px 30px;
            margin: 20px 10px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .button:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0,0,0,0.15);
        }
        .description {
            max-width: 600px;
            margin: 0 auto 30px;
            line-height: 1.6;
        }
    </style>
</head>
<body>
    <h1>Hammer<span>DCat</span> Interactive Demos</h1>
    <p class="description">Experience our revolutionary flattened cat and CatDrone technology with these interactive demonstrations!</p>
    
    <a href="index.html" class="button">Main Website</a>
    <a href="catdrone-interactive-demo.html" class="button">CatDrone Flight Simulator</a>
    
    <p>© 2025 HammerDCat. No cats were harmed in our flattening process.</p>
</body>
</html>
```

4. Click "Commit new file"

## Step 6: Verify Your Website Is Live

1. Go to `https://yourusername.github.io` in your browser
2. You should see your HammerDCat website with the flattened cat image and CatDrone section
3. Visit `https://yourusername.github.io/catdrone-interactive-demo.html` to try the interactive CatDrone demo
4. It might take a few minutes for your site to appear

## Step 7: Share Your CatDrone Website!

Send the link to friends and family so they can experience the revolutionary CatDrone technology!

## Optional Enhancements

Consider these additions to make your HammerDCat website even better:

1. **Custom Domain**: If you want a domain like "hammerdcat.com" instead of "yourusername.github.io":
   - Purchase a domain from a registrar like Namecheap or GoDaddy
   - Follow the GitHub Pages instructions for adding a custom domain

2. **Add More Images**: Create additional flattened cat and CatDrone designs to expand your collection

3. **Add Analytics**: Integrate Google Analytics to track how many visitors are viewing your cat flattening process

4. **Customer Testimonials**: Add a section with fake reviews from "satisfied customers" showing their flattened cats and CatDrones in action

5. **Social Media Integration**: Add buttons to share your CatDrone innovations on various social platforms

Remember: the future of pet technology is flat!
