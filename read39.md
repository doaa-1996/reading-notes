# Next.js

## Assets, Metadata, and CSS


**Assets**

Next.js can serve static assets, like images, under the top-level public directory. Files inside public can be referenced from the root of the application similar to pages.


The public directory is also useful for robots.txt, Google Site Verification, and any other static assets. Check out the documentation for Static File Serving to learn more.


**Download Your Profile Picture**

First, let's retrieve your profile picture.


* Download your profile picture in .jpg format (or use this file).
* Create an images directory inside of the public directory.
* Save the picture as profile.jpg in the public/images directory.
* The image size can be around 400px by 400px.
* You may remove the unused SVG logo file directly under the public directory.


**Unoptimized Image**

With regular HTML, you would add your profile picture as follows:

```
<img src="/images/profile.jpg" alt="Your Name" />
```

**Image Component and Image Optimization**

next/image is an extension of the HTML <img> element, evolved for the modern web.

Next.js also has support for Image Optimization by default. This allows for resizing, optimizing, and serving images in modern formats like WebP when the browser supports it. This avoids shipping large images to devices with a smaller viewport. It also allows Next.js to automatically adopt future image formats and serve them to browsers that support those formats.

Automatic Image Optimization works with any image source. Even if the image is hosted by an external data source, like a CMS, it can still be optimized.

**Using the Image Component**

Instead of optimizing images at build time, Next.js optimizes images on-demand, as users request them. Unlike static site generators and static-only solutions, your build times aren't increased, whether shipping 10 images or 10 million images.

Images are lazy loaded by default. That means your page speed isn't penalized for images outside the viewport. Images load as they are scrolled into viewport.

Images are always rendered in such a way as to avoid Cumulative Layout Shift, a Core Web Vital that Google is going to use in search ranking.


**Metadata**
What if we wanted to modify the metadata of the page, such as the `<title>` HTML tag?

`<title>` is part of the `<head>` HTML tag, so let's dive into how we can modify the `<head>` tag in a Next.js page.

Open pages/index.js in your editor and find the following lines:

```
<Head>
  <title>Create Next App</title>
  <link rel="icon" href="/favicon.ico" />
</Head>
```



Notice that `<Head>` is used instead of the lowercase `<head>`. `<Head>` is a React Component that is built into Next.js. It allows you to modify the `<head>` of a page.

You can import the Head component from the next/head module.

**Adding Head to first-post.js**

We haven't added a `<title>` to our /posts/first-post route. Let's add one.

Open the pages/posts/first-post.js file and add an import for Head from next/head at the beginning of the file:

```
import Head from 'next/head'
```

Then, update the exported FirstPost component to include the Head component. For now, we‘ll add just the title tag:

```
export default function FirstPost() {
  return (
    <>
      <Head>
        <title>First Post</title>
      </Head>
      <h1>First Post</h1>
      <h2>
        <Link href="/">
          <a>Back to home</a>
        </Link>
      </h2>
    </>
  )
}
```


Try accessing http://localhost:3000/posts/first-post. The browser tab should now say “First Post”. By using your browser’s developer tools, you should see that the title tag is added to `<head>`.


**CSS Styling**

As you can see, our index page (http://localhost:3000) already has some styles. If you take a look at pages/index.js, you should see code like this:

```
<style jsx>{`
  …
`}</style>
```


This page is using a library called styled-jsx. It’s a “CSS-in-JS” library — it lets you write CSS within a React component, and the CSS styles will be scoped (other components won’t be affected).

Next.js has built-in support for styled-jsx, but you can also use other popular CSS-in-JS libraries such as styled-components or emotion.


**Layout Component**
First, Let’s create a Layout component which will be shared across all pages.

* Create a top-level directory called components.
* Inside components, create a file called layout.js with the following content:

```
export default function Layout({ children }) {
  return <div>{children}</div>
}
```

Then, open pages/posts/first-post.js, add an import for the Layout component, and make it the outermost component:

```
import Head from 'next/head'
import Link from 'next/link'
import Layout from '../../components/layout'

export default function FirstPost() {
  return (
    <Layout>
      <Head>
        <title>First Post</title>
      </Head>
      <h1>First Post</h1>
      <h2>
        <Link href="/">
          <a>Back to home</a>
        </Link>
      </h2>
    </Layout>
  )
}
```

**Adding CSS**

Now, let’s add some styles to the Layout component. To do so, we’ll use CSS Modules, which lets you import CSS files in a React component.

Create a file called components/layout.module.css with the following content:

```
.container {
  max-width: 36rem;
  padding: 0 1rem;
  margin: 3rem auto 6rem;
}
```

Important: To use CSS Modules, the CSS file name must end with .module.css.

To use this container class inside components/layout.js, you need to:

* Import the CSS file and assign a name to it, like styles
* Use styles.container as the className
* 
Open components/layout.js and replace its content with the following:

```
import styles from './layout.module.css'

export default function Layout({ children }) {
  return <div className={styles.container}>{children}</div>
}
```

**Automatically Generates Unique Class Names**

what CSS Modules does is automatically generates unique class names. As long as you use CSS Modules, so you don’t have to worry about class name collisions.Furthermore, Next.js’s code splitting feature works on CSS Modules as well. It ensures the minimal amount of CSS is loaded for each page. This results in smaller bundle sizes

**Global Styles**

CSS Modules are useful for component-level styles. But if you want some CSS to be loaded by every page, Next.js has support for that as well.

**Styling Tips**

some styling tips that might be helpful:

1. Using classnames library to toggle classes

2. Customizing PostCSS Config

3. Using Sass
