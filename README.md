# Waste_CLassification_machine_model


Project Overview

The Waste Classification Machine is a web-based application built using Django and integrated with a Teachable Machine image classification model. The system is designed to automatically identify the type of waste captured through a user’s camera. By utilizing machine learning, the application classifies waste into categories such as Biodegradable, Non-Biodegradable, and Recyclable, helping users improve their waste segregation practices.
This system functions as an accessible, educational, and environmentally focused platform. It is intended for students, households, small communities, and individuals interested in responsible waste disposal. The project is developed by a team of four members and serves as a final requirement for a course centered on machine learning and web development.
The project aims to show how modern technologies, specifically machine learning, web frameworks, and server interaction can be combined to address real-world environmental challenges. Waste segregation remains one of the most difficult tasks in many communities due to lack of awareness, inconsistent practices, and confusion regarding proper disposal. By simply using a camera, this system can help guide users toward more responsible waste categorization.

Learning Outcomes

Through this project, students were expected to classify different types of wastes using a machine learning model trained through Teachable Machine. By working on real-world waste classification, students learned how machine learning can be applied to solve environmental problems such as improper waste segregation and recycling inefficiency.


Functional Requirements : User Roles

The system supports three types of users:
Guest User
 Can capture images, run predictions, and view basic information.
Admin
 Can manage users, view system-wide analytics, and maintain stored predictions and class labels.
Input Interface
The system accepts camera capture.
Inference
Server-side Inference (Django + TensorFlow):
Django backend loads the TensorFlow model (.h5 or SavedModel format).

Page Design
Inline CSS is used in compliance with project requirements.
Django Templates render HTML pages such as:
Index.html - The logging-in page and main page 


Technical Constraints & Technology Stack
Backend
Django 4+
Python 3.10+
TensorFlow for server-side inference
Database
Firebase (Firestore/Realtime Database)
 Stores:
Prediction logs
User data
Front-end
Django Template Engine (HTML)
Inline CSS
Javascript (for functions) TensorFlow.js (for browser inference)
Model Export
Teachable Machine → TensorFlow.js model
Data, Training, and Evaluation
Training Dataset
At least 3 waste classes
Minimum of 100 image samples per class
Classes are:
Biodegradable
Non-biodegradable
Recyclable


User Journey / Workflow
The user visits the web.
Users sign-up for an account then, account gets stored in Firebase.
User Logging-in
User start the camera 
The model predicts the waste category.
Users use the camera for capturing images.
Results pop-up displays:
Class name
Prediction score
Disposal result recommendations


Conclusion
The Django Waste Classification Machine successfully integrates machine learning into a functional web application. By using Teachable Machine, TensorFlow.js, and server-side TensorFlow, the system provides a hybrid inference pipeline that is fast, accurate, and accessible. The project demonstrates the team’s ability to combine front-end, back-end, machine learning, ethics, and deployment skills into one cohesive platform.
