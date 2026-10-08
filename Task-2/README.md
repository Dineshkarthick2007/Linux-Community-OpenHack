# Task 2 – Access Nginx Website from Another Device

## Objective

Access the HTML page hosted by the Nginx server from another device connected to the same network.

## Environment

- **Server:** Zorin OS Linux PC
- **Web Server:** Nginx
- **Server IP Address:** `10.10.159.197`
- **Protocol:** HTTP
- **Port:** `80`
- **Client Device:** Mobile phone
- **Client Browser:** Web browser

## Procedure

### 1. Find the Linux PC's IP address

The local IP address of the Linux PC was identified using:

```bash
hostname -I
```

The server IP address was:

```text
10.10.159.197
```

### 2. Verify the website using the server IP

The hosted page was tested locally using:

```bash
curl http://10.10.159.197
```

The Nginx server successfully returned the Linux Community OpenHack HTML page.

### 3. Connect the mobile phone to the same network

The mobile phone was connected to the same network as the Linux PC running the Nginx server.

### 4. Access the hosted page from the mobile phone

The following address was entered into the mobile browser:

```text
http://10.10.159.197
```

The Linux Community OpenHack HTML page was successfully displayed on the mobile phone.

## Result

**Task 2 completed successfully.**

The Nginx-hosted HTML page was successfully accessed from another device on the same network using the Linux PC's local IP address.

## Evidence

The `Task-2` folder contains screenshots demonstrating the successful network access:

| Evidence | Description |
|---|---|
| `01-PC-Network-Access.png` | Verification of the hosted page using the PC's network IP |
| `02-Mobile-Access.png` | Mobile phone accessing the Nginx-hosted page |

## Files

```text
Task-2/
├── README.md
├── 01-PC-Network-Access.png
└── 02-Mobile-Access.png
```

## Status

✅ Linux PC IP address identified  
✅ Nginx page verified through network IP  
✅ Mobile connected to the same network  
✅ Hosted page accessed from mobile  
✅ Task 2 successfully demonstrated
