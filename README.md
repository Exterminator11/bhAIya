# bhAIya

## Inspiration

In the bustling streets of India, shopkeepers, affectionately called "Bhaiya," play a crucial role. They help customers find the products they need at the best prices. However, many shopkeepers struggle to meet customer needs due to the vast range of products they handle. Observing this challenge, we thought: what if technology could help? What if we could create an application that acts like a knowledgeable Bhaiya, bridging the gap between customers and products?

## What It Does

**bhAIya** is a unique AI-powered application designed to bridge the gap between consumers and the companies that make their products. Here's how it works:

### Key Features of bhAIya

1. **Product Recommendations**:
   - **AI-Powered Suggestions**: bhAIya uses advanced AI technology to provide personalized product recommendations based on customer needs and preferences.
   - **Smart Search**: Users can search for products by description or image, ensuring they find exactly what they’re looking for.

2. **Image Recognition**:
   - **Snap and Learn**: Customers can take a picture of any product in a store and instantly receive detailed information, including product specs, price details, and past recommendations.

3. **User-Friendly Interface**:
   - **Easy Navigation**: The app is designed to be intuitive and easy to use, making it accessible to a wide range of users, from tech-savvy individuals to those less familiar with technology.

4. **Enhanced Shopping Experience**:
   - **Informed Decisions**: By providing comprehensive product details, bhAIya helps users make well-informed purchasing decisions.

## How We Built It

**bhAIya** is written in Python and powered by the Mistral 7B Instruct model, along with assistance from the Llava Vision model. bhAIya takes the shopkeeper's database as input and adapts to the products listed in the shop. It creates a specialized database for each store using insights from the large language model and uses it to fulfill users' queries. It uses **Few Shot learning** to identify categories from the user's prompt and match it with the already generated categories in the database. These categories on both sides are converted into vector embeddings using Word2Vec and are matched together using Cosine similarity. The top n results are returned back.
 
## Challenges We Ran Into

The main challenge we faced was getting the large language model to perform as intended. After a few sleepless nights, lots of coffee, and sheer determination, we finally discovered the correct mixture of parameters for the prompt, enabling bhAIya to understand any database.

## Accomplishments We're Proud Of

We're proud of providing an immersive and spatial experience to customers, bringing the joy of shopping to everyone. We're also proud of the shopkeepers who benefit from this, now able to convey the purpose of their products more clearly and effectively.

# Demo

https://github.com/Exterminator11/bhAIya/assets/88940647/6e40777d-aa1e-40b6-98fe-f1344b49a29a

# Details
1. main.py - This is the driver code that is responsible for the UI that the customer sees
2. backend/database.csv - A sample product database that is used as a benchmark for creating a sample database
3. backend/ImageBackend - Contains 100 product images that are used for the few shot learning of the LLM
4. backend/database.json - The final dynamic database constructed by bhAIya that contains all the information about the products the shopkeeper has
5. backend/imageDatabase.json - The final image database
6. backend/app.py - The FastAPI server that takes care of all the computation.
