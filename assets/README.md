# Assets Directory

This directory contains media assets for the GitHub profile README.

## Screenshot Guidelines

### Directory Structure
```
assets/
└── screenshots/
    ├── interview-assistant/    # Interview Assistant project screenshots
    ├── whisper-flow/           # Whisper-Flow/Murmur screenshots
    ├── claude-workflows/       # Claude Code Workflows screenshots
    └── other-projects/         # Screenshots for other projects
```

### Adding Screenshots

1. **Capture Screenshots**: Take high-quality screenshots of your projects
   - Use consistent dimensions (recommended: 1280x800 or 1920x1080)
   - Use dark mode for consistency
   - Highlight key features and UI elements

2. **Naming Convention**: Use descriptive names
   ```
   interview-assistant-dashboard.png
   whisper-flow-recording-overlay.png
   claude-workflows-youtube-educator.png
   ```

3. **Optimization**: Compress images before committing
   ```bash
   # Install ImageOptim (macOS) or use online tools
   # Target: < 500KB per screenshot
   ```

4. **Update README**: Replace placeholder text with actual image paths
   ```markdown
   # Before
   [📸 Screenshots Coming Soon]

   # After
   ![Interview Assistant Dashboard](assets/screenshots/interview-assistant/dashboard.png)
   ```

### Best Practices

- **Privacy**: Ensure no sensitive data is visible in screenshots
- **Quality**: Use retina/high-DPI screenshots for clarity
- **Consistency**: Use similar themes/color schemes across all screenshots
- **File Size**: Keep total assets directory under 10MB for fast loading
- **Format**: Use PNG for UI screenshots, JPG for photos/diagrams

### Example Update Workflow

```bash
# 1. Add screenshots to appropriate directory
cp ~/Desktop/screenshot.png assets/screenshots/interview-assistant/

# 2. Stage changes
git add assets/screenshots/

# 3. Update README.md to reference new screenshots
# (Edit README.md manually)

# 4. Commit
git commit -m "docs: Add Interview Assistant screenshots"

# 5. Push
git push origin main
```

## Future Assets

You can also add:
- Architecture diagrams (`assets/diagrams/`)
- Demo GIFs (`assets/demos/`)
- Logos and icons (`assets/icons/`)

Create subdirectories as needed and follow similar naming conventions.
