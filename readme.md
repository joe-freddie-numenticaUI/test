# FAQ AI Bot Plugin for Strapi

This README provides instructions on how to set up and use the `faq-ai-bot` plugin for your Strapi project. Follow the steps below to integrate and use the plugin in your Strapi application.

## Prerequisites

- A working Strapi project. If you don't have one, you can create it by following the [Strapi documentation](https://strapi.io/documentation).
- Node.js and npm installed on your system.

## Installation and Setup

1. **Create the Plugin**
   - Navigate to your Strapi project directory.
   - Create a new plugin named `faq-ai-bot` by running the following command:
     ```bash
     strapi generate:plugin faq-ai-bot
     ```

2. **Replace Plugin Code**
   - Navigate to the plugin directory:
     ```bash
     cd src/plugins/faq-ai-bot
     ```
   - Replace the contents of the `plugin.ts` file with the provided code for the `faq-ai-bot` plugin.

3. **Install Dependencies**
   - Run the following command to install the required dependencies:
     ```bash
     npm install
     ```

4. **Build the Plugin**
   - Inside the `faq-ai-bot` plugin directory, run the following command to build the plugin:
     ```bash
     npm run build
     ```

5. **Start the Strapi Application**
   - Navigate back to the root of your Strapi project:
     ```bash
     cd ../..
     ```
   - Start the Strapi application in development mode:
     ```bash
     npm run develop
     ```

## Additional Information

For more details on creating and managing plugins in Strapi, refer to the [Strapi Plugin Development Documentation](https://strapi.io/documentation/developer-docs/latest/development/plugins-development.html).

If you encounter any issues or have questions, feel free to reach out to the plugin maintainers or consult the Strapi community for support.
