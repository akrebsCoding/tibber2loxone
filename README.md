# tibber2loxone
Tibber2Loxone integrates the Tibber API using GraphQL to retrieve real-time data. The fetched information is locally hosted on a Raspberry Pi through a Flask server and seamlessly integrated into Loxone, providing the data for further utilization within Loxone's environment.

If you wish to create your own queries, Tibber provides its own API/GraphQL Explorer.

Visit: https://developer.tibber.com/explorer

Here, you can load your own token or a demo token.

You'll need the following:
  - A Tibber Token
  - A host where you'll run the script
  - Loxone Config

App Installation:
  - Log in at https://developer.tibber.com/ to obtain an Access Token
  - Load the Tibber folder onto the host
  - Execute app.py

When accessing the host on Port 9945, the current electricity price should be displayed.

![price](https://github.com/akrebsCoding/tibber2loxone/assets/77326088/0525732c-b2f3-44bc-950c-5e769316f52c)


Installation Loxone:

![Lox_HTTP](https://github.com/akrebsCoding/tibber2loxone/assets/77326088/0f33a326-5d87-4b79-b9e4-3cc16c6965e2)

  - Create a virtual HTTP input and enter the corresponding data
    
![Lox_E_opt](https://github.com/akrebsCoding/tibber2loxone/assets/77326088/976d7b32-612f-4b5c-ac20-5e02e36d3a16)

  - Assign a command to the HTTP input and enter the relevant data
    
![Lox_B_opt](https://github.com/akrebsCoding/tibber2loxone/assets/77326088/9de8a048-e7c0-486f-b98e-ce0219dc6b0e)

  - Your directory should now contain the following entries
    
![Lox_Baum1](https://github.com/akrebsCoding/tibber2loxone/assets/77326088/450f130b-d645-44da-b524-0ac46f921edb)


I have several RGBW LED strips in my house that display the current electricity price in color. For example, my LEDs light up green when the current electricity price is below 19 cents.

![20240102_092406](https://github.com/akrebsCoding/tibber2loxone/assets/77326088/8f8562f1-bced-485e-b80b-5638925f31ac)


The logic behind this is as follows:
![Programm](https://github.com/akrebsCoding/tibber2loxone/assets/77326088/6f4d9847-b14c-4613-9ea4-20ea94fe9335)


And here's how it looks in the Loxone App

![Screenshot_20240102_092730_Loxone](https://github.com/akrebsCoding/tibber2loxone/assets/77326088/3e6288ee-55f9-4232-93c2-e5673f8808d1)


