## **Code Peer Review Templete**
------------------
- 코더 : 김동규
- 리뷰어 : 남희정

## **PRT(PeerReviewTemplate)**
------------------  
평가문항	상세기준

2. pix2pix 모델을 구현하여 성공적으로 학습 과정을 진행하였다.	U-Net generator, discriminator 모델 구현이 완료되어 train_step의 output을 확인하고 개선하였다.
3. 학습 과정 및 테스트에 대한 시각화 결과를 제출하였다.	10 epoch 이상의 학습을 진행한 후 최종 테스트 결과에서 진행한 epoch 수에 걸맞은 정도의 품질을 확인하였다.

- [x] **1. 코드가 정상적으로 동작하고 주어진 문제를 해결했나요?**
- [ ] 한가지 이상의 augmentation을 적용하였습니다.
  <code>def random_crop(input_image, real_image):
    stacked_image = tf.stack([input_image, real_image], axis=0)
    cropped_image = tf.image.random_crop(
      stacked_image, size=[2, IMG_HEIGHT, IMG_WIDTH, 3])</code>
  
  - [ ] 한가지 이상의 augmentation을 적용하였습니다.

    return cropped_image[0], cropped_image[1]
- [x] **2. 주석을 보고 작성자의 코드가 이해되었나요?**

- [x] **3. 코드가 에러를 유발할 가능성이 있나요?**

- [x] **4. 코드 작성자가 코드를 제대로 이해하고 작성했나요?**

- [x] **5. 코드가 간결한가요?**

## **참고링크 및 코드 개선 여부**

    
