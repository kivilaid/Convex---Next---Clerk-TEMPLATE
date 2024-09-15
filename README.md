# Convex + TypeScript + Next.js + Clerk + Tailwind + shadcn/ui

This template provides a minimal setup to get Convex working with [Next.js](https://nextjs.org/). It uses [Clerk](https://clerk.dev/) for user authentication, [Tailwind CSS](https://tailwindcss.com/) for styling, and [shadcn/ui](https://ui.shadcn.com/) for UI components.

## Getting Started

1. Create a new project using this template:

```
pnpm create convex@latest -t nextjs-clerk-shadcn
```

Then:

1. Follow steps 1 to 3 in the [Clerk onboarding guide](https://docs.convex.dev/auth/clerk#get-started)
2. Paste the Issuer URL as `CLERK_JWT_ISSUER_DOMAIN` to your dev deployment environment variable settings on the Convex dashboard (see [docs](https://docs.convex.dev/auth/clerk#configuring-dev-and-prod-instances))
3. Paste your publishable key as `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY="<your publishable key>"` to the `.env.local` file in this directory.

If you want to sync Clerk user data via webhooks, check out this [example repo](https://github.com/thomasballinger/convex-clerk-users-table/).

3. Start the development server:

```
pnpm run dev
```

## Project Structure

- `convex/`: Convex backend functions and schema
- `app/`: Next.js application code
- `components/`: Reusable React components

## Key Files

- `convex/myFunctions.ts`: Implement your Convex backend functions
- `app/page.tsx`: Main application page

## Customization

Start by editing `convex/myFunctions.ts` to implement your backend logic, and modify `app/page.tsx` to update the frontend UI.

## Additional Resources

- [Convex Documentation](https://docs.convex.dev/home)
- [Next.js Documentation](https://nextjs.org/docs)
- [Clerk Documentation](https://clerk.com/docs)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [shadcn/ui Documentation](https://ui.shadcn.com/)

## Optional: User Data Sync

If you want to sync Clerk user data via webhooks, check out this [example repo](https://github.com/thomasballinger/convex-clerk-users-table/).

## License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).
