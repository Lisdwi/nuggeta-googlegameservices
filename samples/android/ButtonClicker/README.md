<img src="http://www.nuggeta.com/images/nuggeta.png"/>

<h2>Contents</h2>

<b>ButtonClicker.ngdl</b> : Nuggeta Integration inside the sample real-time game ButtonClicker provided with Google Game Services.

<h2>Prerequisite</h2>

To integrate Nuggeta inside ButtonClicker you need first to complete the following steps
 
1. Build and Run the official ButtonClicker sample available here : https://github.com/playgameservices/android-samples

2. Create a Developer Account on Nuggeta : http://developer.nuggeta.com

3. Read about getting started with Google Game Services and Nuggeta : http://developer.nuggeta.com/#!documentation/client-setup/google-game-services



<h2>About the sample </h2>
The sample ButtonClicker demonstrates how to send and received real-time messages via Google Game Services.
If you have a look at the MainActivity class, you can notice that you have to deal with bytes arrays to exchange data:
In fact, in this sample there is three type of messages :

- a start message : represented by  bytes[0] = 'S'
- a score message : represented by  bytes[0] = 'U' and  bytes[1] = score
- a final score message : represented by  bytes[0] = 'F' and  bytes[1] = score

We can understand it for a simple sample like ButtonClicker, but in real games it may become really complicated... 

With Nuggeta you won't have do deal with bytes, we do the painful job for you ... and more.
Instead you have to deal with your data objects that you have defined in the Nuggeta Developer Site and download it in your API.
Yes you have the power to create your own gaming API with Nuggeta.

<h2>How to run the sample with Nuggeta?</h2>

1. Download a zip of this repo.

2. Replace the file MainActivity.java of the  ButtonClicker project by this one.
	Replace the package name by yours.
	You will have compilation errors in the project. This is normal, now you have to download your Nuggeta API.

3. Download your Nuggeta API of ButtonClicker
	
- Log into Nuggeta Developer Site http://developer.nuggeta.com
	
- Click on the Create Game button and choose import NGDL

- Select the file ButtonClicker.ngdl (in the folder ngdl of the sample) and create the game.

- View the model definiton :

- Click on Download API , and choose Google Game Services

- Save the API in the folder lib of your project ButtonClicker

- Now your project should compile.

- Have a look at the file MainActivity.java to see how Nuggeta simplifies your life ;)
	
	
<h2>Next Steps </h2>

Now your are ready to make complex games with Google Game Services and the Nuggeta Model Definition.

Create your game from the DeveloperSite then define your Game Model API, download your API and enjoy.
	
	
The Nuggeta Team
	
	







