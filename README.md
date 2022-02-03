## TND Data Set

A Data Set generator built with [Mockaroo](https://www.mockaroo.com/) and Hugo

### Mocakroo

We use [Mockaroo](https://www.mockaroo.com/projects/30833) to generate the data files. 

We use Hugo to browse the data files and create markdown files accordingly.

## Setup

1. Clone/Download
2. `$ hugo`
3. Navigate to `/generated_content` to see freshly generated markdown files.
## Collections

Available collections
- posts
- profiles
- events
- products

### Collection parameters
Each collection can take a optional iteration and format parameter

- **iterations**: An integer. This will create X time the number of elements in the data file.
- **format**: A string, only `yaml`|`json` for now. Wether each content file for the collection should be created as JSON or YAML

```yaml
params:
  format: yaml
  collections:
  - name: profiles
  - name: posts
  - name: events
  - name: products
    iterations: 5
```

### Future

1. Create a Hugo website to test drive performances
2. Generate various export files to be imported into CMS services etc...