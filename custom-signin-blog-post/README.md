# Okta Sign-In Widget Customization for Gen3 Example

This repository shows you how to customize the Okta-hosted Sign-In Widget (SIW) Gen3 to match your brand using design tokens, CSS custom properties, and custom HTML elements.

Please read [Stretch Your Imagination and Build a Delightful Sign-In Experience](https://developer.okta.com/blog/2025/11/08/custom-signin) to see how the `delightful-signin-post.html` customization was created.

Please read [Unlock the Secrets of a Custom Sign-in Page with Tailwind and JavaScript](https://developer.okta.com/blog/2025/11/25/okta-custom-sign-in-page) to see how the `custom-signin-tailwind-alpine-post.html` customization was created.

**Prerequisites:**

- An Okta account with the Identity Engine, such as the [Integrator Free Plan account](https://developer.okta.com/signup/). This code was tested using SIW v7.36.
- Your own domain name
- A basic understanding of HTML, CSS, and JavaScript
- A brand design in mind

> [Okta](https://developer.okta.com/) has Authentication and User Management APIs that reduce development time with instant-on, scalable user infrastructure. Okta's intuitive API and expert support make it easy for developers to authenticate, manage and secure users and roles in any application.

- [Getting Started](#getting-started)
- [Links](#links)
- [Help](#help)
- [License](#license)

## Getting Started

To use this example customization:

### Configure Your Custom Domain

Before you begin, you must configure your Okta org to use your custom domain. Custom domains enable code customizations, allowing you to style more than just the default logo, background, favicon, and two colors.

1. Sign in to your Okta Admin Console
2. Navigate to **Customizations > Brands** and select **Create Brand +**
3. Follow the [Customize domain and email](https://developer.okta.com/docs/guides/custom-url-domain/main/) developer docs to set up your custom domain on the new brand

### Enable SIW Gen3

1. Navigate to your brand's **Settings** tab
2. Select **Use third generation** to enable the SIW Gen3
3. Click **Save**

**NOTE:** The code in this repository relies on using SIW Gen3. It will not work on SIW Gen2.

### Customize Your Sign-In Page

1. Navigate to the **Theme** tab for your brand
2. Configure your primary and secondary colors, logo, and favicon images
3. Select **Sign-in Page** from the dropdown menu
4. Click the **Customize** button
5. On the **Page Design** tab, enable the **Code editor** toggle

**NOTE:** You can only enable the code editor if you configure a [custom domain](https://developer.okta.com/docs/guides/custom-url-domain/).

Replace the page contents with the code found in `custom-signin-post.html`.

### Configure Content Security Policy

To load external resources (such as custom fonts from Google Fonts):

1. Navigate to the **Settings** tab for your brand's Sign-in page
2. Find the **Content Security Policy** section and click **Edit**
3. Add the domains for external resources (e.g., `*.googleapis.com`, `*.gstatic.com`, `https://cdn.jsdelivr.net`)
4. Click **Save to draft** and then **Publish**

## Links

This example demonstrates customization techniques for the following:

- [Okta Sign-In Widget](https://github.com/okta/okta-signin-widget)

## Help

Please post any questions as comments on the [blog posts](https://developer.okta.com/blog/tags/siw-customization), or visit our [Okta Developer Forums](https://devforum.okta.com/).

## License

Apache 2.0, see [LICENSE](LICENSE).