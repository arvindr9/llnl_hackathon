

## Taking a picture with raspberry pi

`fswebcam (image name)`

## Running the model

`ppython3 classify_image.py --model ~/Downloads/mobilenet_v2_1.0_224_quant_edgetpu.tflite --label ~/Downloads/imagenet_labels.txt --image (path to image)`

# Tutorial
https://coral.withgoogle.com/docs/edgetpu/api-intro/

# Running live model with USB camera


Try these:

`edgetpu_classify \
--source /dev/video1:YUY2:800x600:24/1 \
--model ${DEMO_FILES}/mobilenet_v2_1.0_224_quant_edgetpu.tflite \
--labels ${DEMO_FILES}/imagenet_labels.txt`

`edgetpu_classify \
--source /dev/video0:YUY2:800x600:24/1 \
--model ${DEMO_FILES}/mobilenet_v2_1.0_224_quant_edgetpu.tflite \
--labels ${DEMO_FILES}/imagenet_labels.txt`
