# Usage
1. Install cvpods first(lastest commit)
2. Download checkpoint of swin-tiny:
[swin-tiny](https://github.com/SwinTransformer/storage/releases/download/v1.0.0/swin_tiny_patch4_window7_224.pth)
3. convert it for cvpods
```
cd segmentation/coco/rcnn/mask_rcnn.swin_tiny.fpn.coco.multiscale.1x
python convert_cvpods_det.py --path /path/to/swin_tiny_patch4_window7_224.pth
```

4. modify the path in config of the swin-tiny pre-train model.
 - like 'swin_tiny_patch4_window7_224_cvpods_det.pth'