# Encrypted Protocol Analysis: Decrypting HTTPS

## Decrypting HTTPS Traffic

| Notes                                                                                                                                                                                                                                                                                                                                                                                                                   | Wireshark Filter                                                                                                                                                                                                   |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <p>"HTTPS Parameters" for grabbing the low-hanging fruits:</p><ul><li><strong>Request:</strong> Listing all requests<br></li><li><strong>TLS:</strong> Global TLS search</li><li>TLS Client Request</li><li>TLS Server response</li><li>Local Simple Service Discovery Protocol (SSDP)</li></ul><p><strong>Note:</strong> SSDP is a network protocol that provides advertisement and discovery of network services.</p> | <ul><li><code>http.request</code></li></ul><ul><li><code>tls</code></li></ul><ul><li><code>tls.handshake == 1</code></li></ul><ul><li><code>tls.handshake == 2</code></li></ul><ul><li><code>ssdp</code></li></ul> |

* Client Hello: `(http.request or tls.handshake.type == 1) and !(ssdp)`&#x20;
* Server Hello:`(http.request or tls.handshake.type == 2) and !(ssdp)`&#x20;

