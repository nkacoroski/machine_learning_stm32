# Machine Learning with STM32 Products Using STM32Cube.AI Developer Cloud Pilot
## Introduction
### Business Understanding
The purpose of this project is to pilot embedding an Machine Learning (ML) model into a STM32 microcontroller unit (MCU) using the STM32Cube.AI Developer Cloud platform. Field Data Technologies (FDT) is developing environmental monitoring devices by inputting ML models into STM32 MCUs. Currently a ML model is written in Python, optimized with OpenMV, and compiled from Python to C on the device using the Secure Digital (SD) card. FDT would like to explore using the STM32Cube.AI Developer Cloud platform instead. The STM32Cube.AI Developer Cloud is a free online tool provided by STMicroelectronics to embed AI into an MCU. Using this platform may better optimize speed and memory performance of the model, and eliminates any risks with SD compilation by converting into C before embedding on the device.

## Technology Understanding
Hardware:
- [STM32H747I-DISCO discovery board](https://www.st.com/en/evaluation-tools/stm32h747i-disco.html)
- discovery kit manual - https://www.st.com/resource/en/user_manual/um2411-discovery-kit-with-stm32h747xi-mcu-stmicroelectronics.pdf
- B-CAMS-OMV camera bundle
- USB 2.0 A-Male to Micro B cable (two for convenience)
- 30 pin FCC ribbon ~ 5 inches? (camera bundle comes with ~ 2inche ribbon, which is too short for mounting camera bundle on discovery kit)
- mini tripod with 3.5+ inch phone holder?
Software:
-  STM32CubeIDE
-  X-CUBE-AI v7.3.0

## Methods
TODO
1. Get all FP-AI-VISION1 models working on discovery kit.
2. Get transfer learning model working on discovery kit.
3. Get model optimized with STM32Cube.AI Developer Cloud (is this just a replacement for X-CUBE-AI?) and working on discovery kit.
ACTIVE
1. Load FP-AI-VISION1 model on discovery kit - start with person detection?
PENDING
1. Get tripod
2. Get longer FCC ribbon 
COMPLETED
1. Connect camera bundle to discovery kit.
2. Connect discovery kit to computer.
3. Download STM32CubeIDE
4. Download X-CUBE-AI v7.3.0
5. Test camera set-up with PC


Tutorials
- Followed - https://github.com/STMicroelectronics/stm32ai-modelzoo/blob/main/image_classification/getting_started/README.md for guidance.
- Following tutorial - https://wiki.st.com/stm32mcu/wiki/AI:How_to_use_transfer_learning_to_perform_image_classification_on_STM32?utm_source=wiki.st.com with video - https://www.youtube.com/watch?v=NDshmSH7WnA
- another helpful video - https://www.youtube.com/watch?v=8AX9uC2Oi1g

Set Up Hardware: 
1. Connect STM32 board to camera bundle using FCC cable and ZIF connectors. Pop up the black piece of the ZIF connector on STM32 board. Insert one end of the FCC cable blue tape side up into the ZIF connector as far as it will go. Lock down the black piece of the ZIF connector. Repeat for camera bundle.
2. Connect USB 2.0 A-Male end of cable to USB port on computer and Micro B end of cable to the STLINK-V3E USB connector on the STM32 board.

Set Up Software:
1. Download and install STM32CubeIDE
2. Download and install X-CUBE-AI v7.3.0

## Results

## Discussion

## References
- [STMicroelectronics. (2022, March 7). Introduction to STM32: Back to the Basics [Video]. YouTube.](https://www.youtube.com/watch?v=8DmJ7pnFE5M)
- [STMicroelectronics. (2021, June 16). AI on STM32 : Computer Vision made simple with FP-AI-VISION1 and STM32Cube.AI [Video]. YouTube.](https://www.youtube.com/watch?v=NDshmSH7WnA)
- [STMicroelectronics. (2021, June 29). Introduction to STM32: Get Developing [Video]. YouTube.](https://www.youtube.com/watch?v=0OjPY-3qMNU)
- [Easily optimize and benchmark AI neural network models for STM32 - STMicroelectronics. (n.d.). STMicroelectronics.](https://www.st.com/content/st_com/en/campaigns/stm32cubeai-developer-cloud.html?ecmp=tt30638_gl_ps_jan2023&aw_kw=ai%20stm32&aw_m=e&aw_c=19657952321&aw_tg=kwd-1507034916705&aw_gclid=Cj0KCQjwiZqhBhCJARIsACHHEH80jO7sMyOIo1TPzCi83H1fe60IRyuJX2C5Sc-dZ_GTFxaeaP5QHtYaApJ2EALw_wcB&gclid=Cj0KCQjwiZqhBhCJARIsACHHEH80jO7sMyOIo1TPzCi83H1fe60IRyuJX2C5Sc-dZ_GTFxaeaP5QHtYaApJ2EALw_wcB)
- https://www.st.com/resource/en/user_manual/um2411-discovery-kit-with-stm32h747xi-mcu-stmicroelectronics.pdf
