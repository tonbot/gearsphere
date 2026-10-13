# GearSphere

**A Community Gear-Sharing and Equipment Rental Marketplace**

GearSphere is a web application designed to connect people who own equipment with people who need it. Users can discover gear, create equipment listings, upload images, and manage their listings through a shared marketplace.

## Deployment
Deployed to Vercel:
[Site Link](https://gearsphere.vercel.app/)

## Tech Stack

- **Framework:** Next.js 16 (App Router)
- **Frontend:** React 19 and TypeScript
- **Styling:** Tailwind CSS 4
- **Backend and Database:** Supabase and PostgreSQL
- **Authentication:** Supabase Auth
- **File Storage:** Supabase Storage
- **Code Quality:** ESLint

## Implemented Features

- **Landing Page:** Introduces the platform, equipment categories, and featured gear.
- **User Authentication:** Authentication-related pages and account access.
- **Equipment Listings:** Create, view, and edit equipment listings.
- **Image Management:** Upload and remove listing images.
- **User Dashboard:** Shared layout and navigation for signed-in users.
- **Booking:** Users can make a bookong or cancel a book for a listing. 
- **Rating & Reviews:** Users can leave a rating and/or add reviews on a listing.
- **Custom 404 Page:** A branded page for unavailable routes.


## Getting Started

### Prerequisites

Install [Node.js](https://nodejs.org/), npm, and Git. You will also need access to the project's Supabase credentials.

### 1. Clone the Repository

```bash
git clone https://github.com/tonbot/gearsphere.git
cd gearsphere
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env.local` file in the project root and add your Supabase project credentials:

```dotenv
NEXT_PUBLIC_SUPABASE_URL=https://YOUR_PROJECT_ID.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=YOUR_SUPABASE_PUBLIC_ANON_KEY

GEARSPHERE_DATABASE_URL=https://YOUR_PROJECT_ID.supabase.co
GEARSPHERE_ANON_KEY=YOUR_SUPABASE_PUBLIC_ANON_KEY
```

Replace the placeholders with the values provided by the project team. Never commit environment files or expose privileged credentials.

### 4. Start the Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Available Commands

| Command | Description |
|---|---|
| `npm run dev` | Start the development server |
| `npm run build` | Build the application for production |
| `npm run start` | Run the production build |
| `npm run lint` | Run ESLint |

## Database and Image Storage

GearSphere uses Supabase and PostgreSQL to manage application data. Listing information is stored in the database, while listing image files are stored in the Supabase Storage bucket `listing-images`, with their metadata maintained in the `listing_images` table.

## Design System

The application uses **Inter** typography and the following theme colors:

- **Primary:** `#166534`
- **Secondary:** `#334155`
- **Accent:** `#F59E0B`

## Collaborators

- [Toyin Ajiboye](https://github.com/tonbot)
- [Collins Onyebuchi Attah](https://github.com/attahcollinso)
- [Michael Tatani Kazembe](https://github.com/michaelkazembe)
- [Lorenzo Ivan Salamanca](https://github.com/ZigzagAlloy01)

## Team Quotes
- "You don't need to figure it all at once, let the problem teach you as you go." - _Toyin Ajiboye_
- "Nothing is impossible with God." - _Michael Tatani Kazembe_
- "Persistence is the key, if your mind can conceive it, you can achieve it". - _Attah Collins_
- "Pride has the power to hinder our progress as nothing else can." - _Lorenzo Ivan Salamanca_

## Repository

[GitHub — tonbot/gearsphere](https://github.com/tonbot/gearsphere)
