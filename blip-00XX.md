```
bLIP: XX
Title: WebLN
Status: Active
Author:  Alby <hello@getalby.com>
Created: 2024-01-10
License: CC0
```

## Abstract

The Lightning Web Standard (WebLN) is an application-level protocol for communication between a lightning-powered application (Lapp) and a lightning wallet without the developer needing to know what wallet the application is connected to. WebLN allows for programmatic interactions which reduces friction by removing the need to switch contexts to a wallet interface in order to request lightning functionality, which can be automated and tied to every event or user interaction.

## Copyright

This bLIP is licensed under the CC0 license.

## Motivation

Requiring a user to open a wallet app or scan a QR code for every lightning interaction within an application limits what is possible. A direct connection between an application and lightning wallet is needed. However, it is difficult and time-consuming for application developers to integrate with multiple incompatible APIs of different lightning wallet implementations. A simple application-level protocol to request lightning functionality from a wallet without having to know what wallet it is vastly simplifies development experience so the developer can focus on building their Lapp and not spending time implementing connections to different wallets. The complexity of connecting to different wallets needs to be decoupled from the application itself, while still enabling the user of the application decide what wallet they wish to connect to.

## Rationale (WIP)

> The rationale fleshes out the specification by describing what motivated
the design and why particular design decisions were made. It should describe alternate
designs that were considered and related work. The rationale should provide evidence of
consensus within the community and discuss important objections or concerns raised
during discussion.

TODO: webln.enable, provider, ...

WebLN is a specification that only describes how to interact with a Bitcoin Lightning wallet. There is no need to trust and integrate a third-party library. An application simply requires a WebLN provider, but it's up to the user to choose, and bring this provider to the application (For example, by installing a browser extension, using a browser with WebLN integrated directly, or by interacting with a UI within the application itself to connect to a wallet). The transport mechanism and what wallets are supported is up to the WebLN provider the user chooses.

## Specification



## Misc (WIP)

WebLN is simplify an interface. Providers of WebLN can be implemented in a multiple different ways - as a browser extension, as an external application