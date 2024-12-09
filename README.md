## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

## For Datebase connection
if you connect database you use "https://nextjs.org/learn/dashboard-app/setting-up-your-database" and adding .env file for your database connection we use potgressql on vercel this education.

## Static and Dynamic Rendering
## -What is Static Rendering?
With static rendering, data fetching and rendering happens on the server at build time (when you deploy) or when revalidating data.

Whenever a user visits your application, the cached result is served. There are a couple of benefits of static rendering:

Faster Websites - Prerendered content can be cached and globally distributed. This ensures that users around the world can access your website's content more quickly and reliably.
Reduced Server Load - Because the content is cached, your server does not have to dynamically generate content for each user request.
SEO - Prerendered content is easier for search engine crawlers to index, as the content is already available when the page loads. This can lead to improved search engine rankings.
Static rendering is useful for UI with no data or data that is shared across users, such as a static blog post or a product page. It might not be a good fit for a dashboard that has personalized data which is regularly updated.

The opposite of static rendering is dynamic rendering.

## -What is Dynamic Rendering?
With dynamic rendering, content is rendered on the server for each user at request time (when the user visits the page). There are a couple of benefits of dynamic rendering:

Real-Time Data - Dynamic rendering allows your application to display real-time or frequently updated data. This is ideal for applications where data changes often.
User-Specific Content - It's easier to serve personalized content, such as dashboards or user profiles, and update the data based on user interaction.
Request Time Information - Dynamic rendering allows you to access information that can only be known at request time, such as cookies or the URL search parameters.

## -Streaming ?

Sayfalarda bulunanan dinamik ve statik sayfa yapısına uygun olarak veriler gelirkenki gecikmeyi son kullanıcıya fark ettirmemek açısından sayfa da bulunan componentlerin sayfaya iskelet olarak gelmesi ve yükleniyor muş gibi görünmesi olayı.

Skeleton ve Suspense bu partta kullanılan önemli kelimeler.

## -Partial Rendering ?

Basit şekilde dinamik ve statik işlemlerin avatajlarını birleştirerek aynı sayfada kullanma olayı.

## -Search and Pagination ?

Debouncing: Veritabanına yollanan istek sayısını azaltabilir böylece kaynak tasarrufu yapabilirsiniz. Yani bir arama yaparken her tuşa bastığınıza arama yapmayı engeller belli bir saniye bekler ve o saniyeye kadar yazılan kelime yada cümle üzerinden arama yapar.