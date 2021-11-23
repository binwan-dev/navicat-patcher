### Install  
1. Download Navicat15 ```https://www.navicat.com.cn/download/navicat-premium```
2. Install capstone  
   ```
   sudo apt-get install libcapstone-dev
   ```  
3. Install keystone  
   ```
   sudo apt install cmake -y
   git clone https://github.com/keystone-engine/keystone.git
   cd keystone
   mkdir build
   cd build
   ../make-share.sh
   sudo make install
   sudo ldconfig
   ```  
4. Install rapidjson  
   ```
   sudo apt install rapidjson-dev 
   ```  
5. Extract navicat15  
   ```
   mkdir navicat15
   mount -o loop navicat15-premium-cs.AppImage navicat15
   cp -r navicat15 navicat15-patched
   rm -rf navicat15
   ```  
6. Run patcher  
   ```
   ./navicat-patcher navicat15-patched
   ```  
7. Package navicat15 patch   
   ```
   ./appimagetool-x86_64.AppImage navicat15-patched navicat15-premium-cs-pathed.AppImage
   ```  
8. Run navicat15-patched
   ```
   chmod +x navicat15-premium-cs-pathed.AppImage
   ./navicat15-premium-cs-pathed.AppImage
   ```  
   Disable network and click register  
9. Register  
   ```
   navicat-keygen --text ./RegPrivateKey.pem
   ```  
   Disable network and input serial number(egg: NAVD-3CN4-PB6X-VMTP) to navicat15 code.  
   Use manual register.  
   Copy register code to navicat-keygen.  
   Paste code to navicat15-patcher
   

