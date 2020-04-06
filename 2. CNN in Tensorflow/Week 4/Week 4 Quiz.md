# Week 4 Quiz

1. The diagram for traditional programming had Rules and Data in, but what came out?
    - [ ] Machine Learning
    - [ ] Bugs
    - [ ] Binary
    - [x] Answers

2. Why are there 10 output neurons?
    - [ ] To make it classify 10x faster
    - [ ] Purely arbitrary
    - [x] There are 10 different labels
    - [ ] To make it train 10x faster

3. What is a Convolution?
    - [ ] A technique to make images smaller
    - [ ] A technique to make images bigger
    - [ ] A technique to filter out unwanted images
    - [x] A technique to isolate features in images

4. Applying Convolutions on top of a DNN will have what impact on training?
    - [ ] It will be slower
    - [ ] It will be faster
    - [ ] It will have no impact
    - [x] It depends on many factors. It might make your training faster or slower, and a poorly designed Convolutional layer may even be less efficient than a plain DNN!

5. What method on an ImageGenerator is used to normalize the image?
    - [ ] normalize
    - [ ] flatten
    - [ ] resize()
    - [x] rescale

6. When using Image Augmentation with the ImageDataGenerator, what happens to your raw image data on-disk.
    - [ ] It gets overwritten, so be sure to make a backup
    - [ ] A copy is made and the augmentation is done on the copy
    - [ ] It gets deleted
    - [x] Nothing, all augmentation is done in-memory

7. Can you use Image augmentation with Transfer Learning?
    - [x] Yes. It's pre-trained layers that are frozen. So you can augment your images as you train the bottom layers of the DNN with them
    - [ ] No - because the layers are frozen so they can't be augmented

8. When training for multiple classes what is the Class Mode for Image Augmentation?
    - [ ] class_mode='multiple'
    - [ ] class_mode='non_binary'
    - [x] class_mode='categorical'
    - [ ] class_mode='all'