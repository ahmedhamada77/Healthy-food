# Project guide

Nourish is a static HTML/CSS/JavaScript site with no dependencies or build step. `index.html` defines the landing page and native dialogs, `style.css` handles the responsive cream-and-sage design, `fixtures.js` contains all recipe ingredients and catalog combinations, and `app.js` implements browsing and calculators. Netlify publishes the root directory.

Keep catalog content separate from rendering. Use explicit labels for estimated nutrition and general cooking videos. Saved recipes are a transient Set for the current page visit, not persistent storage. Do not introduce browser storage for persistence; future persistent features must use Netlify primitives.

Calculations use Mifflin–St Jeor, activity multipliers, and the adult BMI reference interval. Keep the adult-only validation, contextual caveats, and low-intake guard intact. Dialog close must unload the YouTube iframe. Use semantic controls, visible focus states, and reduced-motion support. Follow PLAN.md for the next product milestones.
