# Azure Account Storage with Azure CDN

## Azure CDN

### Overview

- https://docs.microsoft.com/en-us/azure/cdn/cdn-overview

## Compare Product Features

- https://docs.microsoft.com/en-us/azure/cdn/cdn-features

## Best practices and recommendations

- https://docs.microsoft.com/en-us/azure/architecture/best-practices/cdn

## Azure Account Storage

## Account Storage - Static Pages

- Static pages get a primary and secondary endpoint.
- Content is private (access with SSAS token) but it is exposed through these endpoints.
- These endpoints can be cached.
- To achive the same functionality from a regular storage, you need a more advance CDN offering that has rewrite rules.

