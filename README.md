## Development

Build Tailwind CSS and serve locally.

- Install dependencies:

```bash
npm install
```

- Build CSS once:

```bash
npm run build:css
```

- For development watch:

```bash
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

- Serve the project (so external CDN scripts load properly):

```bash
# with Python
python -m http.server 5173
# or with a simple Node server
npx http-server . -p 5173
```

Open `http://localhost:5173` in your browser. If you prefer the Tailwind CDN for quick previews, ensure you're serving over HTTP (Live Server) rather than opening the file via `file://`.
