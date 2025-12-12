#Introduction: 
Medical imaging more specifically X-ray examinations, is a key factor in the detection of bone disorders like fractures and degenerative changes. Manual interpretation and reporting by radiologists traditionally is laborintensive and human-error-prone, especially in low-resource settings. Artificial intelligence allows us to automatize these activities, improving efficiency, accuracy, and accessibility.This project propose a novel system that employs computer vision to scan images and NLP to generate humanreadable diagnostic sentences. By automating X-ray diagnoses, the system is capable of helping doctors make faster and more precise decisions, thereby improving patient outcomes. The proposed model includes Resnet50 for visual feature extraction, a neural classifier for binary classification and for generating report text-to-text transfer transformer is used. The gap between computer vision and NLP will be reduced by this combination in healthcare applications. 
<div>
<h1>#User Interface and Key Features:</h1>
The user interface was developed as a cross-platform mobile application using React Native and the Expo framework, allowing for deployment on both Android and IOS from a single codebase.
<div>1. Cross-Platform UI: The use of React Native's component-based architecture facilitated rapid development and ensured a consistent user experience across different operating systems.</div>
<div>2. Image Acquisition Module: The UI includes features for: Gallery Upload, permitting selection of existing medical images from the device's storage.</div>
<div>3. Interactive Reporting and Visualization: The generated report text and the Grad-CAM heatmap are rendered visually on the original X-ray image, allowing the user to immediately verify where the model focused its attention to make the diagnosis, thereby fostering trust and aiding clinical review.</div>
<div>4. Diagnosis History Management: A dedicated section of the UI allows the user to:</div>
<div>4.1. View History: Display a chronological list of all previous diagnostic submissions retrieved from the /api/history endpoint.</div>
<div>4.2. Retrieve Details: Tap on a list item to view the full details of the past diagnosis, including the image, the full report, and the associated Grad-CAM visualization.</div>
<div>4.3. Delete Records: A dedicated action is provided to allow the user to permanently delete individual history records, communicating this request to the backend via the DELETE API endpoint for complete data removal.</div>
</div>    
<div align="center">
    <h2>📸 Application Screenshots</h2>
</div>
<img width="200" height="520" alt="image" src="https://github.com/user-attachments/assets/880c4a21-fdc6-49b6-99e5-1a9b0e0a1a52" />
<img width="200" height="520" alt="image" src="https://github.com/user-attachments/assets/6164975b-cdc5-403a-844d-90beedce1948" />
<img width="200" height="520" alt="image" src="https://github.com/user-attachments/assets/18132001-0747-4a60-b9b3-83bd7b291693" />
<img width="200" height="520" alt="image" src="https://github.com/user-attachments/assets/1616318d-0b82-4962-9379-674bd2baaede" />
<img width="200" height="520" alt="image" src="https://github.com/user-attachments/assets/43e47e55-b86b-4cfd-8e36-502f8977c46e" />

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
   npx expo start
   ```

In the output, you'll find options to open the app in a

- [development build](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go), a limited sandbox for trying out app development with Expo

You can start developing by editing the files inside the **app** directory. This project uses [file-based routing](https://docs.expo.dev/router/introduction).

## Get a fresh project

When you're ready, run:

```bash
npm run reset-project
```

This command will move the starter code to the **app-example** directory and create a blank **app** directory where you can start developing.

## Learn more

To learn more about developing your project with Expo, look at the following resources:

- [Expo documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with our [guides](https://docs.expo.dev/guides).
- [Learn Expo tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial where you'll create a project that runs on Android, iOS, and the web.

## Join the community

Join our community of developers creating universal apps.

- [Expo on GitHub](https://github.com/expo/expo): View our open source platform and contribute.
- [Discord community](https://chat.expo.dev): Chat with Expo users and ask questions.
