# MC Championship Event API

<br />
<p align="center">
    <img src="https://mcc.live/assets/img/game-screenshots/Hub_2_Live.png" />
</p>
<br />

## Introduction

MC Championship is a competitive Minecraft event for Java Edition created by [Noxcrew](https://noxcrew.com/). From the start of MCC Season 2, we have provided our audience with a way of tracking statistics in real-time in the form of [MCC Live](https://mcc.live/) and we are opening up this data to the public in the form of our first public REST API.

It is worth emphasising that this is only a small fragment of what the team want to make accessible; a second iteration will come in the future with more data being accessible.

<br />

## The API

[Full documentation](https://api.mcchampionship.com/docs/) is now available via the API directly, including information about the data available and the schema of responses.

This initial version provides information about the **current event cycle** only. Although this certainly is something we want to expand upon in the future, it is all we are able to provide for now. This is because the API is entirely based on the same database which feeds [MCC Live](https://mcc.live/), which _at present_ does not rely on any information from previous event cycles.

Please note that, in the interests of safety, the API is **rate limited to 40 requests per minute per IP**. Therefore, we recommend caching responses on your own database. This also enables you to look back at past event cycles until we add the capability to do this directly in the API in the future.

<br />

## Looking ahead

As mentioned, this is an early iteration of the final API for which we are striving. Although this second iteration, whenever it comes out, will have significant differences to accommodate the ability to look at past event cycles, we are aiming to allow for interoperability between the two. At present we are unable to provide concrete details on this and how it will behave with the release of [MCC Island](https://mccisland.net/) but will continue to update this repository with further information when we are ready to share it.

Furthermore, as a REST API this current version lacks the ability to listen to changes directly via technologies like [Web Sockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API/). We may enable this in the future but are unable to confirm with certainty at this stage.

<br />

## Issues and feedback

Should you encounter any issues while using the API, or have any feedback you wish to share, please create an [issue](https://github.com/Noxcrew/mcc-event-api/issues) and we will get back to you as soon as possible.
