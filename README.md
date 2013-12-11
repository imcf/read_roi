# read_roi

- Easy read ImageJ / Fiji ROI binaries in Python
- Created for python 3.3 and more but should work with python 2.7
- To install it just copy / paste read_roi.py in your project
- Specifications and code is largely inspired from: http://rsb.info.nih.gov/ij/developer/source/ij/io/RoiDecoder.java.html

## How to use it

```
import read_roi

zip_file = "example1.zip"
print(read_roi.read_roi_zip(zip_file))
```

```
{'1454-0095-0083': {'y': [7, 19, 27, 40, 56, 74, 96, 120, 134, 152, 183, 182, 171, 151, 140, 117, 92, 65, 51, 50, 35, 21, 11], 'x': [45, 20, 12, 12, 15, 28, 43, 44, 53, 77, 123, 141, 154, 153, 147, 146, 137, 120, 101, 93, 74, 65, 61], 'position': {'channel': 2, 'frame': 73, 'slice': 7}, 'name': '1454-0095-0083', 'n': 23, 'type': 'polygon'}, '0714-0092-0090': {'y': [4, 16, 24, 37, 53, 71, 93, 117, 131, 149, 180, 179, 168, 148, 137, 114, 89, 62, 48, 47, 32, 18, 8], 'x': [52, 27, 19, 19, 22, 35, 50, 51, 60, 84, 130, 148, 161, 160, 154, 153, 144, 127, 108, 100, 81, 72, 68], 'position': {'channel': 2, 'frame': 36, 'slice': 7}, 'name': '0714-0092-0090', 'n': 23, 'type': 'polygon'}, '0014-0089-0092': {'y': [1, 13, 21, 34, 50, 68, 90, 114, 128, 146, 177, 176, 165, 145, 134, 111, 86, 59, 45, 44, 29, 15, 5], 'x': [54, 29, 21, 21, 24, 37, 52, 53, 62, 86, 132, 150, 163, 162, 156, 155, 146, 129, 110, 102, 83, 74, 70], 'position': {'channel': 2, 'frame': 1, 'slice': 7}, 'name': '0014-0089-0092', 'n': 23, 'type': 'polygon'}}
```

```
import read_roi

roi_file = "example2.roi"
print(read_roi.read_roi(roi_file))
```

```
{'example2': {'y': [7, 19, 27, 40, 56, 74, 96, 120, 134, 152, 183, 182, 171, 151, 140, 117, 92, 65, 51, 50, 35, 21, 11], 'x': [45, 20, 12, 12, 15, 28, 43, 44, 53, 77, 123, 141, 154, 153, 147, 146, 137, 120, 101, 93, 74, 65, 61], 'position': {'channel': 2, 'frame': 73, 'slice': 7}, 'name': 'example2', 'n': 23, 'type': 'polygon'}}
```

## License

GPLv3

## Warning

All ImageJ ROI specifications are not integrated but read_roi.py should work for basic ROI shape and informations. All kind of contributions are welcome.

## Author

HadiM : hadrien.mary@gmail.com
