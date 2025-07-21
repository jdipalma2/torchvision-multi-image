# torchvision-multi-image

This repository contains a customized version of the [TorchVision](https://github.com/pytorch/vision) library designed for transforming paired images with the same set of transformations.
This is useful for when running models that need paired inputs with identical transforms but differ in some other aspect.

# Compilation
Run the following command from the directory where `pyproject.toml` is located
```commandline
python -m build
```

After successful compilation, there should be a `dist` directory containing files
```text
dist/
|----tvmi-1.0.0-py3-none-any.whl
|----tvmi-1.0.0.tar.gz
```
Don't worry if the file names differ slightly. As long as files with both extensions exist, your compilation is fine.

Install the Python wheel file as follows:
```commandline
pip install tvmi-1.0.0-py3-none-any.whl
```

Now in a Python interpreter, test importing the `tvmi` package to verify the installation worked.
```python
import tvmi
```
If the above code runs, then you have successfully installed `tvmi`.