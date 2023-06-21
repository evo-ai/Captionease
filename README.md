# CaptionEase

Tired of manually adding alt text to your product images for better SEO? Let AI do the work for you! CaptionEase is an app that utilizes image recognition AI and natural language generation to automatically generate alt text and product descriptions for your Shopify store.

## Features

CaptionEase offers the following configurable options:

1. Generate image alt text using an image, product description, and title.
2. Generate product descriptions using a product image and title.
3. Generate both a product description and image alt text using an image and product title.

Option 1 leverages Microsoft Azure Computer Vision AI to analyze the image, and GPT-3.5 utilizes the AI's description along with the product description and title to generate descriptive alt text.

Option 2 uses the image description from Computer Vision AI and the product title to update the product description in Shopify.

Option 3 combines Computer Vision AI and GPT-3.5 to generate both the product description and image alt text.

## Frontend Implementation

The frontend of CaptionEase is built using Gadget.dev, React, and the Shopify Polaris design system. The `UseImage.jsx` component provides the embedded app UI where users can configure the app's actions.

## Backend Implementation

CaptionEase's backend logic enables listening to Shopify product image webhooks and generating alt text and descriptions. It utilizes Gadget's Success Effects and Run Effects to handle Shopify Product Image 'create' and 'update' actions. The backend code includes integration with Microsoft Azure Computer Vision API and OpenAI GPT-3.5 for generating alt text and product descriptions.

## Resources

To build CaptionEase, the following resources are required:

- Gadget.dev for Shopify app backend and frontend (free)
- Shopify Partners account for Shopify dev store (free)
- OpenAI developer API key (usage cost)
- Microsoft Azure developer API key (usage cost)
- OpenAI NPM package (free)

Refer to the code and resources provided in this repository to build your own instance of CaptionEase.
