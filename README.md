```bash
git clone https://github.com/shcube08/nextjs14-notion.git
```

**Step 2:**

Execute the following command in the root directory of the downloaded repo in order to install dependencies:

```bash
npm install
```

**Step 3:**

Execute the following command in order to run the development server locally:

```bash
npm run dev
```

**Step 4:**

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

### 📜 Scripts

All scripts are defined in the `package.json` file. Here is a list of all scripts:

| Script          | Action                                      |
| :-------------- | :------------------------------------------ |
| `npm install`   | Installs dependencies                       |
| `npm run dev`   | Starts local dev server at `localhost:3000` |
| `npm run build` | Build your production site to `./dist/`     |
| `npm run start` | Start your production site locally          |
| `npm run lint`  | Run ESLint                                  |

## 🔒 Environment Variables

Environment variables[^6] can be used for configuration. They must be set before running the app.

> [Environment variables](https://en.wikipedia.org/wiki/Environment_variable) are variables that are set in the operating system or shell, typically used to configure programs.

**Notion** uses [Convex](https://appwrite.io), and [Clerk](https://clerk.com) as external services. You need to create an accounts on Convex and Clerk and get the required credentials to run the app.

Create a `.env` file in the root directory of the project and add the following environment variables:

```env
CONVEX_DEPLOY_KEY=<CONVEX_DEPLOY_URL>
NEXT_PUBLIC_CONVEX_URL=<NEXT_PUBLIC_CONVEX_URL>

CLERK_PUBLISHABLE_KEY=<CLERK_PUBLISHABLE_KEY>
CLERK_SECRET_KEY=<CLERK_SECRET_KEY>

EDGE_STORE_ACCESS_KEY=<EDGE_STORE_ACCESS_KEY>
EDGE_STORE_SECRET_KEY=<EDGE_STORE_SECRET_KEY>
```

## 🚀 Deployment

#### Deploy to production (manual)

You can create an optimized production build with the following command:

```bash
npm run build
```

#### Deploy on Vercel (recommended)
