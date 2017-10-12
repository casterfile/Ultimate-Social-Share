# UUnity3d ultimate social share plugin for Android and iOS
Developer: Anthony A. Castor

This Source does not give any warranty please use at your own risk </br>

This plugin is for sharing screenshot in social media. </br>

This application is free of virus or malware </br>

<h3>Software Requirment </h3>
Unity 5.6<br/>
Unity C#<br/>

<h3>Online Portfolio</h3>
Distribution itch(Web and Desktop): https://goo.gl/Wq1nuD </br>
Distribution Google Play: https://goo.gl/uKIIr4 </br>
Distribution Itunes AppStore: https://goo.gl/54yJPi </br>
Distribution Amazon Store: https://goo.gl/RUp1Od </br>
Distribution Windows Store: https://goo.gl/rCxsH6   (No Direct link to Dev Page) </br>
Distribution WearVR: https://goo.gl/y0X1nR  (No Direct link to Dev Page) </br>

<h3>More Information and Demo Videos </h3>
Facebook: https://goo.gl/vvDSIL </br>
Linkedin: https://goo.gl/c9Fh6n </br>
YouTube: https://goo.gl/BFZ7C5 </br>
StackOverFlow: https://goo.gl/J1hFqL </br>
Github: https://goo.gl/jPHFPe </br>


<h3>1. Description</h3>
This plugin allows you to use the native sharing window of your mobile device.</br>
•	Works on Unity3d 5.0+</br>
•	Works on Android, version 2.3.3 and higher (probably 2.2 as well).</br>
•	Works on iOS6 and up.</br>


<h3>2. Screenshots</h3>
iOS 7 (iPhone)</br>

![alt text](screenshots/1.png "Scene1")

Sharing options are based on what has been setup in the device settings</br>

Android</br>

![alt text](screenshots/1.png "Scene2")

Sharing options are based on what has been setup in the device settings</br>

<h3>3. Usage on iOS and Android</h3>
using UnityEngine;
using System.Collections;

namespace jtac.SocialSharing
{
    public class Example : MonoBehaviour
    {
        [SerializeField]
        private SocialSharing socialSharing;
        [SerializeField]
        private string text;
        [SerializeField]
        private Texture2D texture2D;

        public void Click()
        {
            //Share text+screenshot
            socialSharing.ShareScreenshot(text);

            //Share text+texture2D
            socialSharing.ShareTexture2D(text, texture2D);
        }
    }
}


