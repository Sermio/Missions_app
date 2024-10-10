# Missions_app (Done with Flutter)

<strong>DISCLAIMER: </strong>Due to a Non-Disclosure Agreement (NDA) I have signed, I am unable to display or share the application code. Thank you for your understanding.


This application consists of monitoring points of sale in different locations. The information that can be obtained is varied, such as the existence of products, prices, store organization, etc.

In this project, I have focused on collecting information (price and name) of a product from an image sent by a user. This image is processed using deep learning algorithms and optical character recognition techniques to detect the product and the corresponding label.

The application is designed for registered users to capture information. A rewards system based on campaigns and missions has been created to reward these users with points for completing each action. These points can be redeemed in the future for discounts and rewards.

The mobile application will be used by users to see which campaigns are active at that moment and to select the ones they wish to complete. Once users have selected which campaigns they will undertake, they can view a map of the nearest stores where they can complete those missions. Depending on the types of missions they need to perform (text or image submission), they can either write a brief response or take a photo of the requested product.

These images are sent to a server where they are processed to extract the data. Once the data submission is complete, the user receives the assigned reward points for their contribution. In case the user is unfamiliar with the city, there is a GPS guide system to help them reach their desired store.

This video shows the general operation of the application: https://drive.google.com/file/d/1NFuND69SWkAiwly5QDcx4ZbPc49uWKpH/view?usp=sharing


First, all users must register in the application using the screen shown in Figure 1.1 on the left. The user must fill in all the fields; if any field is left incomplete, a red indicator will be shown to the user in that field. Once the users completes their registration, they will be redirected to the login screen displayed in Figure 1.1 in the center. On this screen, the corresponding email and password used for registration must be entered. To access the application, it is necessary to check the terms of use checkbox; otherwise, a popup window will appear to inform the user of their error. Once the user has logged into the application, a list of all available campaigns for booking will be displayed (Figure 1.1 on the right) along with a navigation menu at the bottom of the screen. These campaigns are shown with a recency of up to two days. The user will be able to see which campaigns are expiring soon, as well as the title of the campaign and the points they will earn for completing it. If the user selects "Profile" in the navigation menu, their user profile will be displayed (Figure 1.2 on the left). The main objective of this screen is to show the current points the user has, but it also displays their name, profile picture, and allows navigation to the screen where they can edit their data. If the user selects "Edit Profile," they will be able to modify the fields shown in Figure 1.2 in the center, with the option to cancel these changes or update them.

<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/22fc2f8f-ee6d-4a26-9472-efa66c297013" alt="Registro 1" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/e072f372-294d-40d7-8aeb-415bb5cc207d" alt="Registro 2" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/3d481cc4-3d3f-4929-a58b-cf917fb51002" alt="Registro 3" width="200" hspace="30"/>
</div>
Figure 1.1: Registration, login, and available campaigns screens.


<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/8a6d3bcc-9649-4067-8333-2cb6fd2fb5f8" alt="Registro 1" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/90ef28bf-bc24-45eb-9b95-cdba685f0a2b" alt="Registro 2" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/ad79b648-7c5a-4cce-87e5-ea5d5bc77019" alt="Registro 3" width="200" hspace="30"/>
</div>
Figure 1.2: Profile, edit profile, and change password screens.

On the other hand, the modification of the password is also allowed (Figure 1.2 on the right). To update it, the current password, the new password, and confirmation of the new password must be entered. These changes are immediate, so if the user logs out, they will need to enter their new credentials.

If the user selects a campaign from the list of available campaigns shown in Figure 1.1 in the center, the missions contained in that campaign will be displayed (Figure 1.3 on the left). If the user wants to complete these missions, they must reserve them using the button at the top of the screen. Next, if we navigate to the "Map" tab via the navigation menu, we will have a map that shows the points of sale with active reserved campaigns at that moment (Figure 1.3 in the center). To display the markers, there is a slider at the top that allows us to modify the distance at which we will see points of sale (from 0 to 5 km). The markers have a unique icon corresponding to the chain they belong to. If we select them, a button will appear to view the reserved campaigns for that point of sale. On the next screen, we can see which reserved campaigns are available in that store (Figure 1.3 on the right). There is also a button that opens an instance of Google Maps to generate a route to the corresponding location, in case the user needs it.


<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/7587b337-f80b-459c-ba69-0cb729ff6354" alt="Registro 1" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/6575cee2-673e-4461-a826-a2b5617fbcb5" alt="Registro 2" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/be031d6a-391b-4b13-919e-eb34f46f6cf6" alt="Registro 3" width="200" hspace="30"/>
</div>
Figure 1.3: Campaign missions screens, map, and list of reserved campaigns.


<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/b374cf1b-7c37-4e07-ab0b-530a80298680" alt="Registro 1" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/a34a9141-625f-46ce-9405-9721256ed301" alt="Registro 2" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/07ae04c2-a8d2-4b23-9815-2baffec18719" alt="Registro 3" width="200" hspace="30"/>
</div>

Figure 1.4: Screens of the missions that can be completed, mission interface, and text submission of results.

After selecting a previously reserved campaign, a list of the missions that comprise it will be displayed (Figure 1.4 on the left). At this point, we have two options. First, if we select a mission that only requires text submission, a screen will appear indicating the mission and a text field for us to write our response (Figure 1.4 in the center). Next, the user can confirm and submit their data, which will take them back to the main screen along with a confirmation message for the data submission (Figure 1.4 on the right).

On the other hand, if we select a mission that requires image submission, the application will redirect us to another screen that shows a small guide on how to take the photographs (Figure 1.5 on the left). Next, the camera will open with a box located at the bottom center, so the user can position the price tag of the product there (Figure 1.5 on the right).

Once we have taken the corresponding photograph, the application will allow us to confirm or discard that image (Figure 1.6 on the left). Finally, once the user has completed all the missions of that campaign at that point of sale, the reward points obtained for their completion will be sent to them. These points will be reflected in the user's profile (Figure 1.6 on the right).

<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/d43e02d8-dcdd-457c-886d-749dfdb112c7" alt="Registro 1" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/c424da16-98ab-4476-b7ea-cf651459273b" alt="Registro 2" width="200" hspace="30"/>
</div>

Figure 1.5: Guide and camera screens.


<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/98e08478-adb7-4596-9984-10b87bcc4998" alt="Registro 1" width="200" hspace="30"/>
  <img src="https://github.com/user-attachments/assets/c9e24371-9dc2-4c3e-a783-d2e54e4d0dd8" alt="Registro 2" width="200" hspace="30"/>
</div>

Figure 1.6: Image confirmation and profile screens with obtained points.
