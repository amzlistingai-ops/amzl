# amzlisting.ai announcement website

A complete static marketing website for amzlisting.ai, ready to upload to GitHub and deploy on Vercel.

## Included

- Homepage and separate pricing page
- Deep teal and mint theme
- Locally hosted Manrope and Plus Jakarta Sans fonts
- Five AI specialists and the research-to-creative workflow
- SEO listing copy, high-CTR main image concepts, conversion-optimized listing images, bulk variations, A/B testing, and A+ Content strategy
- Individual plan: $95/month for 15 listings
- Team plan: $495/month; allowances announced at launch
- White CreatiWOW attribution, mint hover treatment, and link to https://creatiwow.com/
- Contact email: contact@amzlisting.ai
- Responsive styles and keyboard-accessible specialist tabs
- Launching-soon messaging with no signup or app links

## Upload to GitHub

1. Extract this ZIP file.
2. Create a repository on GitHub, for example `amzlisting-ai`.
3. Choose **uploading an existing file** or **Add file > Upload files**.
4. Upload the contents of the `amzlisting-ai` folder into the repository root. Include the entire `public` directory, `licenses`, `README.md`, and `vercel.json`.
5. Commit the files.

The repository root must contain `vercel.json` and `public/` directly. Do not upload only the ZIP file or place everything inside another nested folder.

## Deploy on Vercel

1. In Vercel, create a new project and import your GitHub repository.
2. Use the repository root as the Root Directory.
3. Keep the Framework Preset as **Other**.
4. The included `vercel.json` sets the output directory to `public` and skips install and build commands. No dependencies or environment variables are required.
5. Deploy.
6. In project settings, add `amzlisting.ai` as a custom domain if you want to use it, and follow the DNS records shown by Vercel.

This package has been checked locally. It has not been deployed to your Vercel account.

## Preview locally

Run from the repository root with Python installed:

```sh
python -m http.server 8000 --directory public
```

Open http://localhost:8000/ and http://localhost:8000/pricing/.

## Edit the website

- Homepage: `public/index.html`
- Pricing: `public/pricing/index.html`
- Styles: `public/assets/style.css`
- Specialist tab behavior: `public/assets/site.js`
- Logos and font files: `public/assets/`

The header, footer, and pricing cards are included directly in each HTML file. Update both pages when changing shared content. If your GitHub repository is connected to Vercel, pushes to the production branch trigger a new deployment.

## Ownership and font licenses

The site content and supplied logos belong to their respective owners. No additional license is granted for those brand assets. Manrope and Plus Jakarta Sans use the SIL Open Font License; their license notices are included in `licenses/`.

## Documentation

- Vercel project configuration: https://vercel.com/docs/project-configuration/vercel-json
- Vercel build settings: https://vercel.com/docs/builds/configure-a-build
