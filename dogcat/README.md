# Dogcat TryHackMe Room
## 1. Recon
```
nmap <machine-ip> -sV
```

we discover 2 interesting ports, 22 (ssh) and apache (80) <br>
when we access the IP from browser, we get the following webpage <br>

running a short fuzz on the IP returns the following files and directories: <br>


If we look closely at the address bar, we can see that it is sending a GET request to the server. let us try exploiting using this request <br>
if we add a simple apostrophe to the URL, we are greeted with an error <br>

