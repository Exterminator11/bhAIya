# bhAIya

*bhAIya* is a one of a kind AI powered application designed to bridge the gap between consumers the companies that make their products.

In India, shopkeepers are often refered colloquially as Bhaiya, meaning brother or guide. Assisting customers finding the products they need for the best price. We aim for our application to help both companies and customers alike.

In many cases there are many shopkeepers that are unable to attend to the needs of the customer because of their inability to understand the broad range of products in their inventory.

With BhAIya we have made use of AI technology to design a powerful recommendation system that can pander to your every need.

Based on customer needs and budget, users can search for the product of their choice via description or image.

This accessibility feature allows for users to simple take a picture of a product in the store and immediately learn every detail about the product including past reccomendations, price details, product specs and much more.

Our aim is to help bridge the gap between customers and companies by allowing users to learn more about the products they use and make informed decisions. 

# Demo

https://github.com/Exterminator11/bhAIya/assets/88940647/6e40777d-aa1e-40b6-98fe-f1344b49a29a

# Details
1. Main.py - This is the driver code that is responsible for the UI that the customer sees
2. backend/database.csv - A sample product database that is used as a benchmark for creating a sample database
3. backend/ImageBackend - Contains 100 product images that are used for the few shot learning of the LLM
4. backend/database.json - The final dynamic database constructed by bhAIya that contains all the information about the products the shopkeeper has
5. backend/imageDatabase.json - The final image database
6. backend/app.py - The FastAPI server that takes care of all the computation.
