# Where should India build its next data centres?

A static, single-page scrolling 3D briefing. No build step is needed.

## Files
- `index.html` – the whole site (map geometry and data are embedded).
- `data/India_DataCentre_Feasibility_Index_2026.xlsx` – the model workbook, linked from the page.
- `vercel.json` – clean URLs and basic security headers.

## Deploy with the Vercel CLI
1. Install Node.js 18+, then run `npm i -g vercel`.
2. In this folder, run `vercel` and follow the prompts (log in, accept defaults; framework: "Other").
3. Run `vercel --prod` to publish to your production URL.

## Deploy from GitHub
1. Create a new GitHub repository and upload these files to its root.
2. In Vercel, choose **Add New → Project**, import the repository, keep Framework Preset = **Other**, leave build and output settings empty, and click **Deploy**.

## Notes
- The page loads three.js from cdnjs/jsDelivr and fonts from Google Fonts, so viewers need internet access. If an organisation blocks these CDNs, download the two scripts into the folder and update the `<script src>` paths.
- To restrict access, use Vercel's Deployment Protection (password or Vercel Authentication) under Project Settings.
