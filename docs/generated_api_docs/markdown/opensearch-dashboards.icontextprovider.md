<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [opensearch-dashboards](./opensearch-dashboards.md) &gt; [IContextProvider](./opensearch-dashboards.icontextprovider.md)

## IContextProvider type

A function that returns a context value for a specific key of given context type.

<b>Signature:</b>

```typescript
export declare type IContextProvider<THandler extends HandlerFunction<any>, TContextName extends keyof HandlerContextType<THandler>> = (context: PartialExceptFor<HandlerContextType<THandler>, 'core'>, ...rest: HandlerParameters<THandler>) => Promise<HandlerContextType<THandler>[TContextName]> | HandlerContextType<THandler>[TContextName];
```
<b>References:</b> [HandlerFunction](./opensearch-dashboards.handlerfunction.md)<!-- -->, [HandlerContextType](./opensearch-dashboards.handlercontexttype.md)<!-- -->, [HandlerParameters](./opensearch-dashboards.handlerparameters.md)

## Remarks

This function will be called each time a new context is built for a handler invocation.
