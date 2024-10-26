# yolov5-zcu102-yoandri
About The Project: Use Vitis AI to deploy yolov5 on ZCU104
## Reference
- yolov5 code: https://github.com/ultralytics/yolov5
- deploy documents: 
- some helpful post: https://fpga.eetrend.com/blog/2022/100565582.html
## Trainigng yolov5
- download yolov5 from https://github.com/ultralytics/yolov5, choose tag v6.0

## ZCU102 Deployment
- Environment: Vitis AI 3.0 : https://github.com/Xilinx/Vitis-AI/tree/v3.0
- Hardware Environment: Ubuntu 20.04/ NVIDIA GeForce RTX 4090/ Driver: 550.54.14/ CUDA: 12.4
## Install Vitis AI 3.0
1、cd Vitis-AI-3.0/docker
2、./docker_build.sh -t gpu -f pytorch(This will take a lot of time)
3、

note:
1、When running the docker_build.sh file, there may be errors, most likely due to poor network conditions. You can rerun this command: ./docker_build.sh -t gpu -f pytorch
2、If there is an access permission issue, locate the specific file and change the file permissions in the command line, usually using the command: chmod +x {filename}.sh
