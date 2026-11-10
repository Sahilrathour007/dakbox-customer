# Dakbox: customer booking site

Customers get a price, drop the pickup pin on a map, book a pickup and track their parcel by AWB.

- `index.html`: the whole site
- `config.js`: Supabase project URL and **anon** key (safe to publish; the database only lets it quote, book and track)

Data lives in the Supabase project `kmqerwmfbpknrffadhoi`. The database setup, staff site and GPS receiver are in the separate **dakbox-ops** repo.

## Run locally
```bash
python3 -m http.server 8080
```
Open http://localhost:8080

## Put it online
Any static host: Netlify, Vercel, Cloudflare Pages or GitHub Pages. It must be served over https for "Use my location" to work.

Maps: OpenStreetMap tiles and Nominatim pincode search (free; max 1 search per second).
