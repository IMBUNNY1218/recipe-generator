
# Smart Recipe Generator
This is a web application that suggests recipes to users based on the ingredients they have on hand. Users can input ingredients via text or by uploading an image. The application features filtering, dietary preferences, recipe ratings, and personalized suggestions.   
**Note:** Other than the given requirements as per the document the additional feature is added which allows the user to see the items that are missing in order to make a partiuclar recipe.

## Features
Ingredient Input: Users can enter a comma-separated list of ingredients.

Image Recognition: Upload an image of your ingredients, and the app will use the Gemini API to identify them.

Recipe Matching: A matching algorithm finds the best recipes from the database based on your available ingredients.

Filtering & Sorting: Filter recipes by difficulty and cooking time, and sort the results.

Dietary Preferences: Select options like Vegetarian, Healthy, Gluten-Free, and Dairy-Free.

Recipe Details: View detailed recipe information, including ingredients, instructions, and nutritional facts in a modal view.

Favorites & Ratings: Logged-in (anonymously) users can save their favorite recipes and rate them.

Missing Ingredients: Also provides the missing ingredients to make a particular dish.

Personalized Suggestions: The app suggests new recipes based on your saved favorites and highly-rated recipes.

Responsive Design: The application is fully responsive and works on mobile, tablet, and desktop devices.

User Authentication: Utilizes Firebase anonymous authentication to store user-specific data like favorites and ratings.

Technical Stack
Frontend: HTML, Tailwind CSS, JavaScript

AI/ML: Google Gemini API for image-based ingredient recognition.

Backend/Database: Google Firestore for storing user favorites and ratings.

Hosting: The application is deployed on GitHub Pages.

Getting Started
To run this project locally, you need to configure your Firebase credentials.

Prerequisites
A modern web browser.

A Firebase project.

Setup
Clone the repository:

git clone [https://github.com/your-username/smart-recipe-generator.git](https://github.com/your-username/smart-recipe-generator.git)
cd smart-recipe-generator

Firebase Configuration:

Create a new project on the Firebase Console.

In your project, go to Project settings > General.

Under "Your apps", click the web icon (</>) to add a new web app.

Copy the firebaseConfig object.

In index.html, replace the placeholder firebaseConfig object with your actual Firebase project configuration.

Enable Anonymous authentication in your Firebase project: Go to Authentication > Sign-in method and enable the "Anonymous" provider.

Set up Firestore: Go to Firestore Database, create a database, and start in test mode for initial development (or set up security rules appropriately).

Gemini API Key:

This project is set up to use an empty API key, assuming it will be run in an environment where the key is injected automatically (like Google AI Studio or a similar platform).

If you are running this on your own, you will need to obtain a Gemini API key from Google AI Studio and replace the empty API_KEY constant in the JavaScript code.

Open index.html:

Open the index.html file in your web browser to start using the application.

Project Structure
index.html: The main and only file for the application. It contains the HTML structure, Tailwind CSS for styling (via CDN), and all the JavaScript logic for the application's functionality.

README.md: This file, providing information about the project.

write-up.md: A brief document explaining the technical approach.

This project is self-contained in a single HTML file for simplicity, as per the project requirements.
