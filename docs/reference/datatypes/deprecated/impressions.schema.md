
# Impressions Schema

```
https://ns.adobe.com/xdm/data/metrics/advertising/impressions
```

The metric impressions describes the number of digital assets rendered.

| [Abstract](../../../abstract.md) | [Extensible](../../../extensions.md) | [Status](../../../status.md) | [Identifiable](../../../id.md) | [Custom Properties](../../../extensions.md) | [Additional Properties](../../../extensions.md) | Defined In |
|----------------------------------|--------------------------------------|------------------------------|--------------------------------|---------------------------------------------|-------------------------------------------------|------------|
| Can be instantiated | Yes | Deprecated | No | Forbidden | Permitted | [datatypes/deprecated/impressions.schema.json](datatypes/deprecated/impressions.schema.json) |
## Schema Hierarchy

* Impressions `https://ns.adobe.com/xdm/data/metrics/advertising/impressions`
  * [Metric Definition](../data/metricdefinition.schema.md) `https://ns.adobe.com/xdm/data/metricdefinition`


## Impressions Example
```json
{
  "schema:name": "metric: impressions",
  "@id": "xdm:impressions",
  "xdm:measurement": "count",
  "xdm:unit": ""
}
```

# Impressions Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [@id](#id) | `string` | **Required** | [Metric Definition](../data/metricdefinition.schema.md#id) |
| [schema:name](#schemaname) | `string` | **Required** | [Metric Definition](../data/metricdefinition.schema.md#schemaname) |
| [xdm:measurement](#xdmmeasurement) | `string` | **Required** | [Metric Definition](../data/metricdefinition.schema.md#xdmmeasurement) |
| [xdm:unit](#xdmunit) | `string` | **Required** | [Metric Definition](../data/metricdefinition.schema.md#xdmunit) |
| `*` | any | Additional | this schema *allows* additional properties |

## @id

The unique identifier of this metric.

`@id`
* is **required**
* type: `string`
* defined in [Metric Definition](../data/metricdefinition.schema.md#id)

### @id Type


`string`
* format: `uri-reference` – URI Reference (according to [RFC3986](https://tools.ietf.org/html/rfc3986))






## schema:name

The human-readable name of the metric. The name can be used in user interfaces and does not have to be unique.

`schema:name`
* is **required**
* type: `string`
* defined in [Metric Definition](../data/metricdefinition.schema.md#schemaname)

### schema:name Type


`string`






## xdm:measurement

How to take measures of this metric.

`xdm:measurement`
* is **required**
* type: `string`
* defined in [Metric Definition](../data/metricdefinition.schema.md#xdmmeasurement)

### xdm:measurement Type


`string`





### xdm:measurement Examples

```json
"distance"
```

```json
"time"
```

```json
"price"
```

```json
"count"
```



## xdm:unit

The unit that this metric is measured in. Whenever possible, metrics should follow the [SI base units](https://www.bipm.org/en/measurement-units/) or be [ISO 4217 currency codes](https://www.iso.org/iso-4217-currency-codes.html).For metric that are counts, the `xdm:unit` must be empty string (equivalent to null)

`xdm:unit`
* is **required**
* type: `string`
* defined in [Metric Definition](../data/metricdefinition.schema.md#xdmunit)

### xdm:unit Type


`string`





### xdm:unit Examples

```json
"m"
```

```json
"kg"
```

```json
"s"
```

```json
"USD"
```

