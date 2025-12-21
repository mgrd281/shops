# 📷 Visual Search System Documentation

## Overview
A high-end, visual-first search experience inspired by top e-commerce sites (Otto/Amazon).
It replaces the standard search list with a rich grid of product images.

## ✅ Features

### 1. Visual Layout (Grid)
- Products are displayed as **Large Image Cards**.
- Clean, minimal design with focus on product visuals.
- Prices and titles are clearly legible.

### 2. "Recently Viewed" Section
- Default view when opening search.
- Shows popular products or recently viewed items.
- Mimics the "Zuletzt angesehen" feature from the reference image.

### 3. Image Search UI 📷
- **Camera Icon:** Added to the search bar.
- **Functionality:** Opens file selector for image upload.
- **Note:** Actual image recognition requires an external API (Google Vision/AWS Rekognition). Currently, it serves as a UI demo ready for backend integration.

### 4. Instant Search
- Updates results as you type (> 300ms delay).
- Uses Shopify's Predictive Search API.

## 🛠 File Structure
- `snippets/visual-search.liquid`: Contains all HTML, CSS, and JS for the system.
- `VISUAL_SEARCH.md`: This documentation.

## 🚀 Usage
The search overlay opens automatically when clicking any search icon in the theme.

### To Revert:
Simply revert the last commit or remove `{% render 'visual-search' %}` from `layout/theme.liquid`.
