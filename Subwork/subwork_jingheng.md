# subwork\_Jingheng

• Finished set up Apollo and Built a server to monitor message communication 3.1-3.5
• verified correctness by using Matt.fx 3.11-3.13

For the following weeks:
1. Debug the subscribe function in MainActivity.java
2. Learn some knowledge about TCP (packet format, connection establishment, data transfer, and connection termination.
3. Learn some knowledge about Litepal APIs and Kotlin.


<font color="red">feedback:
- Next week, please work on communication part (you can learn datastore later). You need to know the basic mechanism of communication, which you will implement later.
- Next task: please setup HealthKit environment
</font>
-------------------------------------------------------------------------------------------------------------------------------------------
Update Mar 22nd:
- Registered a developer account on the Developer Alliance and created an application, configured application information, and applied for Health Kit services in the Developer Management Console.

- Created a project using Android Studio IDE and configure the SDK to access HUAWEI Health dependencies.
- According to the HUAWEI Health Development Guide, implemented API calls and debugging for HUAWEI Health open services.
- Createed an AGC (AppGallery Connect) application and Android Studio project.
- Generated a signing certificate and a signing certificate fingerprint.
- Configured the signing certificate fingerprint.
- Added the application package name and saved the configuration file.
- Configured the Maven repository address and configured the SDK to access HUAWEI Health dependencies.
- Configured the signing file in Android Studio.

- Integrate HMS Core SDK: (1): Configured the Maven repository address for the HMS (Huawei Mobile Services) Core SDK.
- Added compilation dependencies.
- Configured the AndroidManifest.xml file.
- Modified the applicationId
- Completed the app signing process

For the following weeks:
- Run the initial project (download the original framework code)
- Add login code.
- Request user authorization
- Register real-time data listener
- read real-time data
- close real-time data listener.
-------------------------------------------------------------------------------------------------------------------------------------------
Update Mar 29th:
- Learned the basics of Android app development, including concepts such as Activity, layout, and event handling, laying the foundation for future app development.
- Gained a deep understanding of the TCP protocol, including aspects such as packet format, connection establishment, data transfer, and connection termination. Studied how to implement TCP communication functionality in Android apps.
- Read the HUAWEI Health development documentation, learned how to integrate HUAWEI Health-related features into Android apps. Understood the application and configuration process of Health Kit services.
- Learned the Kotlin programming language, became familiar with its basic syntax and programming paradigms. Mastered the method of writing code in Kotlin for Android apps.
- Began researching how to implement user login functionality in Android apps. Understood the OAuth 2.0 authorization process and attempted to apply it to the project.

For the following weeks:
- Complete the development of the login feature, implement user authorization, and ensure that the app can access HUAWEI Health data normally.
- Register real-time data listeners and learn how to monitor and read real-time data.
- Develop and improve the main functions of the app, including data display, data synchronization, and data analysis.
- Optimize and refactor project code to improve code quality and maintainability.
- Prepare project documentation, including requirements analysis, design specifications, and user manuals.
-------------------------------------------------------------------------------------------------------------------------------------------
Update Apr 5th:
- Found a demo given by Huawei Health Kit https://developer.huawei.com/consumer/cn/doc/development/HMSCore-Examples/healthbasic-examplecode-0000001073728936. https://github.com/HMS-Core/hms-health-extention-demo/blob/master/README_ZH.mdIt (this one is optional since it only offers some extension functions that might not necessary for our project, just for a reference) The first URL link offers both Java and Kotlin version demos. In the README file, it already obtain (1) Login and authorization Allows users to log in to their accounts, and obtains the read and write permissions on fitness and health data, (2) Authorization cancellation Allows users to cancel account authorization, (3) Fitness and health data management Supports adding, deleting, updating, and querying authorized health and fitness data, etc. However, by following the doc given by Huawei Health KIt, we can't find the plugin called "HMS Toolkit" in the market of the plugin as they said, but this plugin is important for us to double check whether our configurations are set up like obfuscation and code signing certificate. Also, we are trying to figure out how to finish the configuration, and run our demo in both physical and vertual devices. We hope that next week we can make our app to achieve some basic functions as we expected.

- For the following weeks:
- Coorperate with Shuhao, Beilong to figure out how to combine the API calling in the demo and the UI design together to finish our own Android App.
- Figure how can we use this app to colloborate with the server we build from Platform group
- Finish debugging and testing
- Prepare for the app deployment

Update May 26th:
- Added email validation and password length checking in Android App login page

Update May 27th:
- Finished install Fedml in terminal and run FedML in docker: https://doc.fedml.ai/starter/installation.html
