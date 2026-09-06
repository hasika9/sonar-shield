# Dataset Verification

## GhostVision (crab pot)
- Source: huggingface.co/datasets/PINGEcosystem/sss-crab-pot-detection-ds
- 3,110 annotated SSS images, single class (derelict crab pot)
- Format: Roboflow-style, images + metadata.jsonl
- License: GPL

## SubPipe
- Source: github.com/remaro-network/SubPipe-dataset
- 10,030 SSS images (LF + HF), single class (pipeline)
- Format: COCO bbox annotations
- Attribution required to Oceanscan-MST

## AI4Shipwrecks
- Source: umfieldrobotics.github.io/ai4shipwrecks
- 286 images, 28 shipwreck sites
- Format: segmentation masks — convert to bbox
- Use as cross-domain/unseen test set (Great Lakes, freshwater)

## SeabedObjects-KLSG
- ⚠️ Image-level CLASSIFICATION labels only — no bounding boxes
- Cannot be treated as a native detection dataset
- Check mirror completeness before relying on it
