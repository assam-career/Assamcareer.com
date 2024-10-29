# Assamcareer.com
A premier website for latest government and private jobs in Assam, admission, admit card, competitive exam, results and scholarships related news.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title><data:blog.title/></title>
    <meta name="description" content="Your site's description here" />
    <meta name="author" content="Your Name or Site Name" />

    <!-- Open Graph Meta Tags -->
    <meta property="og:title" content="<data:blog.title/>" />
    <meta property="og:description" content="Brief description of the content" />
    <meta property="og:type" content="website" />
    <meta property="og:url" content="<data:blog.homepageUrl/>" />
    <meta property="og:image" content="https://yourwebsite.com/path/to/image.jpg" />

    <!-- Twitter Card Meta Tags -->
    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:title" content="<data:blog.title/>" />
    <meta name="twitter:description" content="Brief description of the content" />
    <meta name="twitter:image" content="https://yourwebsite.com/path/to/image.jpg" />

    <!-- JSON-LD Structured Data for Articles -->
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "BlogPosting",
      "mainEntityOfPage": {
        "@type": "WebPage",
        "@id": "<data:blog.homepageUrl/>"
      },
      "headline": "<data:post.title/>",
      "description": "<data:post.snippet/>",
      "image": "https://yourwebsite.com/path/to/image.jpg",
      "author": {
        "@type": "Person",
        "name": "Your Name"
      },
      "publisher": {
        "@type": "Organization",
        "name": "Your Site Name",
        "logo": {
          "@type": "ImageObject",
          "url": "https://yourwebsite.com/path/to/logo.jpg"
        }
      },
      "datePublished": "<data:post.date/>",
      "dateModified": "<data:post.date/>"
    }
    </script>
    
    <!-- Blogger Skin Tag for CSS (Optional) -->
    <b:skin>
        <![CDATA[
        /* Your CSS styling here */
        ]]>
    </b:skin>
</head>
<body>

    <!-- Header Section -->
    <header>
        <h1><data:blog.title/></h1>
        <p><data:blog.description/></p>
    </header>

    <!-- Main Content Area -->
    <main>
        <div class="content">
            <b:loop values="data:posts" var="post">
                <article>
                    <h2><a expr:href="data:post.url"><data:post.title/></a></h2>
                    <p><data:post.snippet/></p>
                </article>
            </b:loop>
        </div>
    </main>

    <!-- Footer Section -->
    <footer>
        <p>&#169; <data:blog.title/> - All Rights Reserved</p>
    </footer>

</body>
</html>
