# onnx_map_torch
Introducing a novel approach for ONNX to Torch conversion for known model structures.

## Introduction
The core idea behind this project is to reverse the exporting process of a Torch model. This is achieved by:

- Constructing a specialized Torch model.
- Converting this Torch model to ONNX.
- Mapping the weights between the ONNX and Torch models.

This approach ensures that the weights of the original model are preserved accurately during the conversion process.

## Features
- This is just a conceptual idea, not a complete one-click tool for direct use.
- This idea is aimed at "partially open-source models" where training code is not available, but pre-trained models are provided.
- To validate this idea, we provide an [example](./conversion.ipynb) of converting `ORTModelForVision2Seq` to `VisionEncoderDecoderModel`, demonstrated using the [pix2text-mfr](https://huggingface.co/breezedeus/pix2text-mfr/) model.


## License
This project is licensed under the MIT License.

The [pix2text-mfr](https://huggingface.co/breezedeus/pix2text-mfr/) pre-trained model used in this project is licensed under the MIT License. Please refer to the original source for the detailed license terms.