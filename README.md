# Rentness — House Rental & Property Listing Website

A responsive rental listing website built with HTML, CSS, JavaScript, Node.js and Express.js.

## Features
- Responsive landing page and property cards
- Search by location, property type and maximum monthly rent
- Filter by minimum bedrooms and sort by rent/area
- Property detail modal and enquiry form
- Save favourites in browser localStorage
- Add a property listing through a form
- Express REST API for properties and enquiries

## Requirements
- Node.js (LTS version recommended)
- Internet connection for Google Fonts and remote property photos

## Run on Windows
1. Extract `rentness-website.zip`.
2. Open the `rentness-website` folder in VS Code.
3. Open Terminal > New Terminal.
4. Run `npm install`.
5. Run `npm start`.
6. Open `http://localhost:3000` in your browser.

If `npm` is not recognized, install Node.js LTS from https://nodejs.org/, restart VS Code, and try again.

## API routes
- `GET /api/health` — check server status
- `GET /api/properties` — list properties; supports `q`, `type`, `maxRent`, `minBeds`, and `sort`
- `GET /api/properties/:id` — one property
- `POST /api/properties` — add a listing
- `POST /api/enquiries` — submit a property enquiry

## Important demo notes
- Seed property data is sample data, not live verified real-estate inventory.
- New properties and enquiries are stored in server memory and reset when the server restarts.
- Favourites are saved in the current browser using localStorage.
- This starter project does not include user login, owner verification, payment processing, or a permanent database. Add a database such as MySQL/MongoDB before using it for a real service.
- Images are loaded from Unsplash URLs and require internet access.
