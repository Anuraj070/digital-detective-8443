# Mission 7 - How computers communicate

## Task 7.1 - Network concepts

| Concept | Explain it in your own words | Example |
|---|---|---|
| LAN (Local Area Network) | A network that connects devices within a small, limited physical area like a room, home, or lab. | Home Wi-Fi connecting a laptop and a phone. |
| MAN (Metropolitan Area Network) | A network covering a larger geographic area than a LAN, such as an entire town, city, or college campus. | A university campus network connecting different academic buildings. |
| WAN (Wide Area Network) | A large network that spans broad geographical areas, connecting multiple LANs across cities or countries. | The global Internet. |
| DNS (Domain Name System) | The directory system of the internet that converts human-readable domain names into numeric IP addresses. | Resolving `example.com` into `93.184.215.14`. |
| Router | A networking hardware device that directs data packets between different networks to their proper destination. | Home Wi-Fi router forwarding internet traffic between local devices and ISP. |
| Protocol | A standardized set of rules and formats that devices must follow to communicate reliably with each other. | HTTP, HTTPS, TCP, and IP. |
| Packet switching | The method of dividing data into smaller chunks called packets, sending them independently, and reassembling them at the destination. | Streaming a video where small packets travel across various network routes. |
| Client-server | An architecture where client devices request resources or services, and a centralized server responds and provides them. | A web browser (client) requesting a web page from a web server. |

## Task 7.2 - Observe network information

I tested network connectivity and DNS lookup using `example.com` in Terminal:

```bash
ping -c 3 example.com
nslookup example.com
```

- **What a connectivity test (`ping`) helps you check:**  
  It checks whether your computer can reach a remote server across the network, measuring packet loss and the round-trip response time (latency).
- **What information a DNS lookup (`nslookup`) displays:**  
  It displays the domain name queried, the DNS server used for resolution, and the resolved IP address (such as `93.184.215.14`).
- **Role of DNS when entering a website name:**  
  Computers and routers route data packets using numeric IP addresses, not human words. DNS translates the website address typed in the browser into the correct destination IP address before a connection begins.

## Task 7.3 - What happens when you open a website?

1. **User Request:** The user types a website address (URL) into the browser and presses Enter.
2. **DNS Resolution:** The browser queries a DNS server to translate the domain name into its corresponding IP address.
3. **Establishing Connection:** The browser connects to the web server's IP address using standard protocols (TCP/IP handshake, and TLS for secure HTTPS).
4. **Sending HTTP Request:** The browser sends an HTTP/HTTPS GET request across the local router and internet service provider to request the webpage files.
5. **Server Processing:** The destination web server receives the request, processes it, and generates the necessary response data.
6. **Packet Routing:** The web server breaks the response data into packets and transmits them back across the internet through routers.
7. **Client Rendering:** The browser reassembles the received packets, interprets the HTML, CSS, and JavaScript, and displays the webpage on the user's screen.

---

## 1. Task / objective

Explain basic computer network types and concepts, test network connectivity and DNS lookup tools, and explain the steps involved in opening a website.

## 2. Work completed

Defined network concepts (LAN, MAN, WAN, DNS, Router, Protocol, Packet switching, Client-server), performed `ping` and `nslookup` on a public domain, and wrote a 7-step guide explaining how websites load.

## 3. Commands / tools used

- `ping -c 3 example.com`: Tested network reachability and latency.
- `nslookup example.com`: Performed a DNS query to find the domain's IP address.

## 4. My understanding

Networks allow devices to share information using standardized protocols. Humans use easy-to-remember domain names, but computers use IP addresses resolved via DNS. When accessing a webpage, client and server exchange data packets guided by routers across the network.

## 5. Difficulties faced

No major difficulties. Made sure not to expose private local IP addresses or private Wi-Fi network names in documented outputs.

## 6. How I resolved them

Used public test website `example.com` for connectivity and DNS queries as recommended by the assignment instructions.

## 7. Evidence / files

- `mission-07-networking/README.md`

## 8. Commit details

Commit message: `Explain networking concepts and website communication`

The completed Mission 7 work was committed and pushed to GitHub on the main branch.