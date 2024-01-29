## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

## Day 1 - Building a Next.js App

Next.js is a React framework that helps launch high performance web applications.

It includes features like...

- Styling: The different ways to style your application in Next.js.
- Optimizations: How to optimize images, links, and fonts.
- Routing: How to create nested layouts and pages using file-system routing.
- Data Fetching: How to set up a database on Vercel, and best practices for fetching and streaming.
- Search and Pagination: How to implement search and pagination using URL Search Params.
- Mutating Data: How to mutate data using React Server Actions, and revalidate the Next.js cache.
- Error Handling: How to handle general and 404 not found errors.
- Form Validation and Accessibility: How to do server-side form validation and tips for improving accessibility.
- Authentication: How to add authentication to your application using NextAuth.js and Middleware.
- Metadata: How to add metadata and prepare your application for social sharing.

Over the next several days, I'm going to be building a Financial Dashboard in Next.js and following along with the tutorial.

You can check out my code here:
https://github.com/ninjasort/ninja-app

![Alt text](public/dashboard.png)

---

The first step to building this Next.js application was to scaffold the project.

You can use create-next-app to do that.
https://nextjs.org/docs/app/api-reference/create-next-app

yarn create next-app@latest nextjs-dashboard
--use-yarn
--example "https://github.com/vercel/next-learn/tree/main/dashboard/starter-example"

## Day 2 - Building a Next.js App

Today I'm going over the folder structure of this Next.js app.

Here's how it breaks down:

- /app: Contains all the routes, components, and logic for your application, this is where you'll be mostly working from.
- /app/lib: Contains functions used in your application, such as reusable utility functions and data fetching functions.
- /app/ui: Contains all the UI components for your application, such as cards, tables, and forms. To save time, we've pre-styled these components for you.
- /public: Contains all the static assets for your application, such as images.
- /scripts: Contains a seeding script that you'll use to populate your database in a later chapter.

![Alt text](public/folder-structure.png)

To get the project up and running we can run `yarn run dev`.

Most of the time we are working in the /app folder.

What's nice about Next.js is that all the routes are based on the folder structure.

/app/dashbaord is the route `/dashboard`
/app/dashboard/invoices is the route `/dashboard/invoices`
