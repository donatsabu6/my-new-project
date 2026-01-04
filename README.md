# The Digital Agronomist: AI-based Crop Disease Detection & Consultation

Final project for the Building AI course

## Summary

The Digital Agronomist is an AI-powered assistant that helps farmers identify crop diseases in staple crops (cassava, bananas, maize, beans, soybean, peas) from smartphone photos, and receive farming advice through a natural-language chatbot. It combines image recognition and conversational AI to support better crop health management and decision-making.


## Background

Smallholder farmers often struggle to identify crop diseases early due to limited access to agronomists and agricultural extension services. Misdiagnosis or delayed action can lead to significant crop losses and reduced food security.

Common challenges include:
* Difficulty identifying crop diseases accurately from visual symptoms: Many small-scale farmers lack the specialized knowledge to distinguish between similar-looking diseases.
* Limited access to timely, expert agricultural advice: In many rural areas, access to professional agronomists is often limited and expensive.
* Crop diseases can devastate harvests, leading to significant financial loss and food insecurity: Early detection can save up to 40% of a harvest that would otherwise be lost to preventable spread.
* Dependence on trial-and-error or outdated farming practices

My personal motivation comes from the importance of agriculture in many developing economies and the potential of AI to make expert knowledge more accessible. This topic is important because early disease detection and informed decision-making can improve yields, livelihoods, and sustainability.

## How is it used?

A farmer uses a mobile device to take a photo of a crop leaf or plant suspected to be unhealthy. The AI system analyzes the image and predicts whether the crop is healthy or affected by a known disease. The farmer can then interact with a chatbot to ask follow-up questions and receive explanations, prevention tips, and general farming advice.

The solution is intended for use:
* In rural farming environments
* Directly in the field
* During planting, growing, or early disease outbreak stages

The main users are smallholder farmers. The system should be easy to use, work with low-cost smartphones, and provide responses in simple, understandable language.

## Data sources and AI methods

The image data can come from:

* Photos collected directly from local farms
* Publicly available datasets such as PlantVillage for initial training

The chatbot knowledge can be built using:

* Curated agricultural guides
* Public agricultural extension resources

AI methods used include:

* Computer Vision (image classification using convolutional neural networks): I will use Convolutional Neural Networks for image classification. Training data will come from the PlantVillage Dataset combined with local images collected from the field to ensure regional accuracy.
* Transfer learning with pre-trained image models: To make the model efficient, I'll use a pre-trained model (like MobileNetV2) and "fine-tune" it on my specific set of crops (bananas, beans, soja, peas, and maize).
* NLP & Generative AI techniques for flexible, non–rule-based responses: The chatbot will utilize a Large Language Model (LLM) fine-tuned on agricultural manuals and research papers.


## Challenges

This project does not replace professional agronomists or guarantee perfect diagnosis. Limitations include:

* Accuracy vs. Environment: Photos taken in poor lighting or with blurry backgrounds can lead to "False Positives," where a healthy plant is labeled as diseased
* Hallucinations: In generative AI, the chatbot might suggest a pesticide or treatment that is not available or safe in the farmer's specific region.
* Internet Dependency: While the vision model can be stored on the phone, the generative chatbot typically requires a cloud connection, which may be unavailable in remote areas.
* Risk of users over-trusting AI recommendations



Expansion: Adding more crop varieties and support for local languages using speech-to-text.

IoT Integration: Connecting the app to low-cost soil sensors to predict disease outbreaks before they are visible to the eye.

Needs: To move forward, I would need a partnership with local agricultural universities to verify the AI's advice and access to cloud infrastructure for hosting the generative model.

## What next?

The project could evolve from a diagnostic tool into a full-scale farm management system.

The project could be expanded by:

* Supporting more crop types and regional diseases
* Adding local language support and speech-to-text feature
* Integrating weather and soil data (IoT Integration) to predict disease outbreaks before they are visible to the eye.
* Deploying as a full mobile application

To move forward, additional needs include

* More diverse and labeled datasets
* Collaboration with agronomists and agricultural institutions
* Skills in model deployment, mobile development, and user-centered design
