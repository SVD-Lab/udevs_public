# udevs_public
Linux udev files for download.

```bash
declare -a StringArray=("101-at3-realsense-libusb.rules" "102-at3-dai.rules" "103-at3-m5devices.rules" "104-at3-gnss.rules" "105-at3-webcam.rules" )

for val in ${StringArray[@]}; do
   curl https://raw.githubusercontent.com/SVD-Lab/udevs_public/main/${val} --output /etc/udev/rules.d/${val}
done
```
