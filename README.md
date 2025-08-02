# YC Directory

YC Directory is a platform for entrepreneurs to pitch their startup ideas, connect with others, and get feedback. Users can submit their startup details, including a pitch written in Markdown, and browse a searchable directory of all submitted startups.

![YC Directory Screenshot](public/logo.png) 

## Features

- **User Authentication:** Secure sign-up and login using NextAuth.js.
- **Create & Pitch:** Authenticated users can create a startup profile with a title, description, category, and a detailed pitch using a Markdown editor.
- **Discover Startups:** A public, searchable directory of all startups.
- **Content Management:** Powered by [Sanity.io](https://www.sanity.io/) for robust and scalable content management.

## Tech Stack

- **Framework:** [Next.js](https://nextjs.org/)
- **Styling:** [Tailwind CSS](https://tailwindcss.com/)
- **CMS:** [Sanity.io](https://www.sanity.io/)
- **Authentication:** [NextAuth.js](https://next-auth.js.org/)
- **UI Components:** [shadcn/ui](httpss://ui.shadcn.com/)
- **Deployment:** [Vercel](https://vercel.com/)

## Getting Started

Follow these instructions to get a local copy up and running for development and testing purposes.

### Prerequisites

- [Node.js](https://nodejs.org/en/) (v20 or later)
- [npm](https://www.npmjs.com/)
- A Sanity.io account and project.

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/yc-directory.git
    cd yc-directory
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Set up Environment Variables:**
    Create a `.env.local` file in the root of the project and add the necessary environment variables for Next.js and Sanity. You will need to get these from your Sanity project dashboard.

    ```env
    # Sanity
    NEXT_PUBLIC_SANITY_PROJECT_ID="..."
    NEXT_PUBLIC_SANITY_DATASET="..."
    NEXT_PUBLIC_SANITY_API_VERSION="..."
    SANITY_API_READ_TOKEN="..."
    SANITY_API_WRITE_TOKEN="..."

    # NextAuth
    AUTH_SECRET="..."
    AUTH_GITHUB_ID="..."
    AUTH_GITHUB_SECRET="..."
    ```

4.  **Run the development server:**
    ```bash
    npm run dev
    ```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

### Sanity Studio

The content management studio is embedded in this application. You can access it at [http://localhost:3000/studio](http://localhost:3000/studio) to manage startup data.