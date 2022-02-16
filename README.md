# MedicineRecognizer

How to train and link your Teachable Machine Model:

Training:

1: Open https://teachablemachine.withgoogle.com

2: Click on "Get Started".

3: Click on "Standard Image Project".

4: Change "Class 1" to the first medicine's name.

5: Change "Class 2" to the second medicine's name.

6: If there are more than two medicines, click on "Add a class" and change "Class 3" to the third medicine's name. Repeat until all medicines have a class. If there are only two medicines, skip this step.

7: Click "Webcam", and, if prompted, allow camera access.

8: Hold up the first medicine, ideally with your face away, and hold the "Hold to Record" button.

9: Get at least 250 Image Samples, and then release the button.

10: Repeat steps 7, 8, and 9 for each medicine class.

11: Click on the "Train Model" button.

12: Wait for the model to fully get trained. DO NOT switch tabs, or the training will stop.

13: After the model is trained, test the model by holding up all medicines one after the other.

14: If the model works correctly, click on the "Export Model" button. This will popup a box with the source code and link. Make sure your on the "Tensorflow.js" tab, and click on "Upload".

15: Wait for the model to upload, and copy the link.

LINKING IN THE CODE:

1: Go to the Github page and go to code. Now go to "main.js" and find the line of code: 

classifier=ml5.imageClassifier("/model.json",modelloaded);

2: Before the slash, paste your link. The format should look like this:

classifier=ml5.imageClassifier("https://teachablemachine.withgoogle.com/models/code/model.json",modelloaded);

Done! Save the code, and you can start using the app!


