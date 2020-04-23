# netlify-plugin-pagespeed-insights

> Run Google PageSpeed Insights on your Netlify builds

### Possible flow (wip)
1. Netlify: Get `PUBLISH_DIR` from `constants` ([docs](https://github.com/netlify/build#plugin-constants))
1. Puppeteer: `page.setContent()` passing the built index.html ([docs](https://pptr.dev/#?product=Puppeteer&version=v3.0.1&show=api-pagesetcontenthtml-options))
1. Puppeteer: `page.url()` ([docs](https://pptr.dev/#?product=Puppeteer&version=v3.0.1&show=api-pageurl))
1. PSI: Run PageSpeed Insights on puppeteer url ([docs](https://pptr.dev/#?product=Puppeteer&version=v3.0.1&show=api-pagesetcontenthtml-options))

### Inputs
- Specify contexts to run on; default: `all`
- Specify routes to run on; default: `/`
