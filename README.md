# Andrew Hoang

## Project 5 - Web Crawler

# High Level Approach
The goal of this project was to develop a web crawler capable of navigating the Fakebook website to locate and retrieve five secret flags unique to each student's account. The crawler was designed to perform HTTP GET and POST requests, handle cookies, and manage redirects (HTTP status codes 302, 403, 404, and 503). The crawler is structured around a main Crawler class, which initiates the crawling process. It goes through authentication, queue management, concurrent crawling, HTML parsing, and flag and url management.

# Challenges Faced
Some of the challenges faced was implementing the logic for handling HTTPS connections, including the right use of sockets and SSL context. Also session management, meaning correctly handling session cookies across multiple threads to maintain authentication state with the server. Finally, HTML parsing, efficiently extracting relevant data (flags and URLs) from HTML content without the use of external libraries

# Testing Overview
Testing was done by using print statements in order to read HTTP response code, along with errors and being able to print out the number of links in the queue to keep monitor the progess of the crawler.

