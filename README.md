- CÔNG NGHỆ SỬ DỤNG: PIL (Pillow), NumPy, Matplotlib.pyplot, OpenCV (cv2), Scipy.ndimage, Scikit-image
- THUẬT TOÁN SỬ DỤNG: 
Otsu Thresholding: skimage.filters.threshold_otsu
Morphological Operations: Dilation, Erosion, Opening, Closing
Adaptive Thresholding: skimage.filters.threshold_local
- GIẢI THÍCH CODE
+ Otsu Thresholding:
 thres = threshold_otsu(a) # Tìm ngưỡng tự động.
 b = a > thres # Tạo ảnh nhị phân (white nếu pixel > thres).
+ Dilation
  b = nd.binary_dilation(data, iterations=50) #Mở rộng đối tượng sáng lên 50 lần, làm cho vùng trắng to hơn và lấp các lỗ nhỏ.
+ Opening
  b = nd.binary_opening(data, structure=s, iterations=25) #Loại bỏ nhiễu nhỏ, giữ lại đối tượng chính (thu nhỏ rồi mở rộng trở lại)
+ Erosion
  b = nd.binary_erosion(data, structure=s, iterations=50) #Làm mòn các vùng sáng nhỏ hoặc chi tiết mảnh → dùng để tách các vùng dính nhau.
+ Closing
  b = nd.binary_closing(data, structure=s, iterations=50) #Lấp các lỗ trắng nhỏ trong vùng đối tượng sáng, làm mượt viền.
BAITAP

bai1

![image](https://github.com/user-attachments/assets/9d2f842b-cd47-402b-9d11-6bc454dd1a94)

bai2

![image](https://github.com/user-attachments/assets/196e4414-ce12-4cc6-bc9f-47de3702b439)

bai3

![image](https://github.com/user-attachments/assets/db18cae3-e0e2-4f85-afa3-7c0a0942e502)

bai4

![image](https://github.com/user-attachments/assets/fd853020-b107-45eb-ac8c-d999acffddaf)

![image](https://github.com/user-attachments/assets/653ad8ec-7e28-4e7b-b45d-4b67b63c5d33)

![image](https://github.com/user-attachments/assets/ab1efbee-230a-478d-b26b-cde87dc6e315)








