# Class 41
# React 4
**Reading Questions :**

1.
## Static Routes:

Static routes are routes where the content of a page remains constant and does not change based on user input or other dynamic factors. When you create a static route in Next.js, the content for that route is pre-rendered at build time. This means that the HTML, CSS, and JavaScript for the page are generated ahead of time, and when a user visits the page, they are served this pre-generated content directly from the server. This approach is efficient for pages that don't require frequent updates and are the same for all users.

## Dynamic Routes:

Dynamic routes, on the other hand, allow you to create routes whose content can change based on dynamic data or user input. These routes are generated at runtime, not during the build process. Dynamic routes are defined using placeholders in the route's path, indicated by square brackets (e.g., pages/posts/[id].js). These placeholders can capture values from the URL and be used to fetch data or customize the content of the page.

When a user requests a dynamic route, Next.js will handle the routing, capture the dynamic segment from the URL, and pass it as a parameter to the corresponding page component. This component can then use the captured value to fetch relevant data from a database, API, or any other data source. This approach allows you to create pages that display different content based on the provided dynamic parameter.

## Differences between Dynamic and Static Routes:

### Content Generation:

- Static routes generate the content at build time and serve the same content to all users.
- Dynamic routes generate content at runtime based on user input or dynamic data, allowing for customized content.

### Data Fetching:

- Static routes can also fetch data during the build process using functions like `getStaticProps`, which allows you to pre-render data for static pages.
- Dynamic routes commonly use functions like `getServerSideProps` or `getStaticProps` with dynamic parameters to fetch data based on the specific request.

### URL Structure:

- Static routes have a fixed URL structure.
- Dynamic routes have a flexible URL structure that can include placeholders for dynamic segments.

### Use Cases:

- Static routes are suitable for content that doesn't change frequently and is the same for all users.
- Dynamic routes are useful when you need to show different content based on parameters like IDs, usernames, or other dynamic data.

2.
 **Build Your Next.js Application:**

- Develop your Next.js application.
- Update profile image, name, and self-introduction.

 **Push to GitHub:**

- Create a new repository on GitHub named "nextjs-blog."
- Initialize Git repository locally if not done already.
- Push your Next.js app to the GitHub repository.

 **Deploy to Vercel:**

- Create a Vercel account at [https://vercel.com/signup](https://vercel.com/signup).
- Import your GitHub repository on Vercel ([https://vercel.com/import/git](https://vercel.com/import/git)).
- Install Vercel for GitHub and import your app.
- Vercel will automatically detect Next.js and configure optimal build settings.
- Wait for the build process to complete (usually under a minute).
- Access the deployment URLs provided by Vercel.

**Optional: Preview Deployment for Every Push:**

- Create a new branch on GitHub.
- Make changes, push, and create a pull request.
- Vercel automatically creates a preview deployment for the branch.
- Share the preview URL for feedback.
- Merge the pull request to trigger a production deployment.

**Other Hosting Options (Alternative to Vercel):**

- Deploy to any hosting provider that supports Node.js.
- Build the application using `npm run build`.
- Start the server using `npm run start`.

3. Next.js handles static file serving through a "public" directory in the project's root. This directory stores static assets like images and stylesheets. When referencing these assets in your code, you can use the "/public" path as the base URL, and Next.js will handle the correct URL paths during runtime. This approach allows for efficient serving of static files without going through the Next.js server. During production builds, Next.js automatically adds unique hashes to filenames for cache optimization. Customization of static asset serving behavior can be done through the "next.config.js" file.



## Things I want to know more about
  **Next.js - Static File Serving**
