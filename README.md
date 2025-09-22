# 21cmFAST Performance Profiling Slides

## Viewing the Presentation

### Option 1: Open Directly in Browser
Simply open `index.html` in any modern web browser:
```bash
firefox slide/index.html
# or
chrome slide/index.html
```

### Option 2: Serve with Python HTTP Server
For better compatibility, serve the slides locally:
```bash
cd slide/
python3 -m http.server 8000
# Then open http://localhost:8000 in your browser
```

### Option 3: Using Live Server
If you have a live server extension in VS Code or similar:
- Right-click on `index.html`
- Select "Open with Live Server"

## Navigation
- Use arrow keys to navigate between slides
- Press `ESC` to see all slides
- Press `F` for fullscreen mode
- Press `S` for speaker notes (not used in this presentation)

## Plot Images
The presentation expects the following plot files to exist:
- `plot/execution_times_run0_run1.png` - Execution times comparison
- `plot/profile_run_new.png` - Profile analysis for run_new.py

Generate these plots by running:
```bash
# First, generate profiling data
script/profile.sh -n 5 -t run0
script/profile.sh -n 5 -t run1

# Then create the plots
python script/plot.py run0 run1
```

## Customization
The slides use reveal.js with a white theme and custom CSS for better readability. You can modify the styles in the `<style>` section of `index.html`.