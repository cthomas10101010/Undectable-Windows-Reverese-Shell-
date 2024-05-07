Undetectable reverse shell for windows successfully bypassing windows defender
In this scenario the batch script is being deployed on a fully patched Windows 10 system over email and calling back to the attacker machine (ec2 instance running kali). 
The attacker sets up a net cat listener on port 443 (default port for HTTPS so more likely to look like normal web traffic to firewall). 
![image](https://github.com/cthomas10101010/Undectable-Windows-Reverese-Shell-/assets/169120401/fa818247-619b-4f1f-a821-96d89f9dae75)

 
Target Machine downloads malicious email attachment 
![image](https://github.com/cthomas10101010/Undectable-Windows-Reverese-Shell-/assets/169120401/47144fc1-3cc2-43af-8ca3-aa81c912725a)

 

After the script is run the windows 10 machine calls out to the attacker machine giving the attacker an initial foothold on the Windows machine to begin additional recon and lateral movement.  
Of course, in a real-life scenario an attacker would use social engineering and steganography or a similar technique to make the file appear normal.  
Attackers’ machine after the target executes the script.
  
![image](https://github.com/cthomas10101010/Undectable-Windows-Reverese-Shell-/assets/169120401/f7551ca8-88b4-4ecc-84ea-b0eb3a94efd1)
