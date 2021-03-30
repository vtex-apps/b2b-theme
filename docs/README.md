# B2B Store Theme

<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [Prerequisites](#prerequisites)
  - [Toolbelt](#toolbelt)
  - [Change Store Edition](#change-store-edition)
  - [Easy Setup App (Optional)](#easy-setup-app-optional)
  - [Setup Search](#setup-search)
    - [Setup Search Indexer](#setup-search-indexer)
- [Theme](#theme)
  - [Peer Dependencies](#peer-dependencies)
  - [Setup Organizations Apps](#setup-organizations-apps)
    - [Install Apps](#install-apps)
    - [Update CL Entity](#update-cl-entity)
  - [Setup Reviews and Ratings](#setup-reviews-and-ratings)
- [Preview](#preview)

<!-- /code_chunk_output -->

## Prerequisites

### Toolbelt

Follow this [Developer Docs Guide](https://developers.vtex.com/vtex-developer-docs/docs/vtex-io-documentation-2-basicsetuptodevelopinvtexio) to setup **Toolbelt** and have access to CLI commands.

### Change Store Edition

Follow the steps required to setup `vtex.edition-store@3.x` detailed in this [Developer Docs Guide](https://developers.vtex.com/vtex-developer-docs/docs/vtex-io-documentation-2-prerequesites#implementing-the-correct-edition-app)

### Easy Setup App (Optional)

If you want to setup your environment with products, categories and other resources, take a look at [Easy Setup App](https://github.com/beightone/easy-setup)

### Setup Search

Follow the steps detailed in the section [Implementing the VTEX Intelligent Search](https://developers.vtex.com/vtex-developer-docs/docs/vtex-io-documentation-2-prerequesites#implementing-the-vtex-intelligent-search) of the Prerequisites for Store Framework development guide.

#### Setup Search Indexer

Go to: **STORE SETUP** &rarr; **Search** &rarr; **Integration settings** (`https://{{account}}.myvtex.com/admin/search/integration-settings`) and click "Start Integration"

![Screen Shot 2021-02-18 at 08.31.00](/assets/Screen%20Shot%202021-02-18%20at%2008.31.00.png)

Wait until all the steps are completed.

![Screen Shot 2021-02-18 at 08.32.31](/assets/Screen%20Shot%202021-02-18%20at%2008.32.31.png)

## Theme

### Peer Dependencies

Install B2B Store Theme peer dependencies:

```sh
vtex install \
    vtex.wish-list@1.x \
    vtex.reviews-and-ratings@2.x \
    vtex.quickorder@3.x \
    vtex.location-availability@0.x \
    vtex.shopper-location@0.x \
    vtex.orderquote@1.x \
    vtex.wordpress-integration@2.x
```

![Screen Shot 2021-02-25 at 09.48.10](/assets/Screen%20Shot%202021-02-25%20at%2009.48.10.png)

Accept all terms of use/service

![Screen Shot 2021-02-25 at 09.48.17](/assets/Screen%20Shot%202021-02-25%20at%2009.48.17.png)

### Setup Organizations Apps

#### Install Apps

```sh
vtex install \
    vtex.admin-organizations@1.x \
    vtex.organizations@1.x
```

![Screen Shot 2021-02-25 at 09.56.25](/assets/Screen%20Shot%202021-02-25%20at%2009.56.25.png)

Go to: **ACCOUNT SETTINGS** &rarr; **Authorizations** &rarr; **All Permissions** (`https://{{account}}.myvtex.com/admin/authorization/permissions`)

If you opted out to use [Easy Setup App](#easy-setup-app-optional) and selected `Organizations` resources you should have all Permissions and Roles already setup.

![Screen Shot 2021-02-25 at 09.57.18](/assets/Screen%20Shot%202021-02-25%20at%2009.57.18.png)

![Screen Shot 2021-02-25 at 09.57.26](/assets/Screen%20Shot%202021-02-25%20at%2009.57.26.png)

If not you can either run [Easy Setup App](#easy-setup-app-optional) selecting only `Organizations` resource to have it set everything up for you or follow the steps detailed in the [prerequisites instructions](https://github.com/vtex-apps/organizations#prerequisites) of `vtex.organizations` app.

#### Update CL Entity

Follow the steps in [Changes to existing CL table
](https://github.com/vtex-apps/organizations#changes-to-existing-cl-table) documentation to get everything working as expected.

Wait a few minutes for the changes to be indexed.

### Setup Reviews and Ratings

Go to **PRODUCTS** &rarr; **Catalog** &rarr; **Reviews** (`https://{{account}}.myvtex.com/admin/reviews-ratings/pending`);

Click "Reviews Settings &rarr;" in the top right conrner.

![Screen Shot 2021-02-25 at 10.12.49](/assets/Screen%20Shot%202021-02-25%20at%2010.12.49.png)

Check "Display stars in product-rating-summary if there are no reviews"

Uncheck "Display total reviews number on product-rating-summary block"

Click "Save"

![Screen Shot 2021-02-18 at 10.15.38](/assets/Screen%20Shot%202021-02-18%20at%2010.15.38.png)

You should see a toast message saing: "Your data was submitted successfully."

![Screen Shot 2021-02-18 at 10.21.00](/assets/Screen%20Shot%202021-02-18%20at%2010.21.00.png)

## Preview

Click on the "VISIT STORE" on the top bar to preview your store.

![Screen Shot 2021-02-25 at 10.18.28](/assets/Screen%20Shot%202021-02-25%20at%2010.18.28.png)

You should see a fully working B2B Store Theme.

![Screen Shot 2021-02-25 at 10.21.04](/assets/Screen%20Shot%202021-02-25%20at%2010.21.04.png)

:warning: &nbsp;**Heads up!** If you're setting up the theme on a working environment (with previously setup resources) you have to map categories links in menus and across the theme and also map shelves queries to a working criteria in case you have multiple trade policies.

You now should have a fully working B2B Environment and B2B Store Theme setup and ready to be used.

That's it!
