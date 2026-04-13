# 📸 How to Add Your Images to the Portfolio

Your portfolio is now configured with the **living room/couch image as the hero background banner**. Follow these steps to display all your images:

## Step 1: Prepare Your Images

You need to save 6 images in the `/projects/` folder:

```
projects/
├── modern-living-interior.jpg  (Hero background + Portfolio item)
├── luxury-villa-pool.jpg
├── architectural-3d-model.jpg
├── interior-minimalist.jpg
├── modern-residence-garage.jpg
└── luxury-resort-home.jpg
```

## Step 2: Image Requirements

**Image Format & Size:**
- Format: JPG, PNG, or WebP
- Size: 1200x800px minimum (for project grid)
- File size: Optimized to 200-500KB each

**How to Optimize:**
1. Use online tools: [TinyPNG.com](https://tinypng.com) or Squoosh
2. Or use Photoshop/GIMP to resize and export
3. Or use this command if you have ImageMagick:
   ```
   magick convert image.jpg -resize 1200x800 -quality 80 optimized.jpg
   ```

## Step 3: Add Images to Your Portfolio

### Option A: Simple File Copy (Recommended)
1. Export/save your 6 best renders from Blender/3ds Max
2. Name them exactly as shown above
3. Copy them to the `projects/` folder

### Option B: Using Windows/File Explorer
1. Right-click `projects` folder → Open
2. Drag and drop your 6 images there
3. Rename them to match the filenames above

### Option C: Batch Processing
If you have multiple images to rename, use this batch rename tool:
- Windows: Use Windows built-in renamer (Shift + F10)
- Online: [CloudConvert.com](https://cloudconvert.com)

## Step 4: Verify Setup

Your folder should look like:
```
Urbanstage3Dweb/
├── index.html
├── styles.css
├── script.js
├── projects/
│   ├── modern-living-interior.jpg    ← Hero background
│   ├── luxury-villa-pool.jpg
│   ├── architectural-3d-model.jpg
│   ├── interior-minimalist.jpg
│   ├── modern-residence-garage.jpg
│   └── luxury-resort-home.jpg
├── about/
│   └── photo.jpg                     ← Your profile photo
└── [other files...]
```

## Step 5: Test in Browser

1. Open `index.html` in your browser
2. You should see:
   - ✅ Hero background with living room/couch image
   - ✅ 6 project thumbnails in the portfolio grid
   - ✅ Filters working (All, Real Estate, Characters, VR)
   - ✅ Hover effects on images

## Troubleshooting

### Images Not Showing?
**Problem:** "Images appear broken"

**Solution:**
1. Check file names match exactly (case-sensitive on some servers)
2. Verify files are in `/projects/` folder
3. Check file format (must be .jpg, .png, or .webp)
4. Open browser console (F12) → look for 404 errors

### Images Pixelated or Blurry?
**Solution:**
- Re-export from Blender/3ds Max at 1200x800px or larger
- Use higher quality JPEG (quality 85-90)

### Hero Background Not Showing?
**Solution:**
1. Make sure `modern-living-interior.jpg` is in `/projects/` folder
2. File name must match exactly (case-sensitive)
3. Try refreshing browser (Ctrl + F5 for hard refresh)

## Portfolio Layout After Setup

**Hero Section:** Modern living room image as full-screen background
**Grid:** 3 columns on desktop, responsive on mobile
**Filters:** 
- All (6 items)
- Real Estate (3 items)
- Characters/Interiors (2 items)
- VR (1 item)

## Optional: Advanced Image Settings

To adjust image quality in the code, edit `styles.css`:

```css
.work-thumbnail img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  filter: brightness(1) contrast(1.05);  /* Adjust brightness/contrast */
}
```

## Need Help?

If images still don't load:
1. Make sure Windows isn't hiding file extensions
2. Check that files aren't corrupted (try opening in Preview)
3. Test with one image first
4. If on Windows, check folder permissions

---

**Quick Checklist:**
- [ ] 6 images exported and optimized
- [ ] Files renamed correctly
- [ ] Files placed in `/projects/` folder
- [ ] `photo.jpg` in `/about/` folder
- [ ] File sizes < 500KB each
- [ ] Browser is refreshed (Ctrl + F5)
- [ ] No console errors (F12)

Once all images are in place, your portfolio will be complete! 🎉
