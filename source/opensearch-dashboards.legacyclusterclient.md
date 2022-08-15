<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [opensearch-dashboards](./opensearch-dashboards.md) &gt; [LegacyClusterClient](./opensearch-dashboards.legacyclusterclient.md)

## LegacyClusterClient class

> Warning: This API is now obsolete.
> 
> Use [IClusterClient](./opensearch-dashboards.iclusterclient.md)<!-- -->.
> 

Represents an OpenSearch cluster API client created by the platform. It allows to call API on behalf of the internal OpenSearch Dashboards user and the actual user that is derived from the request headers (via `asScoped(...)`<!-- -->).

<b>Signature:</b>

```typescript
export declare class LegacyClusterClient implements ILegacyClusterClient 
```
<b>Implements:</b> [ILegacyClusterClient](./opensearch-dashboards.ilegacyclusterclient.md)

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(config, log, getAuditorFactory, getAuthHeaders)](./opensearch-dashboards.legacyclusterclient._constructor_.md) |  | Constructs a new instance of the <code>LegacyClusterClient</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [callAsInternalUser](./opensearch-dashboards.legacyclusterclient.callasinternaluser.md) |  | [LegacyAPICaller](./opensearch-dashboards.legacyapicaller.md) | Calls specified endpoint with provided clientParams on behalf of the OpenSearch Dashboards internal user. See [LegacyAPICaller](./opensearch-dashboards.legacyapicaller.md)<!-- -->. |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [asScoped(request)](./opensearch-dashboards.legacyclusterclient.asscoped.md) |  | Creates an instance of [ILegacyScopedClusterClient](./opensearch-dashboards.ilegacyscopedclusterclient.md) based on the configuration the current cluster client that exposes additional <code>callAsCurrentUser</code> method scoped to the provided req. Consumers shouldn't worry about closing scoped client instances, these will be automatically closed as soon as the original cluster client isn't needed anymore and closed. |
|  [close()](./opensearch-dashboards.legacyclusterclient.close.md) |  | Closes the cluster client. After that client cannot be used and one should create a new client instance to be able to interact with OpenSearch API. |
