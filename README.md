# TestLambdaCICD

## Video tutorial
https://www.youtube.com/watch?v=ekNhTHtIT1k

## Console

AWS CLI

Python
Dans cet exercice, vous appelez l'SynthesizeSpeechopération en transmettant du texte saisi. Vous pouvez enregistrer le son qui en résulte dans un fichier et vérifier son contenu.

Exécutez la synthesize-speech AWS CLI commande pour synthétiser un échantillon de texte dans un fichier audio (hello.mp3).

L' AWS CLI exemple suivant est formaté pour Unix, Linux et macOS. Pour Windows, remplacez le caractère de continuation Unix (\) à la fin de chaque ligne par un curseur (^) et utilisez des guillemets complets («) autour du texte saisi par des guillemets simples (') pour les balises intérieures.




Dans l'appel àsynthesize-speech, vous fournissez un exemple de texte à synthétiser par une voix de votre choix. Vous devez fournir un identifiant vocal (expliqué dans l'étape suivante) et un format de sortie. La commande enregistre l'audio qui en résulte dans le fichier hello.mp3. Outre le MP3 fichier, l'opération envoie la sortie suivante à la console.

aws polly synthesize-speech \
    --output-format mp3 \
    --voice-id Mathieu \
    --text 'Bonjour, mon nom est Aboubacar Diallo. je suis informaticien de profession. Vous avez 100000 francs guineens dans votre compte' \
    hello.mp3

{
        "ContentType": "audio/mpeg", 
        "RequestCharacters": "71"
}
