# Search Engine Optimization (SEO)

> This is a SEO cheat sheet repository

Search Engine Optimization (SEO) is the process of optimizing a website or web page to improve its visibility and ranking in search engine results pages (SERPs). By optimizing your website for search engines, you can increase the chances of your website appearing at the top of the SERPs for relevant keywords, which can lead to more traffic and higher conversion rates.

## Table of Contents

- [Key Elements of SEO](#key-elements-of-seo)
- [Tips for SEO Success](#tips-for-seo-success)
- [What are web crawlers?](#what-are-web-crawlers)
- [How does Googlebot work?](#how-does-googlebot-work)
- [HTTP Status Codes](#http-status-codes)
- [robots.txt file](#robotstxt-file)
- [XML Sitemaps](#xml-sitemaps)
- [Special Meta Tags for Search Engines](#special-meta-tags-for-search-engines)
  - [Googlebot tag](#googlebot-tag)
- [Canonical Tags](#canonical-tags)
- [Rendering Strategies](#rendering-strategies)
- [URL Structure](#url-structure)
- [Important meta tags for SEO](#important-meta-tags-for-seo)
- [Open Graph Protocol](#open-graph-protocol)
- [Page Structure](#page-structure)
- [Core Web Vitals](#core-web-vitals)
- [LightHouse](#lighthouse)

## Key Elements of SEO

- **Keyword research:** Identifying the keywords and phrases that your target audience is searching for and incorporating them into your website's content, meta tags, and URLs.

- **On-page optimization:** Optimizing the content, structure, and code of your website to ensure it is easily crawlable and understandable by search engines.

- **Off-page optimization:** Building high-quality backlinks from other websites to improve your website's authority and visibility in the SERPs.

- **Technical SEO:** Ensuring that your website is technically sound and able to be crawled and indexed by search engines.

- **Measuring and Tracking:** Analyzing your website's performance in the SERPs and using tools such as Google Analytics to track your website's traffic and conversions.

## Tips for SEO Success

1. Create high-quality and unique content that provides value to your audience.

2. Use header tags (H1, H2, etc.) to structure your content and make it easily readable.

3. Optimize your images and videos by using descriptive file names and alt tags.

4. Use internal linking to help search engines understand the structure of your website.

5. Create a sitemap and submit it to search engines.

6. Use social media to promote your website and build back links.

7. Make sure your website is mobile-friendly and has a fast loading time.

8. Monitor your website's performance in the SERPs and make adjustments as needed.

> **Note:**
>
> - SEO is not a one-time process, it requires continuous effort and monitoring to stay ahead of the competition.
> - It is important to follow the guidelines and best practices of search engines and avoid manipulative tactics that can get your website penalized.
> - SEO results take time and patience, it is not a quick fix solution.
> - It is important to stay updated with the latest SEO trends, algorithms updates and best practices.

## What are web crawlers?

Web crawlers, also known as spiders, bots, or web robots, are automated programs that crawl the web to index content for search engines. They follow links from one page to another and collect information about the content on each page. The information collected by web crawlers is used to build search engine indexes.

> Note: Googlebot is the web crawler used by Google.

## How does Googlebot work?

1. **Find URLs:** Googlebot finds new URLs by following links from one page to another.

2. Add to Crawl Queue: Googlebot adds the URLs to a crawl queue to be crawled.

3. **HTTP Request:** The crawler makes an HTTP request to get the headers and acts according to the returned status code:

4. **Render Queue:** If the page has some JavaScript client-side based content, the URLs might be added to a Render Queue. Render Queue is more costly for Google as it needs to use more resources to render JavaScript and therefore URLs rendered are a smaller percentage over the total pages out there on the internet.

5. **Ready to be indexed:** If all criteria are met, the pages may be eligible to be indexed and shown in search results.

## HTTP Status Codes

- [HTTP Status Codes](https://github.com/emanuelefavero/http-status-codes)

## robots.txt file

- [robots.txt](https://github.com/emanuelefavero/robots-txt-templates-)

## XML Sitemaps

- [XML Sitemaps](https://github.com/emanuelefavero/xml-sitemaps)

## Special Meta Tags for Search Engines

Meta robot tags are directives that search engines will always respect. Adding these robots tags can make the indexation of your website easier.

- **Noindex:** This tag tells search engines not to index the page. This is useful for pages that are not ready to be indexed, such as pages that are under construction or settings pages and more

- **Nofollow:** This tag tells search engines not to follow the links on the page

  ```html
  <meta name="robots" content="noindex, nofollow" />
  ```

### Googlebot tag

- **Googlebot:** This tag tells Google not to index or follow the page

  ```html
  <meta name="googlebot" content="noindex, nofollow" />
  ```

- **nositelinkssearchbox:** This tag tells Google not to show the sitelinks search box for the page

  ```html
  <meta name="googlebot" content="nositelinkssearchbox" />
  ```

- **notranslate:** This tag tells Google not to translate the page

  ```html
  <meta name="google" content="notranslate" />
  ```

> Full list of Googlebot meta tags: [Googlebot Meta Tags](https://developers.google.com/search/docs/crawling-indexing/robots-meta-tag#directives)

## Canonical Tags

A canonical URL is the URL of the page that search engines think is most representative from a set of duplicate pages on your site.

> It is useful to use canonical tags when you have multiple URLs that point to the same page.

```html
<link rel="canonical" href="https://www.example.com/" />
```

## Rendering Strategies

This is a list of rendering strategies from the most SEO friendly to the least.

- **Static Site Generation** (SSG): The content is generated at build time and served as static files. This is the most SEO friendly rendering strategy.

- **Server Side Rendering** (SSR): The content is generated at request time and served as HTML.

- **Incremental Static Regeneration** (ISR): Use static generation on a per-page basis. Learn more about [Incremental Static Regeneration in Next.js](https://nextjs.org/docs/basic-features/data-fetching/overview#incremental-static-regeneration).

- **Client Side Rendering** (CSR): The content is generated at request time and served as JavaScript. This is the least SEO friendly rendering strategy but sometimes it is the only option.

## URL Structure

- **Use hyphens (-) instead of underscores (\_):** Hyphens are easier to read and are more SEO friendly.

- **Use lowercase:** URLs are case sensitive, using lowercase URLs is more SEO friendly.

- **Use descriptive URLs:** URLs should be descriptive and easy to understand.

- **Use short:** Short URLs are easier to read and are more SEO friendly.

- **Semantic:** URLs should be semantic and easy to understand.

- **logical and consistent patterns:** URLs should follow a logical pattern.

- **Avoid URL parameters:** URL parameters are not SEO friendly.

- **Keyword focused:** URLs should be keyword focused.

## Important meta tags for SEO

- **title:** The title tag is the most important on-page SEO element.

- **description**

- **keywords**

## Open Graph Protocol

The Open Graph protocol enables any web page to become a rich object in a social graph. For instance, this is used on Facebook to allow any web page to have the same functionality as any other object on Facebook.

- **og:title:** The title of your object as it should appear within the graph, e.g., "The Rock".

```html
<meta property="og:title" content="The Rock" />
```

- **og:type:** The type of your object, e.g., "video.movie". Depending on the type you specify, other properties may also be required.

```html
<meta property="og:type" content="video.movie" />
```

- **og:image:** An image URL which should represent your object within the graph.

```html
<meta property="og:image" content="http://example.com/rock.jpg" />
```

- **og:url:** The canonical URL of your object that will be used as its permanent ID in the graph, e.g., "http://www.imdb.com/title/tt0117500/".

```html
<meta property="og:url" content="http://www.imdb.com/title/tt0117500/" />
```

- **og:description:** A one to two sentence description of your object.

```html
<meta
  property="og:description"
  content="lorem ipsum dolor sit amet, consectetur adipiscing elit."
/>
```

> Learn more about [Open Graph Protocol](https://ogp.me/)

## Page Structure

- **Use H1 tag only once per page:** The H1 tag is the most important tag for SEO. It should be used only once per page.

- **Internal links:** Internal links are links that point to other pages on the same website.

- **External links:** External links are links that point to other websites.

### the PageRank Algorithm

The PageRank algorithm is an algorithm used by Google Search to rank websites in their search engine results.
This algorithm goes through every link on a database and scores domains based on how many links they receive (quantity) and from which domains (quality)

> Learn more about [PageRank Algorithm](https://web.stanford.edu/class/cs54n/handouts/24-GooglePageRankAlgorithm.pdf)

## Core Web Vitals

Core Web Vitals are a set of metrics that measure the performance and user experience of a web page. These metrics include:

- **First Contentful Paint (FCP):** measures the time from when the user requests a page to when any visible content is rendered on the screen.
- \*\*Speed Index: measures how quickly the content of a page is visibly populated.
- **Time to Interactive (TTI):** measures the time from when the user requests a page to when the page is fully interactive.
- \*\*Largest Contentful Paint (LCP): measures the render time of the largest element visible in the viewport.
- **Total Blocking Time (TBT):** measures the total amount of time between FCP and TTI that is blocked by long tasks.
- **Cumulative Layout Shift (CLS):** measures the layout shift of visible elements within the viewport.

These metrics are important because they directly affect the user's perception of performance and can lead to higher bounce rates if they are not met.

To measure and improve your Core Web Vitals, you can use tools such as Google's PageSpeed Insights, Lighthouse, and Chrome DevTools.

You can also use the Web Vitals JavaScript library to measure the Core Web Vitals on your website and track them over time.

To improve your Core Web Vitals, you can:

- Minimize the use of third-party scripts and iframes
- Reduce the size of images and other resources
- Defer the loading of non-critical resources
- Optimize your code to reduce the time spent in long tasks
- Use web workers to offload heavy computation to background threads
- Use a Content Delivery Network (CDN) to reduce the time to first byte.

> Learn more about [Core Web Vitals](https://nextjs.org/learn/seo/web-performance)

## Lighthouse

Lighthouse is an open-source, automated tool for improving the quality of web pages. It can be run as a Chrome extension, from the command line, or as a Node.js module. It audits a page and generates a report on its performance, accessibility, best practices, and SEO.

### Features

- **Performance:** Lighthouse measures the loading performance of a page, including the time to first contentful paint, time to interactive, and speed index.
- **Accessibility:** Lighthouse audits a page for accessibility issues, such as missing alternative text for images and proper use of ARIA attributes.
- **Best Practices:** Lighthouse checks a page for best practices, such as the use of HTTPS and avoiding the use of deprecated APIs.
- **SEO:** Lighthouse audits a page for SEO issues, such as the presence of a valid robots.txt file and structured data.

### Usage

> Note: Remember to use Lighthouse in a private window to avoid any caching issues or extension slow down

#### Chrome Extension

1. Install the Lighthouse Chrome extension from the [Chrome Web Store](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk)
2. Go to the web page you want to audit
3. Click on the Lighthouse icon in the Chrome extension bar
4. Click on "Generate Report" and wait for the report to be generated
5. Review the report and take action on any issues that are identified

#### Command Line

1. Install Lighthouse globally by running `npm install -g lighthouse`
2. Run Lighthouse on a web page by running `lighthouse <url>`
3. Review the report and take action on any issues that are identified

#### Node.js

1. Install Lighthouse by running `npm install lighthouse`
2. Use Lighthouse in your Node.js code by requiring the module and running the `lighthouse` function:

```js
const lighthouse = require('lighthouse')
const report = await lighthouse('<url>')
console.log(report)
```

&nbsp;

---

&nbsp;

[**Go To Top &nbsp; ⬆️**](#table-of-contents)
