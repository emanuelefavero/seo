# Search Engine Optimization (SEO)

> This is a SEO cheat sheet repository

Search Engine Optimization (SEO) is the process of optimizing a website or web page to improve its visibility and ranking in search engine results pages (SERPs). By optimizing your website for search engines, you can increase the chances of your website appearing at the top of the SERPs for relevant keywords, which can lead to more traffic and higher conversion rates.

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
