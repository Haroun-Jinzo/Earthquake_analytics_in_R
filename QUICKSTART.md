# 🚀 Quick Start Guide

## Get Your Presentation Running in 2 Minutes

### Step 1: Ensure You Have Required Packages

Open R or RStudio and run:

```r
# Install/update required packages
packages <- c("tidyverse", "readxl", "corrplot", "knitr", "lubridate")
install.packages(packages)
```

### Step 2: Render the Project

**Option A: From PowerShell/Terminal**
```bash
cd "c:\Users\Jinzo\Desktop\Polytechnique\5eme\R\Earthquake_Projet_R\Project_R_Template"
quarto render
```

**Option B: From RStudio**
1. Open `Project_R_Template.Rproj`
2. Click **Build → Render Project**

**Option C: Quick Preview**
```bash
quarto preview
```
This opens a live preview in your browser that updates as you make changes.

### Step 3: View Your Presentation

After rendering, open:
```
docs/index.html
```

That's it! Your presentation is ready.

---

## 📚 What You Get

✅ **Professional Website** with:
- Landing page with project overview
- Sidebar navigation
- 5 analysis sections
- 8+ high-quality plots
- Statistical tables and insights

✅ **Complete Analysis Pipeline**:
1. Data Import
2. Data Cleaning  
3. Exploratory Analysis
4. Correlation Analysis
5. Conclusions

✅ **Publication-Ready Visualizations**:
- Magnitude distributions
- Geographic maps
- Intensity attenuation patterns
- Statistical correlations

---

## 🎯 Project Sections at a Glance

| Section | File | Purpose |
|---------|------|---------|
| **Home** | index.qmd | Overview & navigation |
| **Import** | 01-data-import.qmd | Load raw Excel data |
| **Clean** | 02-data-cleaning.qmd | Handle missing values, fix types |
| **Explore** | 03-exploratory.qmd | Visualize patterns & distributions |
| **Correlate** | 04-correlations.qmd | Statistical relationships |
| **Conclude** | 07-conclusions.qmd | Summary & key findings |

---

## 🛠️ Customization Tips

### Change Author Name
Edit the YAML header in each `.qmd` file:
```yaml
---
author: "Your Name Here"
---
```

### Modify Colors
All plots use this color palette in `03-exploratory.qmd` and `07-conclusions.qmd`:
```r
#2E86AB (blue)     # Primary
#A23B72 (purple)   # Secondary
#F18F01 (orange)   # Accent
#E63946 (red)      # Warning
```

### Add New Analysis
1. Create `XX-topic.qmd` in `qmd/` folder
2. Add to `_quarto.yml` sidebar under `Analysis Pipeline`
3. Run `quarto render`

### Show/Hide Code
In any section header:
```yaml
---
format:
  html:
    code-fold: true    # Hide code by default (show with button)
    code-fold: false   # Show code by default
---
```

---

## 📊 Data Pipeline

```
Raw Data (Excel)
      ↓
01-data-import.qmd   (Load & examine)
      ↓
02-data-cleaning.qmd (Clean & prepare)
      ↓
03-exploratory.qmd   (Visualize patterns)
      ↓
04-correlations.qmd  (Statistical analysis)
      ↓
07-conclusions.qmd   (Synthesize findings)
      ↓
docs/index.html      (Professional presentation)
```

---

## 🔍 What Each File Does

### `index.qmd` - Your Landing Page
- Project title and metadata
- Research questions
- Key findings preview
- Navigation to all sections
- Tools & methods used

### `03-exploratory.qmd` - Data Exploration
- 5 high-quality plots showing patterns
- Magnitude, geography, distance, intensity, temporal analysis
- Summary statistics tables

### `07-conclusions.qmd` - Final Summary
- Geographic analysis with visualizations
- Magnitude breakdown by state
- Seismic attenuation confirmation
- Statistical correlations explained
- Quality metrics and methodological notes

---

## 💡 Pro Tips

1. **Live Preview While Editing**
   ```bash
   quarto preview
   ```
   Keep this running in a terminal. Changes auto-reload in browser!

2. **Share Easily**
   - Copy entire `docs/` folder
   - Open `docs/index.html` in any browser
   - No internet required!

3. **Professional Polish**
   - All plots have captions
   - Callout boxes highlight key findings
   - Color-coded by importance
   - Error bars show uncertainty

4. **Reproducible Research**
   - All code is visible & documented
   - Can toggle code visibility
   - Comments explain each step
   - p-values reported for statistics

---

## ❓ Troubleshooting

### Issue: "Quarto not found"
**Solution:** Install Quarto from https://quarto.org/docs/get-started/

### Issue: "Package not found"
**Solution:** Run in R:
```r
install.packages("package_name")
```

### Issue: Plots look different
**Solution:** Make sure you have latest versions:
```r
update.packages()
```

### Issue: Render fails on data import
**Solution:** Ensure `data/processed/earthquake_clean.rds` exists by running `02-data-cleaning.qmd` first in RStudio.

---

## 🎓 Learning Outcomes

After completing this project, you've demonstrated:

✅ **Data Science Skills**
- Data cleaning & preparation
- Exploratory data analysis
- Statistical analysis
- Data visualization

✅ **R Proficiency**
- tidyverse for data manipulation
- ggplot2 for visualization
- Statistical testing

✅ **Geophysical Knowledge**
- Earthquake magnitude scales
- Intensity measurement
- Seismic wave attenuation

✅ **Communication**
- Professional presentation format
- Clear data storytelling
- Statistical reporting

---

## 📞 Next Steps

1. ✅ Run `quarto render` to generate your presentation
2. ✅ Open `docs/index.html` to view it
3. ✅ Customize author names and details
4. ✅ Share with professors or in portfolio
5. ✅ Consider extensions (interactive maps, predictions, etc.)

---

**Happy Presenting!** 🎉

Your Quarto presentation is publication-ready and demonstrates professional-grade data analysis skills.

---

*Created: January 7, 2026*  
*Project: Earthquake Data Analysis*  
*Tools: R, Quarto, tidyverse, ggplot2*
