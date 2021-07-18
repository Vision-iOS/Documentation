# Vision

### General objective
Development of a mobile application for the iOS platform based on object recognition from an image to make subsequent image searches more efficient.

### Specific objective 
Given an image, the objects present are recognized and shown to the user as sequences of strings that identify the objects. The user can use an image already in his library or take it right now.  
Before analyzing the image, the user can make changes on it to better select the object to be recognized. The application must be able to save the image with the information of the objects recognized in the user's gallery without modifying and/or deleting the original image.  
The photo gallery must be able to analyze the strings of the photos to show the user the images based on the search performed.

### Expected results
The purpose of the application development must grant:  
- Make searching more efficient by taking advantage of tags/strings saved as metadata in photos exported and saved by the application.
- Allow users to obtain information about an object or sets of objects they do not know.
- Allow users to verify that an object or sets of objects match what they think they know.
- Establish a basis to be able to use the application for other types of contexts (recognition of road signs, recognition of hazards, etc).

## Why iOS
Below are the reasons that led to the development of an application for the Apple market on iOS devices.

### Market share
Android undoubtedly has a larger market share than iOS.  

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116373708-e54cf800-a80d-11eb-8080-3cd71be142d5.jpg">
</p>

It is therefore assumed that the best development choice for an application is to focus exclusively on the Android market.  
In reality, the market share is not the only element that influences the development of an application, but there are additional reasons that lead to a development choice for smaller shares.

### Latest version
IOS users are more likely to always keep their devices up to date. Although it may seem a completely irrelevant element for the development of an application, it can represent an excellent development point for iOS.  
This is because future enhancements of the application always cover the majority of users who have the latest version of the software. Normally a new software update from Apple brings significant new features and completely exclusive features only for devices that update to the latest version.  
Therefore, always having users willing to update, it is possible to propose an application that changes and changes following the continuous flow of updates knowing that most users will be able to use them.  

Instead with Android, you can get to cut users from future updates as they do not support the improvements of the new updates. The disadvantage for these users is the total fragmentation of the various major updates as shown by the graphs.  

#### iOS
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116373475-a8810100-a80d-11eb-8559-01126afb2c3a.jpg">
</p>
Updates in a growing list of years: previous versions, iOS 12, iOS 13.

#### Android
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116374444-92277500-a80e-11eb-8652-a675e1cf523f.jpg">
</p>
Updates in a growing list of years: previous versions, Nougat, Oreo, Pie.

### User loyalty
IOS users are more loyal to the manufacturer than owners of Android devices. A user who buys an Apple device is more likely to make future purchases from the same manufacturer. On Android, it is much more complex also because there are many companies (Samsung, Oneplus, Xiaomi and others) that release devices based on Android but *customized* and therefore that can lead to compatibility problems with certain applications that must be optimized for the specific device.  

This can be a strength for development on the iOS system, in fact, it is more likely that users who download the application will keep it for longer than Android users.  
This makes the downloaded application unique and difficult to replace in the future.

### Demographics
Several countries with the highest incomes, including the United States, some European countries, and Australia, prefer iOS.  
On average, people who prefer iOS are younger than people who prefer Android.  
Therefore, there is a target of people who are more inclined to adapt to the type of application and the novelties it entails.

### Spending power
Apple's App Store has more revenue from mobile apps than the Google Play Store.  
Global gross revenue per app **only** in Q3 2019 is:  
- iOS: 14.2 billion.
- Android: 7.7 billion.

This is because the average iOS owner is willing to pay more to take advantage of a product knowing that it reflects the full potential and efficiency of the Apple system. Even if the application was developed for didactic purposes and the total passion of an open code, the possibility of future development of applications whose income is an essential source for the development itself is not excluded.

## Key elements
Some fundamental elements for the preliminary development of the application have been discussed.

### Language
The most obvious choice fell in proposing the application with the language of the device used.  
However, this preference would have led to the development of several different learning models based on the nation and language used, counting all the possible idioms and possible words with different meanings based on the context used.  
We, therefore, preferred to take advantage of a single model in the most influential and spoken language in the world, English.  

It is easy to conclude that a solution to the language problem is to get all the strings of the recognized objects in English and subsequently translate them into the local language. This option was discarded as it would involve the application using data traffic to translate while the idea of developing the application is based on being able to use it in its entirety in any geographical environment, even totally free of signals and radio waves.  
The possibility of integrating the entire linguistic dictionary locally has also been discarded since the application already holds the set of models for recognizing objects which leads to a large part of the memory occupied.

### Security and privacy
Essential in every application. In this case, from the point of view of security, the application requires access to any external tool it needs (camera and gallery). No changes are made to the photo chosen to be analyzed and a copy of the new photo is always created containing the keywords of the recognized objects.  
From the point of view of privacy, however, each photo is processed locally by the device itself, without sending information to external servers.

### All in one
As already mentioned in the **language** section, the strong point of the application is that it has all the functions completely locally without having to rely on a network to function. The motivation is based on the very concept of object recognition and the target users it is intended for.  
An application of this type implies in most circumstances that its use is external. This involves possible places where the use of mobile networks is not possible or in roaming situations where you try to limit the use of data traffic as much as possible.  
It was therefore decided to result in greater use of the phone memory while maintaining use of the application totally free from any condition in which the phone itself may be.

# Identifying the users target
## Types of users
Based on the design idea, the definition and construction of users must include:
- Users who need to use an application capable of building tags/strings quickly and efficiently without them having to do it.
- Users who want to exploit search methods to quickly find an image or sets of images based on one or more keywords.
- Users seeking knowledge of objects they do not know.
- Users who travel to places and places and do not understand the use of certain items. Through recognition, they can obtain a definition of the object and carry out appropriate research to understand its use.
- Curious users want to verify that an object is the one they already know.
- Users who want to be able to broaden their personal knowledge or verify the accuracy of an object or objects.

### Behavioral variables
The analysis is based on defining the user based on:

- How: how the application is used.
- When: when using the application.
- How much: how much does the application use.
- How to purchase: availability and access to the application.

#### How
The application is developed for Apple devices on iOS operating system and adapted to its most popular product: iPhone.  
This choice is based on the two cornerstones of development: mobility and speed. Mobility refers to the possibility of allowing the use of the application in any condition the user is in. According to the report of the Mobility Report in 2019, there are 5.9 billion people who have a smartphone, this allows us to consider that in most cases the user who has a smartphone always keeps it at hand. This condition has favored the development of the application for a mobile environment compared to other developments for other fixed platforms.  
Speed is necessary as the user who downloads an application, especially mobile, wants it to be functional and ready to use as soon as it is opened.  

Furthermore, we must consider the subject of object recognition which represents something very abstract and difficult to understand for a user (be it inexperienced or experienced). Based on this, the application must provide for totally basic and simplistic use.

#### When
Being developed for the mobile environment, the use of the application increases considerably as the smartphone is the most commonly used type of device.  
In this case, the user will use the application for short periods per session, while the use of the application itself can spread over long periods. That is, the analysis of an image requires little time and therefore the user does not need to continue as he has achieved his purpose by saving the image in the gallery but; once the operation has been verified, he will be led many times to use the application itself.

#### How to purchase
The method of purchase means the method by which the user can obtain the application.  
The application does not violate any law and/or rule of the store in which it is inserted for distribution and is valid for all ages. Obviously, this concerns the application and not how the user can use it, for example, it is valid to distribute an application that is based on object recognition in every country but it is not valid for the user to use it to analyze photos that are forbidden to use it. 'acquisition.  
We can therefore proceed to consider that the application can be available globally in the Apple store, reaching all users.

### Mapping of subjects
To understand the most prevalent behavioral variables, it was decided to build a questionnaire containing the following questions:

- What is your name?
- How old are you?
- Where are you from?
- Do you like taking pictures with your iPhone?
  - One answer: Yes, No, Indifferent.
- Do you have many photos saved on your device or in the cloud?
  - Single answer: Lots, Quite a lot, Very few.
- When looking for a specific photo, do you have difficulty finding it?
  - Single answer: Yes, No, Indifferent.
- Suppose you want to search for all the photos that have a pizza, can you do that?
  - Single answer: Yes, No, I've never tried.
- Based on the previous question, do you find interesting the idea of being able to immediately find all the photos that have a particular object such as a pizza?          
   - Single answer: Yes, No, Indifferent.
- Do you find the idea of being able to know the name of any object you photograph interesting?
  - Single answer: Yes, No, Indifferent.
- If you find yourself alone and see something you don't know, what do you do?
  - Multiple answers: I search the Internet by entering keywords of the object, I take a picture to send it to someone hoping to get information, I take a picture and try to look for it on the internet, Other [Specify].
- Based on the previous answer, if there was an app on your iPhone that allows you to instantly recognize the object you have photographed, would you find it useful?
  - Single answer: Yes, No, Indifferent.
- How important is privacy to you?
  - Single answer: Fundamental, Important but not always necessary, I don't care, Indifferent.
- Have you ever found yourself in places where your iPhone was completely isolated from the internet world (no Wi-Fi, data connection, mobile network)?
  - Single answer: Many times, sometimes, rarely, never.

The questionnaire allowed replies to be sent only if the user confirmed that they had an Apple iPhone device.  
The following are the relevant results for the development of the target users:  

#### Questionnaire Completion Age
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116406602-20acee00-a831-11eb-97f6-04ad8a703603.jpg">
</p>


#### You find it difficult to find specific photos
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116407861-7df56f00-a832-11eb-9bcc-8c4eb92a5aa2.jpg">
</p>


#### You find the idea of being able to instantly find all photos with a particular object interesting
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116407863-7e8e0580-a832-11eb-927f-725d6457ed44.jpg">
</p>

#### You find the idea of being able to know any object you photograph interesting
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116407866-7f269c00-a832-11eb-860d-cf5285bcc943.jpg">
</p>

#### If you find yourself alone and see something you don't know, what do you do
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116408724-71bde180-a833-11eb-877a-265892d0957d.jpg">
</p>

In *Other* replies have been received which involve: asking people nearby, completely ignoring the object, "taking" the object and others of lesser importance.

#### You find the idea of an app to instantly recognize an object interesting
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116408721-708cb480-a833-11eb-9f64-9052204fa5ed.jpg">
</p>

#### How important is privacy to you
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116409366-104a4280-a834-11eb-84a9-96127c4ac3cf.jpg">
</p>

#### Have you ever found yourself in places where your smartphone is completely isolated from the internet
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116409360-0fb1ac00-a834-11eb-92fa-ed53da938efb.jpg">
</p>

### Behavioral patterns
The unification of the recurring behavioral patterns led to:  
- Interest in an app that uses artificial intelligence or a model that goes beyond the subject's imagination.
- Get the information you need quickly.
- Sense of cataloging and having a mental order on a whole.

### Summary of characteristics and goals
Based on the survey carried out and other information, a user is preferred:  
- Age between 18-30.
- Subject to preserving a large amount of photos over time.
- Subject to obtaining an immediate and precise response.
- Tends to interface with one's smartphone if it does not have adequate information available.
- Open to innovations that exploit artificial intelligence.
- In charge of, in part, one's privacy.

## Personas
Below are the three personas representing the set of reference users for the application.  
<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116410206-d3cb1680-a834-11eb-924e-579ddd9a7dac.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116410212-d594da00-a834-11eb-94e5-f2cd94dda7e6.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116410215-d62d7080-a834-11eb-853b-3a86cf4d6028.png">
</p>

# Study of the evaluation of usability
## General development
The development of the application idea was based on the *"An interface design process"* model built from four blocks. Once the idea was defined and the users identified, a document was developed that describes the set of tasks that the application must perform. In particular, based on the idea that, given an image, the objects present are recognized and shown to the user as sequences of strings that identify the objects, the tasks include:  

The image can be input into the application in two ways:  
- Camera: you can instantly take a picture and decide whether to perform the analysis on object recognition.
- Photo library: all photos in the photo library can be sent to the application.

Before carrying out the analysis of the objects, the user is allowed to make any changes such as:  
- Selection changes: the user can choose whether to select a specific object within the image in such a way as to make object recognition more precise. If you subsequently decide to save the image, the application will save the entire image taken and not just the previously selected object. This choice allows the user to operate with the same image but meticulously selecting each object and then saving the whole image as a whole.
- Image rotation: allows the image to be rotated left and/or right.
- Scale: set of predefined dimensions for working with the image. For example, the user can render the image for analysis in 4: 3, 3: 2, 19: 9 and other dimensions.
- Reset: cancels any changes that have been made.  

Once the objects have been recognized, the user can optionally delete the sequence of strings that have been associated with the object. Once finished, the image is saved in the photo library as a new image without overwriting the old one. The new image will have stored as metadata the set of strings chosen by the user.  
The latter can type one of these strings in the search field of the photo library to immediately obtain the image and/or set of images containing that word.  
The analysis and set of activities required for each task are discussed later.  

Considering the feasible idea, we moved on to the product elaboration phase through the development of a prototype. This was conceived in the first part of the low fidelity wireframe typology. In this case, the evaluation on the refinement of tasks and usability was subject to the internal members of the project and a limited number of people among the survey participants. Subsequently, the prototype was modeled in such a way as to become interactive and usable by the testers chosen through training tests.  

We then moved on to the usability test phase, discussed later.  
During the test phases, we started to develop the code-side bases of the actual application following the development of the prototype up to the complete software.

## Ben Shneiderman
They represent a fundamental set of rules on which the application was developed, from the prototyping phase to the final software. In particular:  
- Consistency at all costs: colors, layout and lettering are consistent with every part of the system. The font used for the character strings is the same for the system and for each application. The use of **bold** allows to enhance and attract the user's attention to express important information. The use of colors adapts to the state of the system, from the light to the dark version, for greater consistency.  Finally, the layout has been built to remove all non-salient information to give greater immersion.
- General usability: based on the target of users, the needs of the different types of users are recognized, considering users of "almost" all ages with different technological backgrounds. The interface is made simple and clear, and at the same time elegant and captivating.
- Offer training feedback: every action by the user is associated with a response from the system. Any operation the user performs on the interface, latter will provide feedback, even imperceptible, completely visible and understandable to the user. For example, when the user presses a button this will make an animation on his color to give the idea that it has been physically pressed.
- Dialogue with users: each sequence of actions has a beginning, an intermediate point and an end that is totally understandable to the user. For example, if the user analyzes an image, he will import it, modify it and finally obtain the final point will be given by the system which shows the list of recognized objects.
- Handling of errors: the simplicity of the development of the interface has made it possible to minimize the possibility of errors. Any errors such as the lack of access to a photo, the inability to recognize objects in an image and others are managed through special pop-ups and/or writings that clearly show the user the type of error that occurred.
- Allow to go back: the user has full control of the interface. He can always return to a previous screen about the continuity of the same. That is, if the user passes from screen A to B and from B to C, if he goes back he will pass from C to B and not to A, thus following the precise flow of the screens.
- Ensure user control: the user is at the center of the system. The interface responds to every input without hesitation.
- Reduce short-term memory overload: the application was designed to comply with the rules of number 7. There is no information that the user must keep memorized or particular icons associated with specific functions.

## Fitts law
One of the most frequent actions performed by those who interact with a system is to move the pointer or finger on a target. In this case, the main interface holds the button to import photos in the center of the screen, not only for a better visual experience but to take full advantage of Fitts' law, that is to have a completely reduced time to reach by a finger the specific button. Screens tend to get bigger and bigger but the grip of a smartphone always tends to bring the thumb towards and beyond the center of the screen. Inserting the buttons too low would have led to a handle that for very large devices can cause problems in holding the smartphone with one hand, instead of, with a centered button you try to favor the grip and not ask for effort on the part of the 'user.  
The buttons for editing a photo, on the other hand, are placed at the bottom as it was preferred to give space to the vision of the user's image and the complete possibility of being able to make series of cuts to the image in real-time without pressing any buttons.  
Finally, each screen holds the possibility of being able to go back with the appropriate buttons at the top left, as per Apple's development rules, but in addition it supports the possibility of switching to the previous screen by swiping the finger from the left edge to the right, in any vertical point on the edge. This allows the user to go back the screen without having to reach the top of the bar to press the button.  
The saving has been inserted in the bar at the top right as the concept of saving the image allows the completion of the application and is seen as something in which the user must be sure you want to terminate and therefore not *"reachable"* in a super immediate way like the button to import an image.

## Gestalt Laws
**"The set is the sum of its parts"**. 

Gestalt laws play a very important role in defining the interface. For example, considering the following images below we can see the use of some laws.  
The law of proximity and closure allows you to collect as a single unit elements such as *camera* and *photo library* being tools for image selection, or the whole of recognized objects. All these elements are separated by lines using the law of continuity of direction that allows you to identify each object separately but see them as a single entity.  
The law of similarity allows recognizing elements to be pressed such as *camera*, *photo library* and *cancel* and others on which to immediately catch the attention such as the writing of the recognized objects. Finally, the law of past experience is enclosed in the export button of the image at the top right in the image used and recognized by iOS users to share and export.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116411763-4c7ea280-a836-11eb-9599-ca5ef9c0bdb7.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116411771-4e486600-a836-11eb-99b0-74ea2be163db.png">
</p>

# Feature Analysis

## Prototyping
Due to the worldwide COVID-19 emergency, it was preferred to structure the prototyping on an interactive model in such a way that it can be used for usability tests carried out remotely in total safety and compliance with the rules.

## Functional
The application has the following features:  
- Tutorial.
- Image import via photo library.
- Image import via camera.
- Ability to cancel the image import selection operation.
- Ability to cancel the operation of taking a photo.
- Selection of use of the front or rear camera.
- Taking a photo.
- Ability to use the photo taken or take a new shot.
- Image modification by specific selection.
- Image modification by rotation.
- Changing the image by scaling.
- Reset image changes.
- Undoing image editing.
- Object recognition is based on the given image.
- Creation of table containing recognized objects.
- Deletion of one or more recognized objects by the user.
- Saving the image with the corresponding metadata on the recognized objects.
- Ability to go back through the screens.
- Light / dark theme according to device settings.

## Visual
The prototype is available at the following address: https://4cni7n.axshare.com  
If you use the file in the folder you must have the Axure software available at the following address: https://www.axure.com.

## Systemic
Below is the state machine diagram.  
*Click on the image to enlarge*
![Statechart](https://user-images.githubusercontent.com/22590804/116412525-11c93a00-a837-11eb-8719-a9767dc96cca.jpg)

# Field evaluation of subjective and/or objective usability
## Interfaces analysis

### Tab-bar
The layout of a tab bar allows the user to access the main screens of the application. Each screen selected is highlighted through the appropriate color that highlights the state in which the system is located.  
In addition to a descriptive text of the screen, there is a representative icon. The latter allows you to take advantage of the recall to the user's past experience by retrieving information through association. In this way the user, even a novice, can identify the appropriate screens of the application without having to focus on the textual part.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116413112-9caa3480-a837-11eb-9453-672d7385212d.jpg">
</p>

The bar is structured to be always visible, allowing the user immediate access to the cardinal functions of the application. Only in specific cases, the bar is temporarily hidden to increase the sense of immersion on the part of the user; for example when viewing an image. In this way the user has full control over the image, through the use of gestures, avoiding errors due to unintentional or spontaneous actions.  
The bar and associated interfaces hold a limited amount of information that avoids overloading the user's short-term memory. Each feature has been structured to have a beginning, an intermediate point and an end without tiring the user to remember a lot of information.

### Search
The search section allows the user to operate with the entire set of images on which he has carried out the analysis. The search is divided into three *tab* to better diversify the actions that the user can perform on the same data.  
Each tab has a search bar to filter information based on the input transcribed by the user. The search bar is structured to offer the best user usability. Through the image below the user can perform the entire deletion of what he has typed using the appropriate button with the *X* icon, avoiding having to delete every single character using the keyboard. Using the *Cancel* button the interface is restored in its entirety.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116413476-f0b51900-a837-11eb-9b41-7221c21577af.jpg">
</p>

The search bar allows you to filter the tags in each of the three tabs, maintaining consistency on the type of information shown to the user. For example, in the *Grid* tab the subset of *images* filtered by tag will be shown, in the *Tag* tab the filtering takes place using the *tags* themselves.

### Grid
The tab represents the main interface in the search section. The identifier of the *Grid* tab is associated with the grid arrangement of the images. The user has the immediate visualization of the images on which he has carried out the analysis and by pressing on one of these he will be able to view them in their entirety as described before.  

Image management can be done by using the *Edit* button with which the user can select and delete images. The user perceives the state of the system in the image deletion mode as the search bar and the present tabs are inhibited from possible interactions. In this mode, the diversification of user actions is performed by having the image delete button placed at a distance from the one for exiting the deletion procedure. The *Delete* button is updated in the background in relation to the number of images selected by the user in such a way as to always provide the latter with the totality of the selected objects. In addition, each image chosen will be highlighted by a colored outline to distinguish them from the unselected ones.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116413932-55707380-a838-11eb-9c40-4affdf13f2f0.jpg">
</p>

By pressing the *Delete* button the user is asked to confirm the action he is carrying out. The confirmation request has been structured in such a way that:  

- the user accidentally presses the button and deletes the images.
- warn the user that he is faced with an irreversible action as it involves the definitive elimination of the selected images.

Further prevention of user error was coded by the use of colors. Using the color *red* the user is led to fully understand the possible danger of the action involved.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116414061-746f0580-a838-11eb-85b7-ea96324ff9e2.jpg">
</p>

Once the deletion is complete, the grid is automatically updated keeping its order of the photos not processed for deletion.

### Tag
The structure of the Tag tab is mainly composed of a **header** that contains the set of initials of the tags and a **index** that facilitates the scrolling and selection of specific tags.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116414550-da5b8d00-a838-11eb-9b24-37f437775b5f.jpg">
</p>

The header is structured through a coloring that allows the user to identify a group of tags simply and immediately. Using the index, however, the user can scroll directly to the specific tag group.  

In this section, as already shown before, the *laws of the Gestalt* come into play. In particular, we can focus on:  
- Law of proximity: all tags defined by the appropriate header are identified as a single unit as they define the same set of tags starting with the same letter.
- Law of similarity: each letter identifying the header is considered as a single unit that differentiates the subsets of tags.
- Law of continuity of direction: the use of lines delimiting the surface that point towards the same direction more easily makes up the sense of unity of the information being displayed.

By clicking on the name of a tag, the *Grid* interface is called, which contains the set of all images filtered for the chosen tag.

### Map
The map allows the user to obtain a localized view of their images through an *interactive* interface. It is possible to interact with the map using gestures that make use of the user's knowledge through **redundancy** and **coherence**.  
For example with redundancy the user can zoom in on the map in a specific area both through a double tap on the screen that through pinch in, instead of through coherence, the set of gestures now present in the standard use of touch screen devices are used.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116414966-40481480-a839-11eb-9182-498af9ac30c0.png">
</p>

Another call to consistency is the use of the orange pin identifying the user's current position. The use of this specific color allows the user to instantly perceive its location.  
Each image on the map is enclosed in a square to take advantage of the closing law and allow you to associate every single image in a more univocal way. The use of square thumbnails falls within the canon of consistency with the entire application (for example in the *Grid* section the image grid is constructed using square shapes).  

You can interact with each image on the map by selecting one of them. This interaction is partly **hidden** from the user as it takes advantage of part of the latter's experience on the use of the application itself. Since the application has been developed keeping the concept of image as a basic point, each image has maximum interactivity through the actions of the user. This avoided explicitly expressing the possibility of pressing on an image within the map.


<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116414971-41794180-a839-11eb-8b24-c5a69a2a5e02.png">
</p>

By selecting an image, the user will have a partial preview of the tags stored in the photo itself. The new interface part benefits from *ellipsis* and an *info* button. The former has the purpose of expressing to the user that the information is represented in its partiality and not in its entirety. This leads to the definition of a beginning of a sequence of actions that the user will conclude by interacting with the *info* button. Performing this interaction calls up the selected photo viewing interface, giving the user a sense of satisfaction at having completed an activity.

## Image View
Allows you to view the image chosen in your entirety.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116417028-32938e80-a83b-11eb-92b7-263845b118a1.png">
</p>

As previously stated, to obtain greater user immersion, the tab bar is hidden. Similar speech on the set of gestures with which the user can interact with the image.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116417041-358e7f00-a83b-11eb-888d-b1c1b73b65ac.png">
</p>

The navbar is built in such a way as to enclose the set of information associated with the image and not to hinder the user on the focal point: the image. The bar encloses the set of tags, showing them in a scrolling animation.  
The use of animation focuses the user on the entirety of the information present in the bar. When interacting with the image, however, the animation suffers a momentary suspension as the user is focusing on the image and not on the bar.  

The subtitle expresses the total number of images that can be displayed by scrolling. The information of the totality of the photos present identifies a sequence of actions organized with a beginning (opening an image), an intermediate point (scrolling through the images) and a conclusion (the user reaches the maximum number of photos on which he can operate).  
Lastly, the navbar consists of two buttons:
- Edit tags: calls the interface for managing tags described before.
- Save image: saves the selected image in the default gallery.

The use of coherence comes into play again by exploiting images that are coherent with the action that takes place.

## Tag management
The interface allows you to interact with the tags present in an image and/or recognized by the application.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116417447-8d2cea80-a83b-11eb-84de-5361e04d753a.jpeg">
</p>

The tags are shown through a vertical list as it allows you to use all the horizontal space possible for longer tags. Furthermore, this visualization leads the user to perceive a sense of information on the list, where he can interact on every single element.  
Based on this structure, the user can delete a chosen tag by scrolling to the left. This interaction exploits the law of past experience giving rise to a familiar system figure implemented in other applications in the iOS environment.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116417568-ac2b7c80-a83b-11eb-8863-f5ac2dd52c8d.jpeg">
</p>

Using the *Plus* button the user can add one or more tags to the reference image. The interaction with the button leads to the opening of the keyboard and a panel that specifies simply and effectively the action to be performed.  
The panel consists of two buttons that cancel or add the user's tag. Both have different colors and in particular the *Add item* button is represented with the red color. Normally the use of this color expresses dangerous or destructive actions while in this case it outlines the completeness of the action of adding a tag. Since the user has previously interacted with the *Plus* button it is assumed that he wants to complete his operation, so the use of a contrasting color calls for immediacy to conclude the action.

## Preferences
Each feature present in the settings panel is built based on an image that holds the main aspect of the feature itself. For example, the *Delete all data* mode is flanked by a trash can icon that refers to the concept of elimination, the *i* of *Show Tutorial* reports to the information of the info point where to obtain details on the use of the application.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116418059-15ab8b00-a83c-11eb-89f3-ea343af32d9f.png">
</p>

The *Confidence Level* function is placed as the first element of the list being representative for the modification of the application behavior. Through these functions the user has control over data processing for object recognition. Through the use of the Gestalt laws we return to the use of the law of closeness, similarity, closure and others. In particular:

- Law of proximity: similar settings are brought closer together to be highlighted as a single unit. For example *Clear Cache* and *Delete all data* both express similar actions that go to delete data.
- Law of similarity: elements that refer to another page such as *Confidence Level* and *About* are described with a specific color and an identification symbol that refers to the concept of continuity of functionality. Instead, the other features are that identify actions, as described by Apple's HIG for iOS, which refer to pop-up gods.
- Law of closure: Each pair of elements are closed by a horizontal line that covers the entire horizontal space of the screen. This makes it possible to strengthen the concept of the unity of specific pairs of features. Inside them, however, the horizontal line starts from the beginning of the wording of the functionality to mark the diversification of the actions that can be performed.
- Law of good form: elements are described by regular, simple and clean geometric shapes.

One can fall into the mistake of considering it inappropriate to have two features such as *Clear Cache* and *Delete all data* close together. This could lead to user errors in running one feature instead of another. This possible possibility is abolished by the use of confirmation requests and the use of harmless inputs by marking dangerous actions with colors.  

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116418495-7aff7c00-a83c-11eb-94b5-233ddb5838c2.png">
</p>

The use of switches brings back to past experiences on the part of the user who can understand without problems whether it is enabled or disabled. The change of state of the switches is shown through animation and an appropriate coloring (gray/green).  
Next to the switches, information buttons have been inserted to allow the novice and/or general user to correctly use the *Analytics* and the *Tutorial*. In particular, the latter defines, as already expressed in the main documentation, an excellent aid to the user to fully understand the functionality of the application.

## Confidence Level
Section structured in such a way as to make the user understand in a completely immediate way which option is active. The confidence level allows you to select the degree of reliability in the recognition of objects by the algorithm.  
These options were introduced about the **Personas** identified during the analysis of the user base to which the project idea is intended. Greater diversification of the potential of the recognition algorithm outlines greater choices by the corresponding users. For example, one user may choose to have only the most accurate results, while others may have many more but less relevant results.  
The selection of the type of confidence used by the application is shown by using the check box that allows you to indicate the correct selection of the function. Furthermore, depending on the option selected, the relevant text below is updated providing an accurate explanation.

## About
It contains sets of information about the application and is structured to keep the system in the same state even if the functions refer to external views. For example, by clicking on the name of one of the two developers, the screen that refers to the developer's page is opened in the application itself. This practice allows for greater immersion on the part of the user without losing the bond established with the application when opening another application that overshadows the main application.  
In case the user has an installed application that has registered the URL scheme, which identifies the service, the latter will be opened. For example, if the user has the *GitHub* application and performs an action on one of the two developer buttons, the *GitHub* application will be opened. This choice is agreed according to the rules expressed by Apple.

# Usability test
As specified in General development part of the initial training tests to evaluate the design idea and the constructive path of the application were carried out through platforms such as Teams with the appropriate sharing.  
For tests formative information below is a set of information considered relevant and which led to the final development of the application.

## Training tests
### Tutorial

Part of the tests was carried out on subjects who, through the Mapping of subjects had already been routed to the idea of ​​an object recognition app.  
It was therefore decided to broaden the target of users by inserting subjects made totally unaware of the project idea. The tests of the prototypes led some of the users to understand only partially the purpose of the application, that is, the idea of recognizing objects was understood but not that of being able to search for images quickly and quickly. Also some have found it difficult to justify the section for editing the shot image.  
These issues have led to the construction of a tutorial that contains the idea and use of the application in four pages. Each page holds an easily recognizable logo, which tries to provoke the law of past experience, a title and a brief description. The tutorial is only offered to the user when the application is first opened in order to provide all the necessary information. All subsequent openings return to the main screen.

### Colors
Although these were the first prototypes, test users found the screens to be completely bare and lacking in vitality. It was therefore decided to structure the prototype and the application based on adaptable background based on the type of theme (light/dark) active on the device. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116422426-075f6e00-a840-11eb-9d2c-42a5f95e0847.png">
</p>

- Orange: color that describes inner harmony. This color manages to bring a sense of contentment and relaxation to the user.
- Celeste: mainly symbolizes the sense of research related to creativity through communication.

The fusion of the two colors, as shown in the image, tries to lead the user to a place of order and balance where the main focus is that of research, study and analysis.  
The aim is therefore to create an environment that is quiet and at the same time leads the user to use the application.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116422416-04fd1400-a840-11eb-83d7-846793a0922c.png">
</p>

- Red: expresses vital energy, both mental and physical.
- Blue: describes calm, tranquility and balance.

In this case we have tried to use two colors which in their meaning are contrasting with each other. The *"evening"* is seen as part of the day when the human being tends to devote more time to himself and his passions, so two contrasting colors were chosen to bring the user's sense of energy and at the same time that of total tranquility.

### Icon

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116422759-5b6a5280-a840-11eb-8d7f-d84e368a650f.png">
</p>

Various problems emerged to conceive an icon that could represent the idea of the application using elements and shapes already known to users and to enclose them in a tiny space.  
It was therefore decided to start with the basic concept of the image, in expressing a notion of having to do with something that exploits an image. The classic icon representing the image is seen as a series of mountains and a circle representing the sun. In this case the sun takes the place of the widely known research icon.   
The principle is to have users create an association on the basis of these representations, that is to express the concept of searching for an image, to operate with an image and high.  

Obviously, there is no lack of reference to object recognition. It was not included in the icon as it would have resulted in an overhead and indefinite jumble of information that would only lead to confusion. Object recognition is entrusted to the name of the application: **Vision**.

## Summative tests
For the usability tests, the same tools were used plus face-to-face meetings with other users, handing them the devices containing the installed application.
The latter were built as summative tests to systematically evaluate the characteristics of the system in the hands of end users. Below is the complete management of the test based on the final prototype.

## Test management
### Planning
A scenario test was used for planning to avoid implicitly suggesting to users the actions to be performed through a task test. In this way we tried to bring the user to a real context without being forced to follow defined tasks.  
The nature of the test is to evaluate the full comprehensibility of use of the application for release to the public.

### Test Preparation
The scenario test includes:  
You are on holiday abroad with your friend in front of a beautiful landscape. In the distance you notice animals that look like otters while for your friend they are martens. You decide to bet and who is right offers dinner.  
In the evening, walk along a street full of stalls where you can taste local dishes, to help foreigners each counter has exhibited a photo of the dish it offers. Do you remember that you already have photos of the dishes saved in your phone and together with your friend you decide to eat a dish containing mushrooms. \\
At the end of the evening you receive a message from your parents who ask you if you can send them all the images of the pizzas eaten during the holiday and of the dish just eaten.  

It is emphasized that:  
The landscape image was shown via a monitor.  
The phone has six random images in the gallery, two of which are dishes that contain mushrooms.  
The phone has three pictures of pizzas in the gallery.  
In addition to the images for the test, one hundred and fifteen random images were inserted.  
All images (excluding the five random plates) are totally randomly sorted. This is because it was decided to make the photos of the dishes immediately available to be analyzed, while those containing the pizza were searched using the search function.  

The scenario test encompasses the following tasks:
- [Task 1]: Take a photo of the landscape.
- [Task 2]: Analyze the photo just taken, possibly modifying it and selecting the animals with precision.
- [Task 3]: Access the photographic library through the application and analyze the photos of the dishes to obtain those with mushrooms.
- [Task 4]: Search for the word pizza with the search method in the photo gallery.
- [Task 5]: Save one of the two photos of the dish containing the mushrooms via the application to share it with parents via the search function.

### Execution of the test
The test was carried out on twenty subjects, fifteen reflecting the users defined in Personas, while the rest were evaluated as a possible extension of the target of users and unaware of the use of the product.  
The test took place in an environment controlled by a facilitator and an observer (played by both project members in turn) and took place on a user-by-user basis.

## Evaluation report
### Summary
The document reports the analysis on the feasibility of the proposed idea and on the effective usability and application.  
The conclusions led on the one hand to an appreciation and interest in the idea and a completely acceptable success rate on the use of the application.
### Evaluated product
The product evaluated in the summative test involves the use of the final product to be released and distributed on a large scale. All features have been described in Feature Analysis.
### Objectives of the evaluation
The objectives pursued are:
- Functionality: offer all the functionalities to the customer on the basis of the conceived idea.
- Usability: Making the user experience simple as possible.
- Reliability: performance level adaptable to older devices and fluidity in carrying out operations.
- Efficiency: optimal management of space and time. As already discussed in All in one we preferred to balance towards more space but less time.
- Portability: in terms of application this can also be made portable to platforms such as iPad, AppleTv, AppleWatch and possibly other devices, but it always remains linked to the Apple environment.

### Methodology used
Number of users who participated in the final product test: 20.   
Number of users who participated in testing phases for product modeling: 8.  

### User experience level
Users were divided into:
- Inexperienced: users totally inexperienced in the use of new technologies or applications.
- General: intermediate users able to understand the operation of an application without too many pretensions.
- Experts: users able to quickly assimilate the correct use of an application and/or technology.

<p align="center">
  <img src="https://user-images.githubusercontent.com/22590804/116423910-6376c200-a841-11eb-8f4e-5d8877229f71.png">
</p>
