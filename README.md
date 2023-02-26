# PokeType

![](https://github.com/rabiaedayilmaz/PokeType/blob/main/src/assets/poke-main.jpg)

Have you ever wondered about what if you were a pokemon? Well, I did. However, to decide is even harder if you have so many options, like which type of element you are!
Well, machine learning got your back, so no need to worry.

The goal of this project is to predict the pokemon type for a given image. Therefore, each user will be able to load an image, such as her/his selfie etc., click on the predict button, and then discover your type.

![Example from the Interface](https://github.com/rabiaedayilmaz/PokeType/blob/main/src/assets/example.png)

## Usage

You can check it out immediately [here](https://poke-type-game.onrender.com/).

To use it locally, edit etc., firstly clone this repo.

```bash
git clone https://github.com/rabiaedayilmaz/PokeType
```

```src``` folder contains web application using HTML, CSS and JS.
```train``` folder contains machine learning model and dataset using TensorFlow framework and Python. 
After training the model, convert it into ```tensorflow-js``` format to use it in JS.
To convert it, use following structure on the Google Colab, then download the model. Later add model into corresponding file:

```bash
pip install tensorflowjs
tensorflowjs_converter --input_format keras \
                        /content/PokemonTrainerLastBestModel.h5 \
                       /content/
```

For webpage interface, there are some commands to download packages etc. 
```bash
npm install express
npm install jquery
npm install nodemon
```

Then, to activate the project on your local server, use these commands respectively:

```bash
npm init
node src/index.js
```
Now, you are all set up.
You will be able to see and test on ```http://localhost:8080```


Special thanks to Emir Öncü for designing the PokeType logo for me, you rock!
