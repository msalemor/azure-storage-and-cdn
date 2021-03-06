# Azure Account Storage with Azure CDN

## Azure CDN

### Overview

Azure Content Delivery Network (CDN) offers developers a global solution for rapidly delivering high-bandwidth content to users by caching their content at strategically placed physical nodes across the world. Azure CDN can also accelerate dynamic content, which cannot be cached, by leveraging various network optimizations using CDN POPs. For example, route optimization to bypass Border Gateway Protocol (BGP).

The benefits of using Azure CDN to deliver web site assets include:

Better performance and improved user experience for end users, especially when using applications in which multiple round-trips are required to load content.
Large scaling to better handle instantaneous high loads, such as the start of a product launch event.
Distribution of user requests and serving of content directly from edge servers so that less traffic is sent to the origin server.

- https://docs.microsoft.com/en-us/azure/cdn/cdn-overview

## CDN Benefits

- Distributed network delivering content close to where the users request it.
- Highly scalable and performant networking

## CDN Benefits working with Storage Accounts

- Azure CDN works closesly with Azure blob storage to serve content effective and save on blob transfer costs
- Has features such as re-write rules
- Azure CDN can work with SAS tokens

## Compare Product Features

- https://docs.microsoft.com/en-us/azure/cdn/cdn-features

## Best practices and recommendations

- https://docs.microsoft.com/en-us/azure/architecture/best-practices/cdn

## Azure Account Storage

- Associate SAS tokens with Stored Access policy

## Account Storage - Static Pages

- Static pages get a primary and secondary endpoint.
- Content is private (access with SSAS token) but it is exposed through these endpoints.
- These endpoints can be cached.
- To achive the same functionality from a regular storage, you need a more advance CDN offering that has rewrite rules.

### Static Pages CDN Benefits

- Easy configuration
- No extra cost
- Optimized for static content

### Static Pages CDN Drawback

- Public endpoint is alway anonyumous
- No additional customization allowed (i.e. protection with SAS tokens)
