# Task 1 – Nginx Server Setup

## Objective

Set up an Nginx web server on Linux and configure it to serve the custom HTML page provided by the Linux Community OpenHack organizers.

## Environment

- **Operating System:** Zorin OS
- **Web Server:** Nginx
- **Nginx Version:** 1.24.0
- **Web Root:** `/var/www/html`
- **Hosted Page:** `index.html`

## Organizer HTML Page

The HTML page was downloaded from the URL provided by the organizers:

`http://10.10.110.79:3923/test/index.html`

The original organizer-provided HTML file is included in this folder as:

`organizer.html`

The Name and Roll No fields were intentionally left unchanged because the organizer instructions specify that they should be added during Task 3.

## Implementation Steps

### 1. Update the package information

```bash
sudo apt update
```

### 2. Install Nginx

```bash
sudo apt install nginx
```

### 3. Verify the Nginx installation

```bash
nginx -v
```

Expected result:

```text
nginx version: nginx/1.24.0 (Ubuntu)
```

### 4. Check the Nginx service

```bash
sudo systemctl status nginx
```

The Nginx service was verified to be running successfully.

### 5. Test the organizer's HTML page

```bash
curl --connect-timeout 5 -I http://10.10.110.79:3923/test/index.html
```

The organizer server returned:

```text
HTTP/1.1 200 OK
```

### 6. Download the organizer HTML page

```bash
curl -o organizer.html http://10.10.110.79:3923/test/index.html
```

### 7. Copy the HTML page to the Nginx web root

```bash
sudo cp organizer.html /var/www/html/index.html
```

### 8. Verify the hosted page

```bash
curl http://localhost
```

The organizer-provided HTML page was successfully returned by the local Nginx server.

## Result

**Task 1 completed successfully.**

Nginx was installed and configured to serve the custom HTML page provided by the Linux Community OpenHack organizers through the local web server.

The page can be accessed locally at:

`http://localhost`

## Evidence

The `proof` directory contains screenshots demonstrating the Task 1 implementation:

| Evidence | Description |
|---|---|
| `Task-1 Ngnix-Setup.png` | Nginx setup/installation evidence |
| `Task-1 HTML page.png` | Organizer HTML page evidence |
| `Task-1 Output.png` | Final hosted page/output evidence |

## Files

```text
Task-1/
├── README.md
├── organizer.html
└── proof/
    ├── Task-1 Ngnix-Setup.png
    ├── Task-1 HTML page.png
    └── Task-1 Output.png
```

## Status

✅ Nginx installed  
✅ Nginx service running  
✅ Organizer HTML page downloaded  
✅ HTML page configured in Nginx web root  
✅ Local page verified successfully  
