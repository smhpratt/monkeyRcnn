# monkeyRcnn
To install run the following commands:
cd $FRCN/lib
make
cd $FRCN/caffe-fast-rcnn
make all -j4
make pycaffe -j4

These commands can also be found on this walk through of installation: https://huangying-zhan.github.io/2016/09/22/detection-faster-rcnn.html

To run, use the below command:
./tools/test_net.py --gpu 0 --def models/basketball/test.prototxt --net output/basketball/train/zf_faster_rcnn_basketball_iter_20000.caffemodel --imdb basketball_val --cfg experiments/cfgs/config.yml
