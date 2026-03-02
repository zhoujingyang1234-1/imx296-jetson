# imx296-jetson

## Precompiler Driver Use Method
## Driver Install Method
- Flash jetson-orin-nano-devkit-super-SD-image_JP6.2.1
- sudo git clone https://github.com/zhoujingyang1234-1/imx296-jetson.git
- cd imx296-jetson
- sudo tar -xvf linux-5.15-jetson-orin-nano-imx296-package-20260206.tar.xz -C /
- sudo depmod -a
- sudo /opt/nvidia/jetson-io/jetson-io.py
- choose Camera IMX219-A and IMX296-C
- sudo reboot

## Connection
- CAM1 IMX296-C
- CAM0 IMX219




### Test 
- nvgstcapture-1.0 --sensor-id=0   #CAM0
- nvgstcapture-1.0 --sensor-id=1   #CAM1

| Note: If the first time image or video not normal, ctrl+c to stop the command, then re-run the scripts or command.
