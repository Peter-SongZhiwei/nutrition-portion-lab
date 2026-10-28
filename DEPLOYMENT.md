# GitHub Pages deployment

This is a static HTML, CSS and JavaScript site. No installation or build is required.

In repository Settings → Pages:

1. Set Source to **Deploy from a branch**.
2. Select **main** and **/ (root)**.
3. Click **Save** and wait for the Pages deployment to finish.

The page contains the personalized profiles and nutrition targets requested by its owner. Nutrition sources, unit conversions and zero-value fallback rules are documented within the page. Serving sizes are saved only in each browser's localStorage.

## Release process

For every subsequent website update, increment the patch version by 1 (1.0.2 → 1.0.3), update the header badge and APP_VERSION, and prepend a dated entry to RELEASES in index.html. Preserve historical entries: 1.0 initial launch, 1.0.1 category nutrition dialogs, 1.0.2 release history, independent food rankings, page sections, and favicon.

Food rankings are a separate reference dataset, independent of the calculator's selected foods and portions. The embedded USDA SR Legacy values are per 100 g edible food (copper converted from mg to micrograms); trace nutrients use NIH ODS selected-food tables. Preserve source links, food preparation state, approximate serving labels, and ranking scope. Sort by nutrient per gram, and show amount plus serving weight. Do not invent values or replace missing composition values with measured zeros.
