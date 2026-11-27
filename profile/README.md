# MSFP: Media Server Federation Protocol

MSFP lets media servers share their libraries with each other. People on
one server browse and play the titles another server holds, through their
own server, with their own account. No central service is involved: two
operators pair their servers by hand, or friends' servers pair through a
group they joined with one code each, and each server trusts only the
servers it paired with.

The protocol belongs to no server. Any media server can implement it and
pair with any other that does, whatever it is written in.

## Here

- [msfp-spec](https://github.com/msfp-io/msfp-spec): the specification
  (version 0, a draft until version 1), test vectors and a conformance
  suite.
- [msfp-media](https://github.com/msfp-io/msfp-media): MSFP Media,
  the language for media that MSFP carries between servers and a
  product's API can carry between its players and its server.
- [msfp-go](https://github.com/msfp-io/msfp-go): the engine for Go.
- [msfp-dotnet](https://github.com/msfp-io/msfp-dotnet): the engine for
  .NET (NuGet: Msfp.Engine and Msfp.Protocol).

## Implementations

- [Overfin](https://github.com/Overfin/server) (Go)
- [jellyfin-plugin-msfp](https://github.com/C0PT3R/jellyfin-plugin-msfp),
  a Jellyfin plugin (C#)

Questions and gaps in the specification are welcome as issues on
[msfp-spec](https://github.com/msfp-io/msfp-spec/issues).

## How it's made

MSFP is designed by its maintainer, who makes the architecture, security
and protocol decisions, and written with Claude (Anthropic's AI); Claude's
commits carry a `Co-Authored-By: Claude` trailer. It hasn't had an
independent security review yet.

The specification is under CC BY 4.0, the test vectors under CC0.
Implementing the protocol needs no permission.
