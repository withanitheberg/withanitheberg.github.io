<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Landing Page</title>

  <style>
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
        sans-serif;
      line-height: 1.5;
      background: #0b0b0b;
      color: #f9fafb;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .page {
      width: 100%;
      max-width: 600px;
      padding: 1.5rem;
      text-align: center;
    }

    .hero-image {
      width: 100%;
      height: auto;
      display: block;
      margin: 0 auto 1.5rem;
      border-radius: 0.5rem;
    }

    h1 {
      font-size: 1.6rem;
      margin-bottom: 0.75rem;
    }

    p {
      margin-bottom: 1rem;
      color: #d1d5db;
    }

    /* Optional: simple Mailchimp form styling override */
    form {
      margin-top: 1rem;
    }

    input[type="email"] {
      width: 100%;
      max-width: 100%;
      padding: 0.6rem 0.75rem;
      border-radius: 0.35rem;
      border: 1px solid #4b5563;
      margin-bottom: 0.75rem;
      font-size: 0.95rem;
    }

    input[type="submit"] {
      padding: 0.6rem 1.1rem;
      border-radius: 0.35rem;
      border: none;
      background: #f97316;
      color: #111827;
      font-weight: 600;
      cursor: pointer;
      font-size: 0.95rem;
    }

    input[type="submit"]:hover {
      background: #ea580c;
    }

    small {
      display: block;
      margin-top: 0.5rem;
      font-size: 0.75rem;
      color: #9ca3af;
    }
  </style>
</head>
<body>
  <div class="page">
    <!-- Image -->
    <img
      src="hero.jpg"
      alt="Landing page image"
      class="hero-image"
    />

    <!-- Optional title/text above form -->
    <h1>Stay in the loop</h1>
    <p>Join the email list to get updates and announcements.</p>

    <!-- Begin Mailchimp form -->
    <!--
      1. In Mailchimp go to:
         Audience → Signup forms → Embedded forms → Copy the code.
      2. Paste it here, replacing this whole commented block.
      3. You can keep or remove the extra CSS Mailchimp includes.
    -->

    <form
      action="YOUR_MAILCHIMP_POST_URL_HERE"
      method="post"
      target="_blank"
      novalidate
    >
      <label for="mce-EMAIL" class="visually-hidden">Email address</label>
      <input
        type="email"
        value=""
        name="EMAIL"
        id="mce-EMAIL"
        placeholder="Enter your email"
        required
      />
      <input
        type="submit"
        value="Subscribe"
        name="subscribe"
      />
      <small>No spam. Unsubscribe anytime.</small>
    </form>

    <!-- End Mailchimp form -->
  </div>
</body>
</html>
