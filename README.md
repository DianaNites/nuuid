# Nuuid

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
[![nuuid crates.io version and link](https://img.shields.io/crates/v/nuuid.svg)](https://crates.io/crates/nuuid)
![nuuid Crates.io license](https://img.shields.io/crates/l/nuuid)
[![nuuid docs.rs badge](https://docs.rs/nuuid/badge.svg)](https://docs.rs/nuuid)

A New Uuid(nuuid) library for Rust

A `no_std` library to create and use RFC 4122 UUID's in Rust.

This library, through the experimental and ***semver unstable***,
`experimental_uuid` cargo feature, supports UUID v6, v7, and v8.

Details ***MAY*** change as the draft does.

See the draft [New UUID Formats draft RFC][uuid-draft] and
[UUID Prototypes][uuid-proto] for details.

## Specifications

This library follows [RFC 4122], with the following errata taken note of

- [Errata 5560][eid5560]
  - We choose to not touch don't-care bits

## Install

```toml
[dependencies]
nuuid = "0.5.0"
```

`no_std` support:

```toml
[dependencies]
nuuid = "0.5.0"
```

### Dependencies

Depends on [`getrandom`](https://crates.io/crates/getrandom) by default,
which is `no_std` but, depending on target, requires OS system libraries.

This crate is only tested on the latest *stable* Rust.

## Usage

See the documentation for details

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for version history

## See Also

The other [uuid](https://crates.io/crates/uuid) crate.

## Contributing

Feel free to ask questions on the [Github repo](https://github.com/DianaNites/uuid).

[See CONTRIBUTING.md](CONTRIBUTING.md) for details on code contributions.

## License

Licensed under either of

- Apache License, Version 2.0
   ([LICENSE-APACHE](LICENSE-APACHE) or <http://www.apache.org/licenses/LICENSE-2.0)>
- MIT license
   ([LICENSE-MIT](LICENSE-MIT) or <http://opensource.org/licenses/MIT)>

at your option.

[RFC 4122]: https://www.rfc-editor.org/rfc/rfc4122
[eid5560]: https://www.rfc-editor.org/errata/eid5560
[uuid-draft]: https://datatracker.ietf.org/doc/html/draft-ietf-uuidrev-rfc4122bis
[uuid-proto]: https://github.com/uuid6/prototypes
