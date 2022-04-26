# Installing the B2B Store Theme

B2B Store Theme is a front-end template to help your store get started with VTEX’s core features for businesses selling to other businesses.

## Prerequisites

### Set up your development environment

Before starting with the B2B Store Theme setup itself, you must:

1. [Set up a workspace to develop in VTEX IO](https://developers.vtex.com/vtex-developer-docs/docs/vtex-io-documentation-2-basicsetuptodevelopinvtexio) on your machine.
2. Follow [these instructions](https://developers.vtex.com/vtex-developer-docs/docs/vtex-io-documentation-2-prerequesites) to make sure you meet all the prerequisites to develop using Store Framework.
3. Make sure your store’s catalog is integrated with VTEX Intelligent Search, as described in [this article](https://help.vtex.com/en/tracks/vtex-intelligent-search--19wrbB7nEQcmwzDPl1l4Cb/6wKQgKmu2FT6084BJT7z5V).

### Install required B2B apps

Now you must install the required apps listed below. They are mandatory for the B2B Store Theme to work properly.

- [Wishlist](https://developers.vtex.com/vtex-developer-docs/docs/installing-the-b2b-store-theme#wishlist)
- [Reviews and Ratings](https://developers.vtex.com/vtex-developer-docs/docs/installing-the-b2b-store-theme#reviews-and-ratings)
- [Quick Order](https://developers.vtex.com/vtex-developer-docs/docs/installing-the-b2b-store-theme#quick-order)
- [Location Availability](https://developers.vtex.com/vtex-developer-docs/docs/installing-the-b2b-store-theme#location-availability)
- [Shopper Location](https://developers.vtex.com/vtex-developer-docs/docs/installing-the-b2b-store-theme#shopper-location)
- [Wordpress Integration](https://developers.vtex.com/vtex-developer-docs/docs/installing-the-b2b-store-theme#wordpress-integration)

#### Wishlist

[Wishlist](https://github.com/vtex-apps/wish-list) is an app that allows your store’s customers to bookmark their favorite products by clicking on a heart icon.

To install this app on your store, run the following command on the CLI:

```
vtex install vtex.wish-list@1.x
```

#### Reviews and Ratings

The [Reviews and ratings](https://github.com/vtex-apps/reviews-and-ratings) app enables your clients to submit reviews and ratings — using a star rating system — to your store’s products.

Install it using the command:

```
vtex install vtex.reviews-and-ratings@2.x
```

After that, go to your store's Admin to proceed with the installation.

Once you are logged in, follow these steps:

1. Go to the **Account Settings** module.
2. Click on `Apps`.
3. Then, click on `My apps`.
4. Then, find the **Reviews and Ratings** app card and click on `Settings`.
5. It is recommended that you check the **Display stars in product-rating-summary if there are no reviews** option and uncheck the **Display total reviews number on product-rating-summary block** option, as illustrated below.
6. Click on the `Save` button.

![Reviews and Ratings Settings](/assets/image1.png "Reviews and Ratings Settings")

#### Quick Order

[Quick Order](https://github.com/vtex-apps/quickorder) is an app that enables customers to make bulk orders.

To install it, use the following command:

```
 vtex install vtex.quickorder@3.x
```

#### Location Availability

The [Location Availability](https://github.com/vtex-apps/location-availability) app shows product availability and shipping information in the storefront based on the customer’s location, providing a personalized shopping experience.

Install this app on your store using the `vtex.location-availability@0.x ` command.

#### Shopper Location

[Shopper Location](https://github.com/vtex-apps/shopper-location) is a geolocation app. Once it is installed, the app tracks the customer’s location, after permission is granted.

To install it, use the following command:

```
vtex install vtex.shopper-location@0.x
```

#### Wordpress integration

The [Wordpress integration](https://github.com/vtex-apps/wordpress-integration) app enables the account admin to create content on your store’s front through Wordpress’ API.

To install this app, run the following command on the CLI:

```
vtex install vtex.wordpress-integration@2.x
```

### Install B2B Easy Setup (optional)

If you are setting up a new store, you can follow the instructions in [this guide](https://developers.vtex.com/vtex-rest-api/docs/installing-b2b-easy-set-up) to quickly set up a test store with sample data using the B2B Easy Setup app.

> 🚨 We strongly advise that you do not run Easy Setup on a production environment. It will make irreversible changes and may delete some previous configurations on your store.

## Installation

After following the steps above, you are ready to install the B2B Store Theme. You must:

1. Run the `vtex install vtex.b2bstore@3.x `command on the CLI.
2. Run the `vtex browse` command to see the B2B Store Theme on your browser.

Finally, your storefront should look like this:

![B2B Store Theme](/assets/image3.png "B2B Store Theme")

## Customization

After installing the B2B Store Theme, you can customize it according to your store’s business needs. Check our guide on [Customizing the B2B Store Theme](https://developers.vtex.com/vtex-developer-docs/docs/customizing-the-b2b-store-theme) for more information.
