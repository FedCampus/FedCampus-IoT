# Overview

### Motivation

Since we have FedFT (see platform) algorithm whose correctness is verified by some experiences, devices, and student resources on our campus, we can make this theory a practical application. Therefore, we decided to develop a FedCampus platform based on FedFT algorithm and may cater to more FA algorithms in the future.

### Preview

This project implements an Android App to collect health and exercise data for FL training. It has two main function: data collection and local differential privacy (DP). Besides, this project also needs support iot for FL training, e.g: using smart watch.

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

### **Functions** (HealthKit Application)

* **Data Collect**: data from wearable devices.
  * **Store** data in a secure and encrypted format, and apply privacy-preserving technologies to the data, such as differential privacy.
* **Data Analytics**: Process data to extract insights and patterns.
  * Data cleaning: This involves identifying and correcting errors in the data.
  * Data transformation: This involves converting the data into a format that is easier to analyze.
  * Data analysis: This involves using statistical and mathematical techniques to identify patterns and trends in the data.
  * Data visualization: This involves creating graphs, charts, and other visuals to help communicate the findings of the data analysis.
* **Data Collaboration**: Share data with authorized users, recommendation, FL...

Additionally functions:

* **Data Collaboration**: Share data with authorized users, recommendation, FL...

| Person            | Work                                                                                                                | Time Due             |
| ----------------- | ------------------------------------------------------------------------------------------------------------------- | -------------------- |
| Jingheng, Beilong | Data Collection from wearable devices.                                                                              | By the end of May    |
| Beilong           | Backend & privacy techniques (Store data in a secure or encrypted format and apply privacy-preserving technologies) | Mid of May           |
| Beilong           | Data Collaboration & Privacy techniques for FL                                                                      | By the End of Summer |
| Jingheng, Shuhao  | App Implementation - Frontend                                                                                       | End of June          |
| Jingheng          | Data Analytics (Data cleaning, Data transformation, Data analysis, Data visualization)                              | By the End of Summer |

#### Resources

* Apollo server: [https://blog.csdn.net/weixin\_39808143/article/details/112576683](https://blog.csdn.net/weixin\_39808143/article/details/112576683)
* Ali Cloud: [https://help.aliyun.com/document\_detail/163032.html](https://help.aliyun.com/document\_detail/163032.html)
* Health Kit: [https://developer.huawei.com/consumer/cn/doc/development/HMSCore-Guides/apply-kitservice-0000001050071707](https://developer.huawei.com/consumer/cn/doc/development/HMSCore-Guides/apply-kitservice-0000001050071707)
* Health Kit Data: [https://developer.huawei.com/consumer/cn/doc/development/HMSCore-Guides/overview-0000001147638696](https://developer.huawei.com/consumer/cn/doc/development/HMSCore-Guides/overview-0000001147638696)
* Health Kit Overview：[https://developer.huawei.com/consumer/cn/codelab/HMSHealthKit-StepCount/index.html#0](https://developer.huawei.com/consumer/cn/codelab/HMSHealthKit-StepCount/index.html#0)
* Semi-finished code

{% embed url="https://github.com/Thea-Feng/FedC.git" %}
**Semi-code**: for easiness, just look at what is used by MainActivity.
{% endembed %}

| Time                     | Task          | Progress |
| ------------------------ | ------------- | -------- |
| During Semester (A)      | Communication |          |
| During Semester (A)      | Data Storage  |          |
| During Semester (B)      | Algorithm     |          |
| During Semester (B)      | UI            |          |
| 1st month (Summer) (A,B) | Health Kit    |          |
| 2nd month (Summer) (B)   | Smart Watch   |          |
| 2nd month (Summer) (A,B) | Test App      |          |

#### Task

* Communication
* Data Storage
* Algorithm
* UI
* HealthKit & FL Platform

#### Communication

* Build a Apollo broker
  * Build a server to monitor message communication
  *   To verify correctness, use Mqtt.fx / MqttX / EMqtt

      <figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
*   Fix the bug of MQTT subscribe

    * Publish function is implemented well. But there's a little bug in subscribe function: messageArrived is not called when subscribing message (in MainActivity.java)
    * You can also implement TCP version and forget about all the structure of MQTT if you are good at TCP

    <figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

#### Data Storage

* Local storage: LitePal (finished)
* Cloud storage: Ali Cloud (supporting MQTT), setup a dashboard by the instruction in resources (to do)

#### UI (Easy task)

* Beautify
* English version for international student
* ![](<.gitbook/assets/image (2).png>)![](<.gitbook/assets/image (4).png>)

#### Algorithm

* Implement local differential privacy algorithm

#### Health Kit

* After obtaining the authentication, plug in health kit to let the app automatically collect data
* Smart watch plug-in: collect data from the watch
