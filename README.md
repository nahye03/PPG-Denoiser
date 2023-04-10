# PPG-Denoiser
> PPG 신호 잡음 제거 알고리즘 연구

## Table of Contents
1. Data
2. Model
3. 관련 논문
4. Code

## 1. Data
- Mendeley data와 BIDMC open dataset 사용
- 총 6208개의 PPG 신호 중 input data 2849개, reference data 2849개, test data 510개
- PPG 신호에 Gaussian noise, Poisson noise, salt-and-pepper noise, speckle noise, and uniform noise 합성

## 2. Model
Backbone Framework로 TTSR(Texture Transformer Network for Image Super Resolution)이라는 CNN 기반 이미지 복원 기술 사용
<p align="center"><img src="https://user-images.githubusercontent.com/54797864/230807001-8bb569bb-aeec-4248-b69d-b81f8ea7d0f7.png"></p>

## 3. 관련 논문
- 논문 : [Preeminently Robust Neural PPG Denoiser](https://www.mdpi.com/1424-8220/22/6/2082)

## 4. Code
- TTSR : TTSR 모델을 활용한 PPG 신호 잡음 제거 학습
- noise : PPG 신호에 잡음을 합성한 이미지
