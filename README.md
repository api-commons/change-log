# API Change Log

An API Change Log is a simple, machine-readable record of the changes that have shipped for an API over time—each entry capturing a date, a name, a description, a link, and tags. It gives API producers a common way to communicate what has changed to their consumers, and gives consumers a predictable, interoperable place to tune into the evolution of the APIs they depend on. Change is an inevitable part of API operations, and a change log is one of the most important building blocks for managing that change with transparency across the entire API lifecycle.

## API Commons

The API Change Log is an [API Commons](http://apicommons.org) building block—an open, machine-readable schema that can be produced from any system used to manage APIs, and then made interoperable as part of the API contract. It is indexed as a `Common` type within its [APIs.json](apis.yml) index, letting it be discovered, referenced, and reused across the APIs.json ecosystem and surfaced through [apis.io](https://apis.io).

## What's in this repo

- [change-log-schema.yml](change-log-schema.yml) — The JSON Schema that defines a change log entry.
- [change-log-example.yml](change-log-example.yml) — A worked example with a series of change log entries.
- [apis.yml](apis.yml) — The APIs.json index for this building block, referencing the schema and example as `Common` artifacts.

## The Schema

The [change-log-schema.yml](change-log-schema.yml) defines each change log item as an object with the following properties:

- **date** — The target date for the API change log item.
- **name** — The name for the API change log item.
- **image** — The image for the API change log item.
- **link** — The link for the API change log item.
- **tags** — An array of tags for the API change log item.

## Example

The [change-log-example.yml](change-log-example.yml) file provides a list of change log entries you can use as a starting point:

```yaml
- date: 2023-09-01
  name: Feature One
  description: >-
    Lorem ipsum dolor sit amet, consectetur adipiscing elit...
  image: 'https://s3.amazonaws.com/kinlane-productions2/bw-icons/bw-linkedin.png'
  link: 'https://example.com'
  tags:
    - Tag One
    - Tag Two
```

## How It Fits

The change log is one of a growing set of API Commons building blocks that describe the business and technical realities of API operations in a machine-readable way. It cross-links with the [road map](https://github.com/api-commons/road-map), [teams](https://github.com/api-commons/teams), [use cases](https://github.com/api-commons/use-cases), [plans](https://github.com/api-commons/plans), [guidance](https://github.com/api-commons/guidance), [policies](https://github.com/api-commons/policies), and other building blocks—each one a small, reusable schema that can stand alone or be composed together within an APIs.json index.

## Support

This work is in an early stage of development and is rapidly moving as it is applied across a variety of user interfaces and approaches to API operations and governance. If you would like to contribute, have any questions, or would like to inform the work happening, please submit a GitHub issue on this repository or email kin@apievangelist.com.

## Part of API Commons

A machine-readable building block from **[API Commons](https://apicommons.org)** — open specifications and schemas for the APIs you produce and consume. See all building blocks and tools at **[apicommons.org](https://apicommons.org)** and the tools at **[apicommons.org/tools](https://apicommons.org/tools/)**.

**Related building blocks**
- [road-map](https://github.com/api-commons/road-map) — a machine-readable way to publish an API's roadmap
- [use-cases](https://github.com/api-commons/use-cases) — machine-readable API use-case building blocks
- [plans](https://github.com/api-commons/plans) — machine-readable API access plans, tiers, and pricing
- [guidance](https://github.com/api-commons/guidance) — the how-to layer that turns governance rules into help
