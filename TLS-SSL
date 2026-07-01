# New TLS Old SSL

I’ll give a clear, practical overview of how SSL/TLS secures a connection, including the handshake, certificates, and encryption flow.

SSL (Secure Sockets Layer) is the older name; today, almost everyone really means TLS (Transport Layer Security), which replaced SSL because SSL versions are insecure.

How it works, simply:

1. Client says hello  
Your browser connects to a server and sends supported TLS versions and cipher options.

2. Server proves identity  
The server sends its TLS certificate (issued by a trusted Certificate Authority).  
Your browser checks:
- certificate is valid and not expired
- certificate matches the domain
- certificate chain is trusted

3. Key agreement  
Using asymmetric cryptography (public/private keys), both sides securely agree on shared session keys without sending them in plain text.

4. Secure channel starts  
After handshake success, both switch to fast symmetric encryption (like AES/ChaCha20) for actual data transfer.

5. Data protection in transit  
TLS provides:
- Confidentiality: outsiders can’t read traffic
- Integrity: tampering is detected
- Authentication: confirms you’re talking to the intended server (and optionally client auth too)

Why asymmetric + symmetric together?
- Asymmetric crypto is great for identity and secure key exchange, but slower.
- Symmetric crypto is much faster for bulk data.

Extra detail:
- Modern HTTPS uses TLS (not old SSL).
- TLS also supports session resumption to reconnect faster.
- If cert validation fails, browsers show security warnings.

If you want, I can also explain this with a simple diagram of the TLS handshake (TLS 1.2 vs TLS 1.3).





