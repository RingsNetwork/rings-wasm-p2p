<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://static.ringsnetwork.io/ringsnetwork_logo.png">
  <img alt="Rings Network" src="https://raw.githubusercontent.com/RingsNetwork/asserts/main/logo/rings_network_red.png">
</picture>


An Example of WASM based P2P (browser oriented)
====

# TL;DR

This example shows how rings network (https://github.com/RingsNetwork/rings-node) works with wasm in browser envirement. In the example, you can create arbitrary nodes, and connect them together by manually SDP handshaking or by relay handshaking.

This example is using Rings-node v0.3.0, you can visit it via:

https://rings.rs/rings-wasm-p2p/

# Explain

This demo is designed for testing handshakes as well as sending and receiving messages. The implementation is straightforward: you import client, init client, and then client.listen(). All features are implemented through client.request. You can review the details in the button.on_click handlers.

The following documents may be helpful for you:
how handshake works:
       https://rings.gitbook.io/rings-network/advanced-topic/handshake
       https://rings.gitbook.io/rings-network/advanced-topic/exchange-sdp
and API list (you can call json apis via `client.request(`method`, [<params>]):
       https://rings.gitbook.io/rings-network/advanced-topic/jsonrpc
