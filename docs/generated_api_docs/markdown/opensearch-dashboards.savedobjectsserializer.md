<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [opensearch-dashboards](./opensearch-dashboards.md) &gt; [SavedObjectsSerializer](./opensearch-dashboards.savedobjectsserializer.md)

## SavedObjectsSerializer class

A serializer that can be used to manually convert [raw](./opensearch-dashboards.savedobjectsrawdoc.md) or [sanitized](./opensearch-dashboards.savedobjectsanitizeddoc.md) documents to the other kind.

<b>Signature:</b>

```typescript
export declare class SavedObjectsSerializer 
```

## Remarks

Serializer instances should only be created and accessed by calling [SavedObjectsServiceStart.createSerializer](./opensearch-dashboards.savedobjectsservicestart.createserializer.md)

The constructor for this class is marked as internal. Third-party code should not call the constructor directly or create subclasses that extend the `SavedObjectsSerializer` class.

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [generateRawId(namespace, type, id)](./opensearch-dashboards.savedobjectsserializer.generaterawid.md) |  | Given a saved object type and id, generates the compound id that is stored in the raw document. |
|  [isRawSavedObject(rawDoc)](./opensearch-dashboards.savedobjectsserializer.israwsavedobject.md) |  | Determines whether or not the raw document can be converted to a saved object. |
|  [rawToSavedObject(doc)](./opensearch-dashboards.savedobjectsserializer.rawtosavedobject.md) |  | Converts a document from the format that is stored in opensearch to the saved object client format. |
|  [savedObjectToRaw(savedObj)](./opensearch-dashboards.savedobjectsserializer.savedobjecttoraw.md) |  | Converts a document from the saved object client format to the format that is stored in opensearch. |
