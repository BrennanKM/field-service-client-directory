# Field-Service Client Directory

A mobile web app I built to run my seasonal outdoor-services business (blackberry removal, pressure washing, junk removal) in the Portland, Oregon area. It replaced a spreadsheet and I use it daily in the field from my phone.

**[Try the live demo](https://brennankm.github.io/field-service-client-directory/)** (works best on a phone; you can install it to your home screen).

> **This is a public demo.** The live version syncs to a private Airtable base. Here, the data layer is replaced by an in-memory store with the same request and response shape, filled with generated sample data. Every client, address, and phone number is fictional.

## What it does

- **Directory:** every client with contact actions (call, text, map), service history, lifetime revenue, and a status pipeline (to contact, reached out, booked, done). Clients are segmented into repeaters, friends and family, and one-timers so outreach goes to the likeliest rebookings first.
- **Schedule:** month calendar, upcoming jobs, and a "log actuals" flow that records hours worked and amount paid once a job is done.
- **Outreach:** logs Nextdoor posts and door-to-door card drops, with card-drop areas and client locations plotted on a map.
- **Stats:** revenue by month and by service, $/hour by service, top clients, and year-over-year comparison. Free-text job descriptions are grouped into service categories by a keyword classifier.

## What I learned from the data

$/hour by service showed blackberry removal earned the most per hour, so I moved my marketing to lead with it.

## Built with

HTML, CSS, and vanilla JavaScript in a single file; Leaflet and OpenStreetMap for the map; installable as a PWA (offline support through a service worker). The live version reads and writes Airtable through its REST API.

## Run it

Open `index.html` in a browser. There's no build step and nothing to install.
