 FloodVision AI

Flood-impact and community-connectivity decision support prototype built with Lovable. All flood extent, settlement populations, road conditions, alerts, and priorities are explicitly simulated. Uploaded images are reference photographs of different scenes, not a before-and-after satellite pair. No live AI or satellite integration is claimed.

## Prototype workflow

Default assessment: **Bhote Koshi–Trishuli corridor, Nepal; 26 August 2026**, based on the supplied Track B briefs. Coordinates and settlements are invented placements, not actual case-study data. River Bridge and Hill Ascent start closed: Riverside loses both hospital and sample-town paths. Reset restores connectivity. Assessment area/date and closures persist across page navigation for matching map and report results, but not page reloads.

Area/date controls only change scenario metadata; they do not process satellite data for a selected valley. The map includes illustrative floodwater, debris, building footprints, roads and service layers. Building exposure counts derive from footprint centers inside the shared illustrative polygon, not observed damage. The satellite slider uses the PDF's generated illustrative radar examples, never a real Sentinel pair. Original user photos remain on Home and Evidence Verification.

Six additional user-provided Nepal flood photographs appear on the Home and Evidence Verification pages. Their dates, exact locations, photographers and usage rights are unverified, so they are reference context only and never satellite inputs or proof of model accuracy.

English and Nepali situation reports derive every count from the graph and footprint model. English PDF/CSV downloads require sign-in; Nepali uses browser Print / Save PDF for Unicode rendering. Reports use deterministic templates, not a generative AI copilot. The Reports page lists the max-six-page report, GitHub, three-minute video and EMSR927 submission readiness. Data Sources lists allowed inputs, checking-only reference datasets, license caveats, mandatory attribution and all judging weights.

## Competition requirements not yet implemented

Raw Sentinel-1/Sentinel-2 processing for arbitrary judge-selected areas/dates, historical pre-event OSM extraction, trained flood segmentation or a real AI situation-report copilot, DEM flow tracing, real damage measurements and independent EMSR927 validation remain unavailable. Current OSM tiles are display-only and must not become analysis inputs. Official damage maps, UNOSAT and post-event OSM edits are validation-only. Use same-orbit radar comparisons and cloud-masked optical scenes. No minutes-ahead warning of glacier collapse is possible. No victim imagery is used.

Email/password and Google authentication use Lovable Cloud. Signup requires email confirmation. Profiles and roles are separate, owner-readable tables; profiles allow owner-only name updates and new users are viewers. Field-report submission, privileged coordinator workflows, and live satellite analysis are explicitly unavailable rather than simulated as successful actions.
DF and CSV downloads require sign-in and include simulation limitations. Offline snapshots save public sample network information and scenario metadata only, not map tiles, images, private reports, or live updates. There is no full offline application shell or automatic synchronization.

## Run in VS Code

Open the repository folder in VS Code, install Bun, then run `bun install` and `bun run dev`. Copy the project's public Cloud configuration into a local `.env` using these names (do not include service-role secrets): `VITE_SUPABASE_URL`, `VITE_SUPABASE_PUBLISHABLE_KEY`, and `VITE_SUPABASE_PROJECT_ID`. The generated integration supplies these in Lovable. Database schema lives in `drizzle/migrations/`.

Run `bun run test` for route and connectivity tests. Leaflet loads after hydration; Graphology computes undirected paths. This project uses TanStack Start rather than a separate Python API. No custom external API endpoints are needed; account and profile requests use the generated Cloud client with RLS. Reference photo usage rights, location and acquisition dates require verification.

## Build with Lovable

Open your project in the [Lovable editor](https://lovable.dev) and keep building.

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: connect the project to GitHub and every change made in Lovable handles the code.
- **Stay in sync**: connect the project to GitHub and every change made in Lovable is committed straight to your repository.
- **Full ownership**: this code is yours. Push to your repository and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
## Built with

- TanStack Start
- TypeScript
- React
- Tailwind CSS

