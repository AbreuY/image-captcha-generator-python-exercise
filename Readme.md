# Captcha generator with Python & captcha library

Install captcha:
```sh
pip install captcha
```
### Code

```python
from captcha.image import ImageCaptcha
import random
import string

# Set image size
image = ImageCaptcha(width=300, height=100)
# Generate random uppercase text
letters = string.ascii_uppercase
captcha_text = ''.join(random.choice(letters) for i in range(5)) 
# Set random text for captcha
image.write(captcha_text, 'captcha.png')
```
Demo output

![Screenshot](captcha.png?raw=true)

