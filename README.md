#Introduction
Medical imaging more specifically X-ray examinations, is a key factor in the detection of bone disorders like fractures and degenerative changes. Manual interpretation and reporting by radiologists traditionally is laborintensive and human-error-prone, especially in low-resource settings. Artificial intelligence allows us to automatize these activities, improving efficiency, accuracy, and accessibility.This project propose a novel system that employs computer vision to scan images and NLP to generate humanreadable diagnostic sentences. By automating X-ray diagnoses, the system is capable of helping doctors make faster and more precise decisions, thereby improving patient outcomes. The proposed model includes Resnet50 for visual feature extraction, a neural classifier for binary classification and for generating report text-to-text transfer transformer is used. The gap between computer vision and NLP will be reduced by this combination in healthcare applications. 
#User Interface and Key Features 
The user interface was developed as a cross-platform mobile application using React Native and the Expo framework, allowing for deployment on both Android and IOS from a single codebase.
1. Cross-Platform UI: The use of React Native's component-based architecture facilitated rapid development and ensured a consistent user experience across different operating systems.
2. Image Acquisition Module: The UI includes features for: Gallery Upload, permitting selection of existing medical images from the device's storage.
3. Interactive Reporting and Visualization: The generated report text and the Grad-CAM heatmap are rendered visually on the original X-ray image, allowing the user to immediately verify where the model focused its attention to make the diagnosis, thereby fostering trust and aiding clinical review.
4. Diagnosis History Management: A dedicated section of the UI allows the user to:
4.1. View History: Display a chronological list of all previous diagnostic submissions retrieved from the /api/history endpoint.
4.2. Retrieve Details: Tap on a list item to view the full details of the past diagnosis, including the image, the full report, and the associated Grad-CAM visualization.
4.3. Delete Records: A dedicated action is provided to allow the user to permanently delete individual history records, communicating this request to the backend via the DELETE API endpoint for complete data removal.
<div align="center">
    <h2>📸 Application Screenshots</h2>
    <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 10px;">

        <img 
            src="https://raw.githubusercontent.com/nahidforhad/Xray_Report_Generator/main/assets/WhatsApp%20Image%202025-12-09%20at%201.02.59%20AM.jpeg" 
            alt="Screenshot 1 - Main Screen" 
            width="180" 
            style="border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);"
        />
        
        <img 
            src="https://raw.githubusercontent.com/nahidforhad/Xray_Report_Generator/main/assets/WhatsApp%20Image%202025-12-09%20at%201.02.59%20AM2.jpeg" 
            alt="Screenshot 2 - Selection Dropdowns" 
            width="180" 
            style="border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);"
        />
        
        <img 
            src="https://raw.githubusercontent.com/nahidforhad/Xray_Report_Generator/main/assets/WhatsApp%20Image%202025-12-09%20at%201.02.59%20AM3.jpeg" 
            alt="Screenshot 3 - Abnormal Report" 
            width="180" 
            style="border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);"
        />
        
        <img 
            src="https://raw.githubusercontent.com/nahidforhad/Xray_Report_Generator/main/assets/WhatsApp%20Image%202025-12-09%20at%201.02.59%20AM4.jpeg" 
            alt="Screenshot 4 - History" 
            width="180" 
            style="border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);"
        />
        
        <img 
            src="https://raw.githubusercontent.com/nahidforhad/Xray_Report_Generator/main/assets/WhatsApp%20Image%202025-12-09%20at%201.02.59%20AM5.jpeg" 
            alt="Screenshot 5 - Normal Report" 
            width="180" 
            style="border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);"
        />
    </div>
</div>

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
