# What Happens When You Type a Website Into a Browser

## Overview
When you type a website URL into a browser, a series of steps occur to locate the server, request the page, and display it. 
This process involves DNS resolution, network communication, and rendering, all happening in milliseconds.

## Steps
1. **Browser parses the URL** – Identifies protocol (HTTP/HTTPS), domain name, and path.  
2. **DNS Lookup** – Browser asks a DNS server to resolve the domain into an IP address.  
3. **Establish Connection** – Browser initiates a TCP connection (and TLS handshake if HTTPS) with the server.  
4. **Send HTTP Request** – Browser sends a GET request asking for the webpage data.  
5. **Server Processes Request** – Web server retrieves the requested content and prepares a response.  
6. **Server Sends Response** – Data is sent back over the network to the browser.  
7. **Browser Renders Page** – Browser interprets HTML, CSS, and JavaScript to display the page visually.  
8. **Load Additional Resources** – Browser fetches images, scripts, and styles referenced by the page.  
9. **Interactive Page Ready** – JavaScript runs and the page becomes fully interactive for the user.  

## Operational/Security Considerations
- **DNS spoofing** could redirect users to malicious sites.  
- **HTTPS ensures encrypted communication** to protect data in transit.  
- **Caching** improves speed but can serve outdated content.  
- **Browser extensions** can interfere with page rendering.  

## How This Breaks or Gets Attacked
- **DNS failure or misconfiguration** can make the website unreachable.  
- **Server downtime** prevents responses from being sent.  
- **Man-in-the-middle attacks** could intercept unencrypted HTTP traffic.  

