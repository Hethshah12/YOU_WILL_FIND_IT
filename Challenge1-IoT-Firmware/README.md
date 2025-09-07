# 🚩 Challenge 1: Poisoned IoT Firmware Update

### Storyline
A smart lock company has released a firmware update.  
Your team suspects it contains a **poisoned backdoor** that secretly communicates with an attacker’s server.  
You intercepted the file `firmware.bin`. Reverse-engineer it and uncover the hidden C2 server address.  

---

### Tasks
1. Analyze the `firmware.bin` file.  
2. Locate the malicious injected code segment.  
3. Extract the **C2 server address** hidden with XOR obfuscation.  
4. Submit the flag when you’ve decoded it.  

---

### Hints
- Use `binwalk` and `strings` to start.  
- Check unusual sections in the binary.  
- The XOR key is the first 4 bytes of the firmware.  

---

### Flag Format
flag{iot_firmware_backdoor_detected}
