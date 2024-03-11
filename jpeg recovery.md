                                                Jpeg recovery/photo shop

The user will be able to upload the contents of a deleted sim card.
The app would interate over the components of that file.
While iterating the app would look at the data in hexadecimal form.

    If it finds the hex code 0xFF, 0xD8 it will begin storing the data in iterates over into a new file until
    it encounters the sequence 0xFF, 0xD9 at which point it would store a new file as a jpeg in the public folder.


Stretch goals  
    Modifications to photos such as black and white, sepia tone, squished, blurry etc.


    framework:PyImagine

        download

            pip install pyimagine

        imports

            from pyimagine import Arta
            from pyimagine.constants import Style

        example of usage

            # Initialize Imagine
            arta = Arta()
            arta.signupNewUser()

            # Generate from inspiration
            inspired_image = arta.infer(prompt="Create something amazing!", style=Style.REALISTIC_2)

            # Prompt from image
            original_image = open('image.jpg', 'rb').read()
            prompt_image = arta.image2text(original_image, language_code='en')

           










Sources