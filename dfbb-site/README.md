# DFBB website

A responsive, framework-free static website. Open index.html in a browser. No build step, database, API keys, or application server is required. All content and navigation work without JavaScript.

## Pages and design
- Home: large editorial headline, actual DFBB YouTube thumbnail, featured performances, introduction, support link.
- Our story: Boston young-professional community and documented dance background.
- The crew: honest pending state for member profiles. Add approved names, portraits, roles/styles, and short bios to members.html.
- Videos: 12 direct video links found in YouTube search, all attributed to the DFBB Dance channel. videos.json is a reference inventory; edit videos.html to change rendered cards.
- Support: donation information pending; working YouTube support link. Replace the pending panel with the organization's verified hosted donation URL and approved explanation of fund use.
- 404: custom error page.

Pale lavender, dark plum, and purple accent palette; bold typography; responsive grids; keyboard focus indicators; skip link; reduced-motion support. Remote YouTube thumbnails load when pages open. Videos open on YouTube, avoiding heavy embedded players.

## Hosting decision
Public web hosting is necessary, but renting/managing a dedicated server is not. Use managed static hosting and optionally connect your own domain. YouTube hosts the videos. A hosted donation checkout can handle payments independently of this site. A backend becomes relevant only for private member accounts, a custom admin system, or custom transaction processing.

Cloudflare Pages supports this folder directly: https://developers.cloudflare.com/pages/framework-guides/deploy-anything/
Upload this folder using its static deployment flow, or connect a Git repository. For a repository containing this folder as its root, use no framework and the root output directory; no build is needed. The official guide documents `exit 0` as the optional build command. A pages.dev address is provided. Cloudflare now recommends Workers for new projects in its overview; Workers Static Assets is another suitable managed option. This portable HTML site does not depend on either provider.

## Before launch
1. Confirm the page copy and branding.
2. Add approved member profiles and photos. Do not publish private contact details.
3. Provide the exact donation destination, recipient name, use-of-funds copy, and any applicable receipt information. No tax-deductibility claims have been added.
4. Add a public organizational contact address if desired.
5. Choose a host/domain, publish, and verify HTTPS and all links.

The site has not been published. A real donation destination and member information were not provided; these areas are visibly pending, not fabricated.

## Sources, checked September 29, 2026
- User: Boston nonprofit crew formed by young professionals from different fields.
- YouTube search: https://www.youtube.com/results?search_query=dfbb+dance
- Channel: https://www.youtube.com/@dfbbdance
- Channel ID returned in search: UCPlDy-4JzqzqMJRfn6N8e5g
- HCSSA 2020 program (founding year and styles): https://hcssa.github.io/spring/
- HCSSA 2022 program corroborates Boston nonprofit dance group: https://harvardcssa.org/wp-content/uploads/2022/02/2022-HCSSA%E8%99%8E%E5%B9%B4%E6%98%A5%E6%99%9A%E5%9C%BA%E5%88%8A-1.pdf

YouTube search metadata confirms video IDs, titles, and uploader; playback and geographic availability may vary. No current member roster was inferred from historical video credits.
