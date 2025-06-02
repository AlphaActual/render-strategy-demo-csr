# Render Strategy Demo - CSR (Client-Side Rendering)

This repository demonstrates Client-Side Rendering (CSR) implementations with modern web frameworks.

## Structure

This repository contains CSR applications built with different frameworks:

### CSR (Client-Side Rendering)

- **CSR/next-app-csr**: Next.js application with Client-Side Rendering
- **CSR/nuxt-app-csr**: Nuxt.js application with Client-Side Rendering  
- **CSR/sveltekit-app-csr**: SvelteKit application with Client-Side Rendering

## What is Client-Side Rendering (CSR)?

Client-Side Rendering is a web development approach where:
- The initial HTML page is minimal (just a shell)
- JavaScript runs in the browser to fetch data and render the content
- The entire application logic runs on the client side
- SEO requires additional considerations (like prerendering)

### Benefits of CSR
- Rich interactive experiences
- Reduced server load after initial delivery
- Great for Single Page Applications (SPAs)
- Smooth transitions between pages

### Considerations
- Initial page load can be slower
- SEO challenges without proper setup
- JavaScript dependency for functionality

## Workspace Setup

This repository is configured as an npm workspace to enable efficient development and deployment optimizations.

### Requirements Met

✅ **GitHub repository**: Connected to GitHub  
✅ **npm workspaces**: Configured with root package.json  
✅ **Package manager lockfile**: package-lock.json at repository root  
✅ **Unique package names**: Each project has a unique name  
✅ **Explicit dependencies**: Dependencies declared in package.json files  

### Available Scripts

```bash
# Development - Individual CSR apps
npm run dev:next-csr     # Start Next.js CSR dev server
npm run dev:nuxt-csr     # Start Nuxt.js CSR dev server  
npm run dev:svelte-csr   # Start SvelteKit CSR dev server

# Development - All CSR apps
npm run dev:csr          # Start all CSR apps

# Build - Individual CSR apps
npm run build:next-csr   # Build Next.js CSR app
npm run build:nuxt-csr   # Build Nuxt.js CSR app
npm run build:svelte-csr # Build SvelteKit CSR app

# Build - All CSR apps
npm run build:csr        # Build all CSR apps

# Install dependencies for all workspaces
npm install
```

### Deployment

With this workspace setup, deployment platforms will:
- Only build projects that have changed
- Skip builds for unaffected projects
- Reduce build queue times
- Optimize resource usage

Each CSR project can be deployed independently while benefiting from monorepo optimizations.

## Getting Started

1. Clone the repository
2. Install dependencies: `npm install`
3. Start development servers: `npm run dev:csr`
4. Visit the applications:
   - Next.js CSR: `http://localhost:3000`
   - Nuxt.js CSR: `http://localhost:3001` 
   - SvelteKit CSR: `http://localhost:5173`
