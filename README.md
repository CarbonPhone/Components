
# Carbon Components

A guide for creating components.     
Are you searching for guides to install a component? This guide is hosted in the reposistory [[CarbonPhone/InstallComponent](https://github.com/CarbonPhone/InstallComponent)]

---


## Component types & Connections

### Basic
The basic component uses 5 different PIN types

| PIN Name | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `data_in` | `input/data` | The PIN for sending data from the Component to the Core |
|`data_out` | `output/data` | The PIN for recieving data from the Core
| `passport` | `input/data` | The PIN for identifying your component
|`Power0`| `power/-` | The PIN which is connected to the GND of the Core
|`Power1`| `power/+` | The PIN connected to the VIN of the Core
### Battery

Each Core contains 4 Battery PINs. No matter the size or shape of the battery it needs to be designed for these PINs.

No other component may be placed in these PINs.


![Please wait for the image to load...](https://github-production-user-asset-6210df.s3.amazonaws.com/151966278/617067758-2a1c614e-da4a-4a8d-a333-6028227e2ce6.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20260704%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20260704T071114Z&X-Amz-Expires=300&X-Amz-Signature=9a249f2c65f0a550a842b2b11ddbcfb54530b3385ca3199810d222e072d43a78&X-Amz-SignedHeaders=host&response-content-type=image%2Fpng)

The PINs are explained here:
| PIN Location|Pin name|Pin description| 
|:-------------------|:-------------------|:------ |
|⏺️🟦<br>🟦🟦|  Power/IN|Charging port -> Battery|
|🟦⏺️<br>🟦🟦| Power/OUT| Battery -> Phone |
|🟦🟦<br>⏺️🟦| Power/INN| GND from the Battery  -> Charging port | 
|🟦🟦<br>🟦⏺️| Power/OUTN| GND from the Battery -> Phone|


### Display 
The display is a component which is put on the front side of the phone. It is commonly already placed on the phone since production and the user doesn't have to place it. The display being a component is only used for upgrading and replacement purposes.
There is no guide to how the display component is pinned-out or how to create drivers for it, but there is an instalation and replacement guide on [this reposistory](https://github.com/CarbonPhone/DisplayReplacement).


## Drivers

For every component you need to create software drivers so the OS can support them.

Check out the [drivers reposistory](https://github.com/CarbonPhone/Drivers) for tutorials, guides and templates!

It's easy, we promise :)
## Badges
Creating a component requires a GitHub reposistory with the component's code and schematic.

Please add these badges to your reposistory if you may need them:

### If you would like to have your component published to the Carbon store add this badge

![Carbon Components Store](https://img.shields.io/badge/Carbon%20Components%20Store-Awaiting%20approval-yellow?style=plastic)
(Do not change any parts of the badge)

and 

![Contact email](https://img.shields.io/badge/Contact%20email-%5Bplease%20add%20your%20email%20here%5D-yellowgreen?style=plastic&logo=gmail)
(Add your email for ways we could contact you. Note that since your reposistory is public you may recieve some emails from people who are not associated with Carbon. You may remove this badge after your component is approved for the Carbon store)


When your component gets approved you will recieve an email from noreply.carbon@wanets.me with the URL of your Carbon Store component listing and your new badge similar to:

![Carbon Component Store](https://img.shields.io/badge/Carbon%20Component%20Store-Install-green?style=flat-square)

linking to your listing

>[!NOTE]
>
>We recommend checking out this reposistory's wiki tab for guides, tutorials and examples as well as quick starts for making a component, If you have any problems or questions feel free to ask us things in the Issues tab with the tag [Q&A]

