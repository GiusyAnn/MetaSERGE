# SERGE 2.0: A digitalization of the Serious Game For the Education of Risk Management 
<h3 align = "center"> </h3>
<p align = "center"> An open-source project developed with Unity3D and Photon Unity Networking to reenact the serious game SERGE in a tridimensional virtual environment for academic and educational purposes. </p>
<p align = "center"> This project is based on the Serious Game SERGE descibed in the paper (https://dl.acm.org/doi/abs/10.1145/3639474.3640085).</p>
<p align = "center">
  <!-- <img src = "blobs/presentation_pic.jpg?raw=true" width = "800" heigth = "600"> -->
</p>


## Application Description
The main goal of this project was to develop and validate a digital recreation of the serious game **SERGE**: a serious game specifically developed to support academics and students in learning risk management.
The platform is a conference room where it's possible to interact with other players, objects and play SERGE. It is based on a previous project named **The Metaverse Classroom** by **Viviana Pentangelo** - [vipenti](https://github.com/vipenti) at University of Salerno.

<div align="center">
  <img src="blobs/stripe1.JPG" width="150"/>
  <img src="blobs/stripe3.png" width="195"/>
  <img src="blobs/stripe2.JPG" width="304"/>
  <br>
  <img src="blobs/stripe4.png" width="202"/>
  <img src="blobs/stripe5.png" width="202"/>
</div>


## Content of the Repository
This repository contains:
- _SERGE_: The complete Unity Project of the application subdivided into several archives.
- _Windows Build_: The built application ready to use for Windows.
- _MacOS Build.app_: The built application for MacOS.

## How to Install

### Application only
**Windows:**
1. Download the _Windows Build_ folder.
2. Run the _SERGE_ executable.

**MacOS:**
1. Download the _MacOS Build.app_ and extract it into a folder
2. Follow these steps to allow your device to run the application:
    - Open the terminal and navigate to the folder that contains the extracted files.
    - Type the following command <code>chmod -R +x MacOS Build.app/Contents/MacOS</code> into the terminal.
    - Type the following command <code>xattr -cr MacOS Build.app</code> into the terminal.
    - Double-click on _MacOS Build.app_.

### Unity Project

**Requirements:**
- Unity3D version: 2021.3.22f1
- Unity Hub

**Steps:**
1. Download the _SERGE_ folder.
2. Open the Unity Hub, go in the _Projects_ tab and click on the _Open_ button.
3. Choose the path to the new directory.
4. The project should now appear in your projects list. Click on its name and Unity will install all the needed libraries to make it work.

## Shoutouts
* **Pricey1600** for making the chairs - [Pricey1600](https://sketchfab.com/Pricey1600)
* **MozillaHub** for making the table and the conference room- [mozillareality](https://sketchfab.com/mozillareality)
* **goff.brian** for making the exclamation mark - [Brian Goff](https://www.vecteezy.com/members/goff-brian)
* **Neberkenezer** for making the buildings - [Neberkenezer](https://sketchfab.com/neberkenezer)
* **Froggreen** for making the sofas - [Froggreen](https://sketchfab.com/Froggreen)

## Tutorial 
* https://drive.google.com/file/d/1L5YOSa9zhIIMmlJmR_DxB9OjYUGis-Po/view?usp=share_link

## Dependencies

All dependencies are already included in the Unity project, so no additional installation is needed:
- Unity3D 2021.3.22f1
- Photon Unity Networking (PUN) 2, v2.41, and Photon Voice (in `Assets/Photon`)
- Standard Unity packages (Input System 1.5.1, TextMeshPro 3.0.6, UGUI), installed automatically by Unity Hub when opening the project

If needed, PUN can be re-imported via _Window > Package Manager > Install from name_.

## Photon Setup

Networking and synchronization between players are handled by the Photon cloud service, so an internet connection is required. To run the project with your own Photon account:
1. Create a free account on [photonengine.com](https://www.photonengine.com) and create a _PUN_ application and a _Voice_ application.
2. In Unity, open `Assets/Photon/PhotonUnityNetworking/Resources/PhotonServerSettings` and paste the App IDs in the _App Id Realtime_ and _App Id Voice_ fields.
3. The default region is `eu`; it can be changed in the same file.

Rooms are created with a maximum of 12 players; the evaluation sessions used two players per room.

## Hardware Requirements

MetaSERGE has no specific hardware requirements: a standard desktop or laptop computer running Windows, macOS, or Linux with an internet connection is sufficient. The evaluation sessions were run on university lab machines and personal computers in desktop mode (no VR headset).

