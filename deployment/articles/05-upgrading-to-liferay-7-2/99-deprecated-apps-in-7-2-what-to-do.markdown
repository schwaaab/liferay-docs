---
header-id: deprecated-apps-in-7-2-what-to-do
---

# Deprecated Apps in 7.2: What to Do

[TOC levels=1-4]

During the development of any software product, it's sometimes necessary to stop
development on or remove outdated or unpopular features. @product-ver@ is no
different. In @product-ver@, Liferay has deprecated several apps and features. Some apps and features are in maintenance mode. 

It's important
to note what, exactly, *maintenance mode* and *deprecated* mean here. 

While an app or feature is in maintenance mode, Liferay continues to provide bug fixes and support in accordance to with the subscribers' subscription level and the end of service life policies of the compatible Liferay DXP version. 

There are three types of deprecated apps: 

1.  Deprecated apps that remain in @product@, but will be removed in a future
    release. (Availability: *Bundled*)

2.  Deprecated apps that have been removed from @product@, yet are still 
    available for download via [Liferay
    Marketplace](https://web.liferay.com/marketplace) (Availability:
    *Marketplace*) 

3.  Deprecated apps that have been removed from @product@ and aren't available 
    for download. (Availability: *Removed*) 

| **Note:** All apps deprecated by Liferay are no longer in active development.
| You should therefore plan to stop using these apps. Such apps, however, may
| still be available for download.

| **Note:** For information on apps deprecated in @product@ 7.1, please see 
| [Deprecated Apps in 7.1: What to Do](/docs/7-1/deploy/-/knowledge_base/d/deprecated-apps-in-7-1-what-to-do)

## Apps and Features in Maintenance Mode 

Here are the items in maintenance mode:

-   Liferay Connected Services
-   Liferay Sync
-   Liferay Mobile Experience (Liferay Screens, Liferay Mobile SDK, Liferay 
    Push)
-   Staging 

Here are the apps deprecated in @product-ver@. 

## Foundation

| App |  Availability |  Notes |
| --- | ------------- | ------ |
| AlloyUI | Bundled | Replaced by [MetalJS](https://metaljs.com/) (temporary) exposed as [ClayUI tag](/docs/7-2/reference/-/knowledge_base/r/front-end-taglibs) equivalents. |  
| CMIS Store | Removed | Migrate to another [Document Repository Store option](/docs/7-2/deploy/-/knowledge_base/d/document-repository-configuration). Before [upgrading to @product-ver@](/docs/7-2/deploy/-/knowledge_base/d/upgrading-to-product-ver), migrate your document store data using [Data Migration in Server Administration](/docs/7-2/user/-/knowledge_base/u/server-administration). |
| JCRStore | Removed | Migrate to another [Document Repository Store option](/docs/7-2/deploy/-/knowledge_base/d/document-repository-configuration). Before [upgrading to @product-ver@](/docs/7-2/deploy/-/knowledge_base/d/upgrading-to-product-ver), migrate your document store data using [Data Migration in Server Administration](/docs/7-2/user/-/knowledge_base/u/server-administration). |
| Legacy Search Portlet | Bundled | Will be removed in a future release. Replaced by the [Search widgets](/docs/7-2/user/-/knowledge_base/u/search). |

## Personalization

| App |  Availability |  Notes |
| --- | ------------- | ------ |
| Audience Targeting | Removed | Replaced by [Personalization](/docs/7-2/user/-/knowledge_base/u/segmentation-and-personalization). | 

## Web Experience

| App |  Availability |  Notes |
| --- | ------------- | ------ |
| RSS Publisher | Bundled | See [the article](/docs/7-1/user/-/knowledge_base/u/the-rss-publisher-widget) on enabling and using this widget. |
| User Group Pages (Copy Mode) | Bundled | See the [Legacy User Group Sites Beahavior](/docs/7-1/user/-/knowledge_base/u/user-group-sites#legacy-user-group-sites-behavior) instructions on how to enable it. |
| Resources Importer | Bundled | Deprecated as of 7.1 with no direct replacement |

## Forms

| App | Availability | Notes |
| --- | ------------------ | ----------- |
| Web Form | Nexus &rarr; Will be removed. | Final version released for 7.0. |

## Security

| App |  Availability |  Notes |
| --- | ------------------ | ----------- |
| Central Authentication Service | Bundled | Migrate to [SAML based authentication](/docs/7-2/deploy/-/knowledge_base/d/configuring-saml). |
| Google Login | Marketplace release planned | Replaced by [OpenID Connect](/docs/7-2/deploy/-/knowledge_base/d/authenticating-with-openid-connect). |
| NTLM | Marketplace release planned | Replaced by [Kerberos](/docs/7-2/deploy/-/knowledge_base/d/authenticating-with-kerberos). |
| OAuth 1.0a | Marketplace release planned | Replaced by OAuth 2.0, which is included in the bundle. |
| OpenAM / OpenSSO | Bundled | Migrate to [SAML based authentication](/docs/7-2/deploy/-/knowledge_base/d/configuring-saml). |
| OpenID | Marketplace release planned | Replaced by [OpenID Connect](/docs/7-2/deploy/-/knowledge_base/d/authenticating-with-openid-connect). |

## User and System Management

| App |  Availability | 
| --- | ------------------ |
| Live Users | Enabled through the [`live.users.enabled`](@platform-ref@/7.2-latest/propertiesdoc/portal.properties.html#Live Users) [portal property](/docs/7-2/deploy/-/knowledge_base/d/portal-properties). | 
