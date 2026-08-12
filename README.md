# 👁️ OpenCV Crash Course – Object Detection

## 🎯 Tasks to be Performed

1. 🔹 **Single Object Detection**
2. 🔹 **Multiple Object Detection**
3. 🔹 **Webcam / CCTV Detection**

---

# 🧩 10-Step Framework for OpenCV Object Detection

1. 📚 **Import Libraries**
2. 🤖 **Import Model**
3. 🖼️ **Import Image / Video**
4. ⚫ **Convert the Image / Frame into Grayscale**
5. 🔍 **Use Multi-Scale Detector to get the position coordinates**
6. 📦 **Use a Looping Statement to draw rectangular bounding boxes around the detected objects**
7. 🖥️ **Display the Image / Video Frame**
8. ⌨️ **Use `waitKey()` to pause/refresh the program and capture the key used to close it**
9. 🔓 **Release the Video / Image Frame**
10. ❌ **Close all OpenCV Windows**

---

# 1️⃣ Single / Multiple Object Detection

In this section, OpenCV is used to detect faces from an image using a **Haar Cascade Classifier**.

### 🔄 Process

```text
🖼️ Input Image
      ↓
⚫ Convert Image to Grayscale
      ↓
🤖 Haar Cascade Face Detector
      ↓
📍 Detect Face Coordinates
      ↓
📦 Draw Bounding Boxes
      ↓
🖥️ Display Result
```

---

## 🖼️ Image-Based Face Detection

The following steps are performed:

* 📚 Import OpenCV
* 🤖 Load the Haar Cascade model
* 🖼️ Read the input image
* ⚫ Convert the image into grayscale
* 🔍 Detect faces using `detectMultiScale()`
* 📍 Extract the coordinates of detected faces
* 📦 Draw rectangular bounding boxes
* 🖥️ Display the detected image

---

## 🛠️ Important OpenCV Functions

| 🔧 Function               | 🎯 Purpose                                  |
| ------------------------- | ------------------------------------------- |
| `cv2.CascadeClassifier()` | 🤖 Loads the Haar Cascade detection model   |
| `cv2.imread()`            | 🖼️ Reads an image                          |
| `cv2.cvtColor()`          | ⚫ Converts the image to grayscale           |
| `detectMultiScale()`      | 🔍 Detects objects/faces at multiple scales |
| `cv2.rectangle()`         | 📦 Draws a bounding box                     |
| `cv2.imshow()`            | 🖥️ Displays the image                      |
| `cv2.waitKey()`           | ⌨️ Waits for a keyboard input               |

---

# 3️⃣ CCTV / Webcam Detection

In this section, OpenCV captures frames continuously from a webcam and detects faces in **real time**.

### 🔄 Process

```text
📹 Webcam / CCTV
      ↓
🎞️ Capture Frame
      ↓
⚫ Convert Frame to Grayscale
      ↓
🤖 Haar Cascade Face Detection
      ↓
📍 Detect Face Coordinates
      ↓
📦 Draw Bounding Boxes
      ↓
🖥️ Display Frame
      ↓
🔁 Repeat
```

---

## 🛠️ Important Functions

* 📹 `cv2.VideoCapture(0)` → Opens the default webcam.
* 🎞️ `video.read()` → Captures each video frame.
* ⚫ `cv2.cvtColor()` → Converts each frame into grayscale.
* 🔍 `detectMultiScale()` → Detects faces.
* 📦 `cv2.rectangle()` → Draws bounding boxes around detected faces.
* 🖥️ `cv2.imshow()` → Displays the live video.
* ⌨️ `cv2.waitKey(1)` → Refreshes the video frame and checks for keyboard input.
* 🔓 `video.release()` → Releases the webcam.
* ❌ `cv2.destroyAllWindows()` → Closes all OpenCV windows.

---

## ⌨️ Exit Condition

The program checks for the **`Q` key**.

```text
🔤 Q / q
   ↓
🛑 Break the loop
   ↓
🔓 Release webcam
   ↓
❌ Close all windows
```

---

# 💡 Key Concept

The important idea in this OpenCV object-detection example is:

> 🧠 **OpenCV uses a pre-trained Haar Cascade model to detect faces by analyzing image features at multiple scales.**

The detected face coordinates are then used to draw **📦 rectangular bounding boxes** around the detected objects.

---

# 📝 Quick Revision

```text
🖼️ Image / 📹 Video
        ↓
⚫ Grayscale
        ↓
🤖 Haar Cascade
        ↓
🔍 Object Detection
        ↓
📍 Coordinates
        ↓
📦 Bounding Box
        ↓
🖥️ Display
```

---

# 🏁 The END! 🎉
