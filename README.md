# accounting-
import pytesseract
from PIL import Image

# 1. Upload ki gayi bill ki photo load karein
bill_image = Image.open("bill_photo.jpg")

# 2. Image se text extract karein (OCR)
extracted_text = pytesseract.image_to_string(bill_image)

# 3. Extracted data print karein (jise baad mein PDF bill mein dala jayega)
print("Bill Details:\n", extracted_text)
