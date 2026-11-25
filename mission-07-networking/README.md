# Mission 7 — How computers communicate

## 1. Task / objective
Explain basic networking concepts, test connectivity and DNS lookup for a public website (`example.com`), and describe step-by-step what happens when a website opens.

## 2. Work completed
Completed Tasks 7.1 through 7.3 in this folder.

### Task 7.1 — Explain network concepts

| Concept | Explain it in your own words | Example |
| :--- | :--- | :--- |
| LAN | A network covering a small area, such as a home, lab or office. | My home Wi-Fi connecting my laptop and phone. |
| MAN | A network covering a city or large campus area. | A university campus network connecting multiple buildings. |
| WAN | A network covering large geographical areas. | The internet connecting networks across countries. |
| DNS | Translates a domain name into an IP address. | Turning `example.com` into `104.20.23.154`. |
| Router | Connects networks and forwards data between them. | A home Wi-Fi router sending traffic between my laptop and the internet. |
| Protocol | A set of rules devices follow to communicate. | HTTP / HTTPS for loading web pages. |
| Packet switching | Data is divided into packets that travel across a network. | Breaking a webpage into small packets and reassembling them on my laptop. |
| Client-server | A client requests a service and a server provides it. | My browser (client) asking GitHub's server for a repository page. |

### Task 7.2 — Observe network information
Ran `ping -c 2 example.com` and `nslookup example.com` from Terminal (local network details redacted).
- **Connectivity test (`ping -c 2 example.com`):** Sent 2 packets and received 2 replies with `0.0% packet loss`.
- **DNS lookup (`nslookup example.com`):** Displayed the public IP addresses for `example.com` (`172.66.147.243` and `104.20.23.154`), with my local DNS server details `[redacted]`.

**Answers:**
- **What a connectivity test helps you check:** It checks whether my computer can reach another computer on the network or internet and how fast packets travel there and back.
- **What information a DNS lookup displays:** It shows the domain name and the IP address(es) mapped to it, along with the DNS server that answered the query.
- **Role of DNS when you enter a website name:** Computers need an IP address to connect, not a name. DNS looks up the domain name you typed and gives your browser the matching IP address.

### Task 7.3 — What happens when you open a website?
1. I type a website address (like `example.com`) into my browser, which acts as the **client**.
2. The client asks a **DNS** server to translate the domain name into the website's IP address.
3. Once the **client** gets the IP address, it sends a request using the HTTPS **protocol** through my local router and across the internet.
4. The request travels as small packets across routers until it reaches the web **server** at that IP address.
5. The **server** receives the request, prepares the webpage files (HTML, CSS, images), and sends them back in packets using the same **protocol**.
6. My browser (**client**) receives the packets, puts them back together, and displays the webpage on my screen.

## 3. Commands / tools used
- `ping -c 2 example.com` — Checked network reachability and round-trip time.
- `nslookup example.com` — Looked up the IP addresses for `example.com`.

## 4. My understanding
Opening a website involves the client (browser), DNS to find the server's IP address, routers to forward packets, and protocols like HTTPS so both sides understand each other.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-07-networking/README.md`

## 8. Commit details
Committed with message `"Explain networking concepts and website communication"` and pushed to `origin/main`.
