---
title: Getting started
description: Get started with the astro-sdk SDK with a step-by-step guide
category: Getting started
position: 0
---

This documentation will walk you through how to:

- Set up a astro-sdk account.
- Install astro-sdk SDK into your project.
- Create a astro-sdk instance to use through your project.

---

## Account setup

Before installing astro-sdk SDK, you will first need to create a astro-sdk Account to get your API credentials.

1. Sign up for a astro-sdk Account [here](#/signup).
2. Navigate to the developer section under settings [here](#/settings/developer).
3. Obtain your generated [public](/docs/sdk/concepts#public-keys) and [secret keys](/docs/sdk/concepts#secret-keys).

---

## Installation

### Prerequisites

The only requirement for using astro-sdk SDK is to have Node.js (version 16 or higher) installed on your machine.

### Install the SDK with a package manager

If you're using npm or yarn, then adding the astro-sdk SDK to your project is really simple. Once you've created a
directory for your project, navigate into your project's root folder in your terminal `cd your-project-folder`, and type
the following:

```bash
npm install astro-sdk
# or
yarn add astro-sdk
```

<div class="highlight highlight--note">
    <span>Note</span>
    <p>Note that examples provided using the astro-sdk SDK are using the latest version - available on <a href="https://www.npmjs.com/package/astro-sdk">npm</a>.</p>
</div>

### Instantiate astro-sdk with your API key

We're almost ready to go! We need to create a new astro-sdk instance and give it our [public
key](/docs/sdk/concepts#scope) (you can get your API keys from [astro-sdk Dashboard > Settings >
Developer](#/settings/developer)).

<div class="highlight highlight--info">
    <span>Tip</span>
    <p>For more information on API keys authentication, read more on <a href="/docs/sdk/concepts#authentication">how we authenticate astro-sdk core endpoints</a>.</p>
</div>

```js
// Import the astro-sdk module
import astro-sdk from 'astro-sdk';

// Create a astro-sdk instance
const astro-sdk = new astro-sdk('{public_api_key}');
```

<div class="highlight highlight--note">
    <span>Note</span>
    <p>We've built in a console debugger into the astro-sdk SDK to help with debugging during development. To enable the debugger you can include the second argument <code>true</code> when you create your astro-sdk instance like so: <code>const astro-sdk = new astro-sdk('{public_api_key}', true);</code>. Note that a test API key has to be provided as the first argument for the console to show messages - it won't work with a live key.</p>
</div>

Awesome, you have set up your astro-sdk Account, installed the astro-sdk SDK and created your first astro-sdk instance! You
now have access to the `astro-sdk` object in your application to build out a truly unique frontend presentation layer!

---

### Next steps

Browse through the rest of our documentation to explore all the features of astro-sdk SDK - [listing
products](/docs/sdk/products#list-products), [add products to cart](/docs/sdk/cart#add-to-cart), or [capture an
order](/docs/sdk/checkout#capture-order). Note that all requests made using the astro-sdk SDK will have responses that
are returned asynchronously in a promise. Alternatively, if you want to dive more into reading a high-level overview of
astro-sdk SDK and its features, read more [here](/product/features).

<div class="highlight highlight--warn">
    <span>Important</span>
    <p>Please note that for all the following SDK documentation on  <b>Products</b>, <b>Cart</b>, and <b>Checkout</b>, we import <code>astro-sdk</code> in every example using astro-sdk SDK for the sake of brevity. In practice, you would follow the example of creating and exporting out your astro-sdk client in a file such as <code>/lib/astro-sdk SDK</code>.</p>
</div>

---
