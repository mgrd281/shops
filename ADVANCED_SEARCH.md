# 🔍 Advanced Search System Documentation

## Overview
The Advanced Search System transforms the standard search into an "Amazon-like" experience with auto-complete, instant product suggestions, and search history.

## ✅ Features
1. **Intelligent Auto-complete:** Predicts user intent as they type.
2. **Instant Product Suggestions:** Shows products with images, prices, and ratings immediately.
3. **Search History:** Remembers last 10 searches for quick access.
4. **Voice Search:** Integrated microphone support (Chrome/Edge).
5. **Keyboard Navigation:** Full support for arrow keys and Enter.
6. **Mobile Optimized:** Responsive design for all devices.

## 🛠 File Structure
- `snippets/advanced-search.liquid`: The core component containing HTML, CSS, and JavaScript.
- `ADVANCED_SEARCH.md`: This documentation.

## 🚀 How to Enable/Disable
This system is designed for easy revert.

### To Enable:
The `advanced-search` snippet is rendered in `layout/theme.liquid` or `sections/header.liquid`.

### To Disable:
Simply revert the last commit or remove the `{% render 'advanced-search' %}` line.

## 🔧 Customization
- **Max History:** 10 items (Change in JS `saveToHistory`)
- **Suggestions Limit:** 6 items (Change in JS `performSearch`)
- **Debounce Time:** 300ms (Change in JS `searchInput` listener)

## 📊 Performance
- **Debouncing:** Prevents excessive API calls.
- **Local Storage:** Caches search history locally.
- **Lazy Loading:** Product images are lazy-loaded.

---
**Status:** ✅ Active and Optimized
