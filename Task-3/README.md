# Task 3 – Modify HTML Page and Verify Changes

## Objective

Modify the custom HTML page hosted by the Nginx server and verify that the changes are reflected when the hosted page is accessed from another device on the same network.

## Environment

- **Operating System:** Zorin OS
- **Web Server:** Nginx
- **Server IP Address:** `10.10.159.197`
- **Protocol:** HTTP
- **Port:** `80`
- **Client Device:** Android mobile phone
- **Web Browser:** Mobile web browser
- **Web Root:** `/var/www/html`

## Task Requirement

The organizer-provided HTML page contains placeholders for:

```html
<p>Name: [Your Name]</p>
<p>Roll No: [Your Roll No]</p># Task 3 – Modify HTML Page and Verify Changes

## Objective

Modify the custom HTML page hosted by the Nginx server and verify that the changes are reflected when the hosted page is accessed from another device on the same network.

## Environment

- **Operating System:** Zorin OS
- **Web Server:** Nginx
- **Server IP Address:** `10.10.159.197`
- **Protocol:** HTTP
- **Port:** `80`
- **Client Device:** Android mobile phone
- **Web Browser:** Mobile web browser
- **Web Root:** `/var/www/html`

## Task Requirement

The organizer-provided HTML page contains placeholders for:

```html
<p>Name: [Your Name]</p>
<p>Roll No: [Your Roll No]</p>

The Name and Roll No were added during Task 3 as instructed by the organizers.
Procedure
1. Open the hosted HTML file
sudo nano /var/www/html/index.html

2. Modify the Name and Roll No
The placeholder values were replaced with:
<p>Name: Dinesh Karthick M</p>
<p>Roll No: 7376242CB120</p>

3. Save the modified HTML file
The modified file was saved and closed using the nano editor.
4. Verify the modified page on the Linux server
curl http://localhost

The server successfully returned the updated HTML page containing the participant's Name and Roll No.
5. Verify the changes from another device
The Android mobile phone was connected to the same network as the Linux PC.
The following address was opened in the mobile browser:
http://10.10.159.197

The updated HTML page was successfully displayed on the Android mobile phone.
Result
Task 3 completed successfully.
The custom HTML page hosted by Nginx was modified with the participant's Name and Roll No, and the updated content was successfully verified from another device on the same network.
Evidence
The proof directory contains the screenshot showing the updated hosted page accessed from the Android mobile phone.
Evidence	Description
Task-3-Mobile-Access.png	Updated HTML page displayed on the Android mobile phone


Files
Task-3/
├── README.md
└── proof/
    └── Task-3-Mobile-Access.png

Status
- [x] HTML page modified
- [x] Name added
- [x] Roll No added
- [x] Modified page verified using curl
- [x] Updated page accessed from Android device
- [x] Task 3 successfully demonstrated
