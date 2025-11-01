# Visualizations Usage Guide

## 🎨 What Was Created

### Interactive Visualizations (visualizations.html)

A comprehensive interactive dashboard with **7 different chart types**:

1. **Overall Quality Comparison** - Bar chart showing 94% vs 76%
2. **Quality Dimensions Radar** - Spider chart with all 7 dimensions
3. **Topic-by-Topic Results** - Grouped bar chart for all 7 topics
4. **Citation Count Comparison** - Doughnut chart (265 vs 166)
5. **Grokipedia Advantages** - Horizontal bar chart of point differences
6. **Win Distribution** - Pie chart (6 wins, 0 losses, 1 tie)
7. **Quality Margins by Topic** - Bar chart with color-coded margins

**Features:**
- Interactive tooltips on hover
- Responsive design (mobile/desktop)
- Professional gradient styling
- Built with Chart.js library
- Ready for GitHub Pages

**View Live:** https://davidorban.github.io/pedia/visualizations.html

### Static SVG Graphics (images/)

Four high-quality vector graphics ready for presentations:

1. **overall-comparison.svg** (800×500px)
   - Bar chart with winner badge
   - Shows 26.7 vs 33.0 scores
   - Best for: Executive summaries, social media

2. **key-findings.svg** (1000×600px)
   - 6 key statistics in card layout
   - Includes emojis and colors
   - Best for: Infographics, newsletters

3. **dimension-comparison.svg** (900×700px)
   - All 7 dimensions with bars
   - Shows exact scores and checkmarks
   - Best for: Detailed presentations

4. **topics-comparison.svg** (900×600px)
   - Individual topic scores
   - Color-coded margins (+2 to +11)
   - Best for: Topic-specific discussions

## 📊 Quick Usage Examples

### For Blog Posts

```markdown
![Key Findings](https://davidorban.github.io/pedia/images/key-findings.svg)

The analysis reveals compelling results across multiple dimensions...
```

### For Presentations

**PowerPoint/Keynote/Google Slides:**
1. Go to Insert → Image
2. Select any SVG file from `images/` folder
3. Scale to desired size (vectors scale perfectly)

### For Social Media

**Twitter/X:**
- Use `key-findings.svg` (fits well in timeline)
- Use `overall-comparison.svg` (simple, clear message)

**LinkedIn:**
- Use `dimension-comparison.svg` (professional detail)
- Link to full analysis: https://davidorban.github.io/pedia

### For Research Papers

```latex
\begin{figure}[h]
\centering
\includegraphics[width=0.8\textwidth]{images/overall-comparison.svg}
\caption{Overall quality comparison between Wikipedia and Grokipedia}
\label{fig:overall}
\end{figure}
```

## 🎯 Which Visualization to Use When

### Executive Summary / Quick Overview
→ Use **overall-comparison.svg** or **key-findings.svg**
- Shows headline numbers
- Easy to understand at a glance
- Great for non-technical audiences

### Detailed Analysis
→ Use **dimension-comparison.svg** or **topics-comparison.svg**
- Shows all dimensions/topics
- Good for technical discussions
- Supports detailed questions

### Interactive Exploration
→ Use **visualizations.html**
- Let audience explore data
- Best for workshops/presentations
- Provides drill-down capability

### Print Media
→ Use any **SVG file**
- Scales to any size
- High print quality
- Small file size

## 🎨 Customization Options

### Changing Colors

All SVGs use these color codes:
- Wikipedia Blue: `#2563eb`
- Grokipedia Orange: `#f97316`
- Success Green: `#10b981`

To customize:
1. Open SVG in text editor
2. Find and replace color codes
3. Save and reload

### Changing Dimensions

SVGs have fixed viewBox but scale perfectly:
- `overall-comparison.svg`: 800×500
- `key-findings.svg`: 1000×600
- `dimension-comparison.svg`: 900×700
- `topics-comparison.svg`: 900×600

To resize in HTML:
```html
<img src="images/overall-comparison.svg" width="1200">
```

### Creating New Variations

The visualizations.html page can be customized:
1. Edit the data arrays at the top of `<script>`
2. Modify Chart.js options
3. Add new chart types
4. Change colors in CSS variables

## 📱 Mobile Responsiveness

All visualizations are mobile-friendly:
- **Interactive charts**: Automatically resize
- **SVG graphics**: Scale to container width
- **Touch support**: Works on tablets/phones

Recommended mobile display:
```html
<img src="images/overall-comparison.svg"
     style="max-width: 100%; height: auto;">
```

## 🔗 Embedding in Websites

### Direct Image Embed
```html
<img src="https://davidorban.github.io/pedia/images/key-findings.svg"
     alt="Key Findings"
     width="800">
```

### Interactive Frame
```html
<iframe src="https://davidorban.github.io/pedia/visualizations.html"
        width="100%"
        height="600"
        frameborder="0">
</iframe>
```

### Markdown (GitHub, Jekyll, Hugo)
```markdown
![Overall Comparison](images/overall-comparison.svg)
```

## 📊 Data Sources

All visualizations are based on the analysis data:
- **7 topics** evaluated
- **7 quality dimensions** measured
- **1-5 scale** for each dimension
- **Total: 98 data points** (7×7×2)

Data files available in:
- `v2_analysis/evaluation_summary.md` - Statistical summary
- `v2_analysis/quality_matrix.md` - Complete scoring matrix
- Individual `eval_*.md` files - Per-topic details

## 🎓 Best Practices

### For Academic Papers
1. Use SVG files for figures
2. Reference source data clearly
3. Cite as: Orban, D. (2025)
4. Include methodology note

### For Presentations
1. Start with overall-comparison
2. Show key-findings summary
3. Drill into dimension-comparison
4. End with topics-comparison

### For Blog Posts
1. Lead with key-findings
2. Embed interactive visualizations
3. Link to full analysis
4. Include data source

### For Social Media
1. Use single impactful chart
2. Add concise caption
3. Include link to full analysis
4. Use relevant hashtags

## 🚀 Performance

**File Sizes:**
- visualizations.html: ~30KB (plus 180KB Chart.js CDN)
- Each SVG: 10-25KB
- Total images folder: ~60KB

**Load Times:**
- SVGs: Instant (inline or cached)
- Interactive page: <1 second on good connection

## 📄 License

All visualizations licensed under CC BY 4.0

**Attribution:**
```
Visualizations from "Wikipedia vs Grokipedia Quality Comparison"
by David Orban (2025)
https://github.com/davidorban/pedia
```

## 🔄 Updates

Want to update the visualizations with new data?

1. **Interactive Charts:** Edit data arrays in visualizations.html
2. **SVG Graphics:** Edit XML in SVG files directly
3. **Both:** Use vector graphics tools (Figma, Inkscape, Illustrator)

## 📞 Support

Questions about visualizations:
- Check [images/README.md](images/README.md)
- Review source code in visualizations.html
- Open issue on GitHub: https://github.com/davidorban/pedia/issues

---

**Created:** 2025-11-01
**Version:** 1.0
**Tools Used:** Chart.js, SVG, HTML5/CSS3
