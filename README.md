# FEM website demo

A responsive static website concept for FEM, inspired by the community, activity discovery and calendar structure of nchillhaus.com.

## Run

Requires Node.js 20 or newer. No dependency installation is needed.

```sh
npm start
```

The development server uses port 3000; override with `PORT=3001 npm start`.

```sh
npm run build
```

Publish the generated `dist/` directory with a static hosting provider. Publishing has not been performed.

## Content and booking

Verified from the public @fem.famm Instagram profile: female community positioning; workout, nutrition and mindfulness focus; Malaysian context; FEM GROUP ENTERPRISE (MA0310522-P).

The palette, illustration, marketing copy and class formats are proposed creative direction. Instagram post photographs and captions have not been extracted or verified. The illustration is original SVG artwork, not a photograph of FEM's studio.

The interactive timetable uses illustrative sessions generated relative to the visitor's current date. It does not represent live availability. All actual booking links open https://bookings.vibefam.com/femclub/classes where visitors select their real session and complete registration/payment. No payment or personal information is collected by this demo.

A live schedule embedded directly in the site requires a supported Vibefam widget or API integration supplied by the studio/provider. The current implementation makes no claim to sync bookings or reserve spaces.

## Files

- `public/index.html`: page content and accessible booking dialog
- `public/styles.css`: responsive styling
- `public/app.js`: schedule navigation, filters, dialog
- `public/schedule.js`: sample data and date helpers
- `server.js`: local static server
- `build.js`: static build output

External Google Fonts are optional; system and Georgia fallbacks are provided.

## Preview on Vercel

`vercel.json` configures the static build automatically.

1. Push these project files to your GitHub repository.
2. In Vercel, choose **Add New → Project**, then import `eewern/FEM-Website-`.
3. Use `fem` as the project name if available. Keep the root directory at the repository root. The configuration sets `npm run build` and the `dist` output directory.
4. Deploy. Vercel supplies the actual preview and production URLs.

Alternatively, from this directory with your Vercel account authenticated:

```sh
npx vercel
```

That creates a preview deployment. To publish a production deployment:

```sh
npx vercel --prod
```

The preferred address is `fem.vercel.app`. Vercel controls availability of this subdomain; this configuration does not reserve it. If unavailable, choose another project name such as `fem-famm`. No deployment or domain reservation has been performed by creating these files.
