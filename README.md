# Whistler
Pure C# PROOF OF CONCEPT Stealer that sends logs to PHP script that stores as txt
DO NOT USE THIS POC SOFTWARE IN LIVE SYSTEMS!! I am not responsible for any damage or
illegal acivities you start with this !! 
Also i want to make clear i am NOT a blackhat. 


# Features
- USB Spreading (Experimental, 2 Methods)
- Get chromium based browser logins (Chrome, Edge, FireFox, Brave etc)
- Get FileZilla logins (when there was no masterpassword)
- Get some CDKeys from games
- (Not implemented fully) Outlook
- (Not implemented fully) OpenVPN , ProtonVPN, NordVPN logins
- System Informations (IP , Country , PC Specs etc)

- Uploads to PHP Server that stores the logs as txt files.
- Logfiles are encoded with special lambda methods.
- Logfiles are uploaded invisible to Fiddler / Wireshark network analyzers
- Does not leave a trace on the filesystem when ran in mem or USB.


# Installation / Usage
-- Requirements 
- Webspace ( 100MB Minimum)
- IP or Domain
- Visual Studio 2019 or other IDE

Now the full way to use this framework :

1. Upload the contents of the Folder called "SERVER" to your webspace and CHMOD 777 the php file and logs folder
2. Go to the folder called "Stealer" and open the Visual Studio file , then compile WhistlerDecoder and start it.
3. Enter your webspace URL or IP path (http://yourIPorDomain.com/server.php) for example
4. Click ENCODE and copy the now generated encoded text of your IP / Domain 
5. find the Project called Whistler -> open the code of frmMain.cs of the stealer 
and find line 28 "urlToServer" , replace the "xxx" string with the encoded string from the decoder.

6. Make changes to the code / add / remove stuff as you wish , then compile the software
7. Done :) You can now use the stealer and logs are getting saved to the logs folder you uploaded to the webspace.

# TODO list / known bugs 
- TODO - Make the code FUD
- TODO - Add more encryption to the traffic
- TODO - Add dynamic URL / IP Check for server finding after a defined pattern so the stealer will upload logs to any server matching the pattern when one server goes offline
- TODO - Add batch decoding of entire folders of logs to the Decoder
- TODO - Add Webpanel to preview logs (how to decode in PHP)
- BUG - Stealer maybe wont upload logs when the OS is using a systemproxy ?
- BUG - Stealer wont upload on windows 7 - FIXED - Setting SSL configs before uploading for SSL servers


# Credits / Shoutouts
- Echelon Stealer
- Infected-Forums
- Github
- Splamy
