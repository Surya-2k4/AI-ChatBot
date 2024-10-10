# AI-ChatBot

Gemini API key i have used in this project : AIzaSyCJFuAoKhUSle7hxyr8S6ah6wDEWxg9kg4


Download your API Key : https://aistudio.google.com/app/apikey

*1. Create or open a Flutter project*

*2. Add dependencies*
Open pubspec.yaml file from your flutter project and under depencencies section add below dependencies

dependencies:
  google_generative_ai:  
  intl:

_google generative ai: used to communicate with gemini AI._
_intl: used for DataTime Formating._


*Basic Information on how to use google generative ai package (code explanation)*

This is Snippet Code- Not Complete Code- Find Complete code below with UI design Chat App

final model = GenerativeModel(model: 'gemini-pro', apiKey: apiKey);
final content = [Content.text(message)];
final response = await model.generateContent(content);

This above snippet code initializes a GenerativeModel object with the specified model (‘gemini-pro’) and API key. Then, it prepares the content to be sent to the AI model (Basically a Text/prompt message), which consists of a list containing a single text content (message). Finally, it sends this content to the Gemini AI model and awaits the response, which will contain the AI-generated content based on the input message user provide.
