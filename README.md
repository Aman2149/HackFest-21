# HackFest-21
Repository contains data and code files for the creation of X-ray image classification model and Covid-19 cough voice model.

## CoviGenix

### Abstract and Idea 

Waiting in a tiring queue for a simple Covid-19 checkup after a long search for outlets for different services, expecting a result for days (which also can turn out wrong at times) is a significant nuisance. We bring to you CoviGenix as a solution to all these problems where you can check your Covid-19 health status at home with your voice or lungs X-ray images and get the pinpointed location of facilities nearby, thus constructing an AI based centralized application for all your Covid-19 related services.

Problem Statement - Developing a centralized AI embedded application for instant Covid-19 check-up and apt facilities for citizens and service providers. We sought to prepare two ML algorithms, to classify whether you are infected or not using Covid-19 cough voice data and X-ray images of Covid-19 infected lungs using Machine Learning deployed on an application for consumer usage.

Utilizing cough-voice data, Spectrograms, Spectral Centroid, Zero Cross rate, Chroma Frequencies, Spectral Roll-off and, MFCC will be extracted and preprocessed using SMOTE, Autoencoders and General Adversarial Networks with a final model built using Gradient Boosting Decision tree algorithm and ANN. Through X-ray images of lungs, features such as Mel-Spectrograms will be extracted. Data preprocessing will take place by the methods of DownSampling, GANs and, Autoencoders, subsequently, building a Convolutional Neural Network on the dataset. The Covid-voice data was gathered from KaggleCCR, Virufy, Coswara and, COUGHVID and, X-ray images consist of a total of 6800 images that were self-scraped from online platforms. 

The Android application will be written in Kotlin, incorporating Model-View-ViewModel (MVVM) architecture. Key libraries include Android Jetpack's Navigation component for navigation, RecyclerView as a key UI element, Firebase for user authentication and, Retrofit for handling API requests. The proposed solution also has an OTP based login services part, where users can enter either as patients or as providers of services. 

The ‘Patients’ section of the application will register basic details of users like Phone Numbers, Address and Location coordinates. They can select their requirement from a list and view the locations of hospitals and service providers dealing in that commodity on a map. They can place a request for the commodity by selecting amongst a list of hospitals sorted by their proximity to the patient’s location.

The Provider part of the app will be responsible for listing out the requests in ascending order of distance. Providers can toggle the visibility of commodities and contact requesting patients via phone to coordinate the delivery. If the patient gives his/her consent to share the address with the provider, the address will get shared and the provider will be able to deliver the commodity.

A common aspect of both parts will be the ‘Community Request’ section. If a patient is unable to find providers in his range, he can create a community request specifying his/her name, phone number and, town/city. Other users of the application (including providers) can view such requests sorted in ascending order of the distance between their and the patient’s location. Fellow patients can share contact details to the given phone number. Providers can contact the patient to coordinate deliveries. The patient will mark the request as done after successfully availing the commodity.

