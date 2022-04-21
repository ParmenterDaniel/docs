---
title: Google Ads Authentication
sidebar: cyclr_sidebar
permalink: google-ads-connector
tags: [connector]
---

# Google Ads set up

You need to do the following to enable Google Ads access for the Google Ads connector:

1. Enable the Google Ads API for a project within your workspace.
2. Obtain your **client ID** and **client secret** by setting up OAuth 2.0 credentials.
3. Obtain your **developer token** for your Google Ads account.
4. Obtain your **client customer ID** for your Google Ads client account.

### Enabling the Google Ads API

To access the Google Ads API endpoints, you need to enable the Google Ads API within a project in your workspace. Google’s documentation on how to do this can be found [here](https://support.google.com/googleapi/answer/6158841?hl=en).

### Obtaining your client ID and client secret

You need a **client ID** and **client secret** to set up the Google Ads connector in Cyclr. You can obtain these by creating OAuth 2.0 credentials for the Google project where you enabled the Google Ads API in the previous step. Google's documentation on how to do this can be found [here](https://support.google.com/cloud/answer/6158849?hl=en). You need to set up the fields below as follows:

-   **Authorised redirect URIs**: Your Cyclr callback URL e.g. https://{Your Cyclr service domain e.g. app-h.cyclr.com}/connector/callback

Once you have created OAuth 2.0 credentials, make note of the **client ID** and **client secret** as you need both needed to set up the Google Ads connector in Cyclr.

### Obtaining your developer token

You need a Google Ads **developer token** to set up the Google Ads connector in Cyclr. Google's documentation on how to get this can be found [here](https://developers.google.com/google-ads/api/docs/first-call/dev-token).

### Obtaining your client customer ID

You need your **client customer ID** to set up the Google Ads connector in Cyclr. Google's documentation on how to get this can be found [here](https://support.google.com/google-ads/answer/1704344?hl=en-GB).

# Cyclr set up

### Client installation

When using a template containing the Google Ads connector, clients will be prompted for the following information from the previous sections:

-   **Client ID**: The **client ID** they obtained from setting up OAuth 2.0 authentication in their Google project.
-   **Client secret**: The **client secret** they obtained from setting up OAuth 2.0 authentication in their Google project.
-   **Developer token**: The **developer token** they obtained from their Google Ads account.
-   **Client customer ID**: The **client customer ID** of the account they want to manage the API.

### Partner templates

To set up the Google Ads connector within a template:

1. Go to the **Cyclr Console**.
2. Click the **Templates** dropdown menu at the top of the page.
3. Click **Template Library**.
4. Click **Design New Template** and enter a **Template Name** to create a new template, or click **Edit Most Recent Draft** to change an existing template.
5. Click **+Add Application** in the right-hand menu.
6. Use the search bar to find the **Google Ads** connector and click **Install**.
7. Change the **Name** and **Description** as required and click **Next**.
8. Enter the following values from the previous sections:
    - **Client ID**: Your **client ID** you obtained from setting up OAuth 2.0 authentication for your Google project.
    - **Client secret**: Your **client secret** you obtained from setting up OAuth 2.0 authentication for your Google project.
    - **Developer token**: Your **developer token** you obtained from your Google Ads account.
    - **Client customer ID**: Your **client customer ID** of the account you want to manage the API.
9. Click **Next**.

Your Google Ads connector is now set up! You can test it by running a method within the template it’s installed in to confirm it returns data.