
<div id="schema-header-title">
  <h2>BlockMeta <span id="schema-header-title-project">schemablocks <a href="https://github.com/ga4gh-schemablocks/template" target="_BLANK">&nearr;</a></span> </h2>
</div>

<table id="schema-header-table">
  <tr>
    <th>{S}[B] Status <a href="https://schemablocks.org/about/sb-status-levels.html">[i]</a></th>
    <td><div id="schema-header-status">proposed</div></td>
  </tr>

  <tr>
    <th>Provenance</th>
    <td>
      <ul>
<li><a href="https://schemablocks.org">Original development for SchemaBlocks project</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Used by</th>
    <td>
      <ul>
<li><a href="https://schemablocks.org">SchemaBlocks</a></li>
      </ul>
    </td>
  </tr>

<!--more-->

  <tr>
    <th>Contributors</th>
    <td>
      <ul>
<li><a href="https://orcid.org/0000-0002-9903-4248">Michael Baudis</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Source (v0.0.1)</th>
    <td>
      <ul>
        <li><a href="current/BlockMeta.json" target="_BLANK">raw source [JSON]</a></li>
        <li><a href="https://github.com/ga4gh-schemablocks/template/blob/master/schemas/BlockMeta.yaml" target="_BLANK">Github</a></li>
      </ul>
    </td>
  </tr>
</table>

<div id="schema-attributes-title">
  <h3>Attributes</h3>
</div>

  
__Type:__ object  
__Description:__ BlockMeta defines the format of the SchemaBlocks metadata, used to describe
e.g. the given block's provenance, scope, external usage.

### Properties

<table id="schema-properties-table">
  <tr>
    <th>Property</th>
    <th>Type</th>
  </tr>
  <tr>
    <th>contributors</th>
    <td>array of https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json [<a href="https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json" target="_BLANK">SRC</a>] [<a href="https://schemablocks.org/schemas/sb-phenopackets/ExternalReference.html" target="_BLANK">HTML</a>]</td>
  </tr>
  <tr>
    <th>provenance</th>
    <td>array of https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json [<a href="https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json" target="_BLANK">SRC</a>] [<a href="https://schemablocks.org/schemas/sb-phenopackets/ExternalReference.html" target="_BLANK">HTML</a>]</td>
  </tr>
  <tr>
    <th>sb_status</th>
    <td>string</td>
  </tr>
  <tr>
    <th>use_cases</th>
    <td>array of https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json [<a href="https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json" target="_BLANK">SRC</a>] [<a href="https://schemablocks.org/schemas/sb-phenopackets/ExternalReference.html" target="_BLANK">HTML</a>]</td>
  </tr>

</table>


#### contributors

* type: array of https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json [<a href="https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json" target="_BLANK">SRC</a>] [<a href="https://schemablocks.org/schemas/sb-phenopackets/ExternalReference.html" target="_BLANK">HTML</a>]

The `contributors` attribute provides a list of one or more contributors
which had been involved in the block's definition or support its format.


##### `contributors` Value Example  

```
{
   "description" : "Michael Baudis",
   "id" : "orcid:0000-0002-9903-4248"
}
```

#### provenance

* type: array of https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json [<a href="https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json" target="_BLANK">SRC</a>] [<a href="https://schemablocks.org/schemas/sb-phenopackets/ExternalReference.html" target="_BLANK">HTML</a>]

The `provenance` attribute provides a list of pointers to e.g. external
schemas, predecessors of the current schema or external documentation
describing the schema's genesis.


##### `provenance` Value Example  

```
{
   "description" : "Original GA4GH schema",
   "id" : "https://github.com/ga4gh/ga4gh-schemas/blob/master/src/main/proto/ga4gh/bio_metadata.proto#L111"
}
```

#### sb_status

* type: string

With `sb_status` the current support level of the schema block inside
the {S}[B] ecosystem has to be demonstrated. A first recommendation of
levels is:

* `playground`
  - early development or import stage, of any quality
  - no recommendation; existence does not mean any current or future
  {S}[B] support
* `proposed`
  - at least some {S}[B] contributors are in favour of such a block
  - the code may undergo considerable maturation
  - not recommended for integration into products w/o close tracking
  - contributions and discussions are encouraged
* `implementation`
  - mature block which is implemented in one or more {S}[B] aligned
  schemas
  - may be extended from a core block or be too specific for general
  ("core") usability
* `core`
  - a schema block with recommended use
  - stable through minor version changes
  - has to be used in at least 2 approved / under review GA4GH products


##### `sb_status` Value Examples  

```
"core"
```
```
"implementation"
```
```
"proposed"
```
```
"playground"
```

#### use_cases

* type: array of https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json [<a href="https://schemablocks.org/schemas/sb-phenopackets/v1.0.0/ExternalReference.json" target="_BLANK">SRC</a>] [<a href="https://schemablocks.org/schemas/sb-phenopackets/ExternalReference.html" target="_BLANK">HTML</a>]

With the `use_cases` attribute one can provide links and descriptions
for the use of a given block in an external implementation.
This is not intended to provide a catalogue of all known implementations
of the schema.


##### `use_cases` Value Examples  

```
{
   "description" : "Phenopackets",
   "id" : "https://github.com/phenopackets/phenopacket-schema/blob/master/docs/age.rst"
}
```
```
{
   "description" : "Progenetix database schema (Beacon+ backend)",
   "id" : "https://github.com/progenetix/schemas/tree/master/main/yaml"
}
```


### `BlockMeta` Value Example  

```
{
   "contributors" : [
      {
         "description" : "Michael Baudis",
         "id" : "orcid:0000-0002-9903-4248"
      },
      {
         "description" : "Ben Hutton",
         "id" : "https://github.com/Relequestual"
      }
   ],
   "provenance" : [
      {
         "description" : "Developer branch of original GA4GH schema",
         "id" : "https://github.com/ga4gh-metadata/metadata-schemas/blob/master/schemas/shared.proto#L60"
      }
   ],
   "sb_status" : "playground",
   "used_by" : [
      {
         "description" : "Phenopackets",
         "id" : "https://github.com/phenopackets/phenopacket-schema/blob/master/docs/geolocation.rst"
      },
      {
         "description" : "Progenetix database schema (Beacon+ backend)",
         "id" : "https://github.com/progenetix/schemas/tree/master/main/yaml"
      }
   ]
}
```

