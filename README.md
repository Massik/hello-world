<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>Mozilla splash page</title>
    <link href='https://fonts.googleapis.com/css?family=Open+Sans:400,700' rel='stylesheet' type='text/css'>
    <style>
      /* header and body setup */

      html {
        font-family: 'Open Sans', sans-serif;
        background: url(pattern.png);
      }

      body {
        width: 100%;
        max-width: 1200px;
        min-width: 360px;
        margin: 0 auto;
        background-color: white;
        position: relative;
      }

      /* Header styling */

      header {
        height: 150px;
      }

      header img {
        width: 100px;
        position: absolute;
        right: 32.5px;
        top: 32.5px;
      }

      h1 {
        font-size: 50px;
        line-height: 140px;
        margin: 0 0 0 32.5px;
      }

      /* main section and video styling */

      main {
        background: #ccc;
      }

      article {
        padding: 20px;
      }

      h2 {
        margin-top: 0;
      }

      p {
        line-height: 2;
      }

      iframe {
        float: left;
        margin: 0 20px 20px 0;
        max-width: 100%;
      }

      /* further info links */

      .further-info {
        clear: left;
        padding: 40px 0;
        background: #c13832;
        box-shadow: inset 0 3px 2px rgba(0,0,0,0.5),
                    inset 0 -3px 2px rgba(0,0,0,0.5);
      }

      .further-info a {
        width: 25%;
        display: block;
        float: left;
      }

      .further-info img {
        max-width: 100%;
      }

      .clearfix {
        clear: both;
      }

      /* Red panda image */

      .red-panda img {
        display: block;
        max-width: 100%;
      }
    </style>
  </head>
  <body>
    <header>
      <h1>Mozilla</h1>
      <!-- insert <img> element, link to the small
          version of the Firefox logo -->
<img src="firefoxlogo120.png">
    </header>

    <main>
      <article>
        <!-- insert iframe from youtube -->
<iframe width="400" height="315" src="https://www.youtube.com/embed/ojcNcvb1olg" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
        <h2>Rocking the free web</h2>

        <p>Mozilla are a global community of technologists, thinkers, and builders, working together to keep the Internet alive and accessible, so people worldwide can be informed contributors and creators of the Web. We believe this act of human collaboration across an open platform is essential to individual growth and our collective future.</p>

        <p>Click on the images below to find more information about the cool stuff Mozilla does. <a href="https://www.flickr.com/photos/mathiasappel/21675551065/">Red panda picture</a> by Mathias Appel.</p>
      </article>

      <div class="further-info">
        <!-- insert images with srcsets and sizes -->
        <a href="https://www.mozilla.org/en-US/firefox/new/">
          <img  srcset="firefoxlogo120.png w120, 
                        firefoxlogo400.png w400"
               sizes=" (max-width:480px) 120px,
                      400px"
               src="firefoxlogo400.png"  alt= "The firefox logo">
        </a>
        <a href="https://www.mozilla.org/">
          <img src="index.svg">
        </a>
        <a href="https://addons.mozilla.org/">
         <img  srcset="firefox-addons120.jpg w120, 
                        firefox-addons400.jpg w400"
               sizes=" (max-width:480px) 120px,
                      400px"
               src="firefox-addons400.jpg"  alt= "Firefox addons">
        </a>
        <a href="https://developer.mozilla.org/en-US/">
          <img  srcset="mozilla-dinosaur120.png w120, 
                        mozilla-dinosaur400.png w400"
               sizes=" (max-width:480px) 120px,
                      400px"
               src="mozilla-dinosaur400.png"  alt="Head of a dinosaur">
        </a>
        <div class="clearfix"></div>
      </div>

      <div class="red-panda">
        <!-- insert picture element -->
          <picture>
              <source media="(max-width=799px)" srcset= "red-panda600.jpg">
              <source media="(min-width=800px)" srcset= "red-panda1200.jpg">
              <img src="red-panda1200.jpg" alt="Big red panda on the tree">
      </div>

    </main>
  </body>
</html>
