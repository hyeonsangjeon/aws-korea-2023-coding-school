# aws-korea-coding-school-2023



Text-to-image generation using Huggingface stable diffusion ControlNet conditioning and AWS Translate's prompt translation function

![screenshot1](https://github.com/hyeonsangjeon/AIsketcher/blob/main/pic/yahunjeon.png?raw=true)
![screenshot2](https://github.com/hyeonsangjeon/AIsketcher/blob/main/pic/seowonjeon.png?raw=true)

## Project Description
이 함수는 이미지와 프롬프트 텍스트 두 가지 입력을 사용하여 작동합니다. 멀티 모달 모델의 기능을 활용하고 있습니다.

이 프로젝트에서는 Stable Diffusion을 사용했으며, 프롬프트는 영어로 작성되었습니다. 그러나 다른 언어를 주로 사용하는 사용자들에게는 입력 문장의 세부 사항을 표현하는 것이 어려울 수 있습니다. 따라서 사용자의 언어를 입력 프롬프트로 사용하고, 해당 텍스트는 Amazon Translate를 사용하여 영어로 기계 번역된 후 모델에 입력됩니다.

사전 준비 사항: StableDiffusionControlNet 파이프라인에 ControlNetModel과 StableDiffusionModel을 로드하고, PNDMScheduler를 준비합니다.


# 워크플로우
1. 사전 준비사항을 실행합니다. 
2. 7개의 주어진 그림을 보고 상상했던 프롬프트를 입력합니다. 
3. 직접 찍은 사진을 SageMaker에 업로드한 다음 사용해봅니다. 

# 설계도
![screenshot3](https://github.com/hyeonsangjeon/aws-korea-2023-coding-school/blob/main/readme.png)


# Package Used
AIsketcher를 구현 사용했습니다.[1]
Generative AI 및 Torch와 OpenCV에 대한 코드는 최대한 은닉했습니다. 사용자 눈높이에서는 한국어 프롬프트만 사용하면 되도록 구현합니다. 


### References 
- `[1]`. AIsketcher, [https://github.com/hyeonsangjeon/AIsketcher](https://github.com/hyeonsangjeon/AIsketcher)

