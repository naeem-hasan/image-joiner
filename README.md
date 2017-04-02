# pillow-pil-image-joiner
Join multiple images horizontaly or vertically! It returns an PIL/Pillow Image object that can be saved easily.

## Usage:
```python
from PIL import Image
from image_joiner import ImageJoiner

img1 = Image.open("img1.jpg")
img2 = Image.open("img2.jpg")
img3 = Image.open("img3.jpg")

joiner = ImageJoiner(img1, img2, img3)
joiner.set_orientation("vertical")
# default is horizontal
joiner.get_image().show()
```

### Note:
This is for Python 2.7.x only! Feel free to port this to Python 3 if you want. Also I'd love if you contribute!
