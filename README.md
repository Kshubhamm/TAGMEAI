<p align="center">
  <a href="https://github.com/kshubhamm/TAGMEAI/">
    <img src="https://github.com/kshubhamm/TAGMEAI/blob/main/tagme.jpg" alt="Tagonizer" width="150" height="150"> 
  </a>
</p>

<p align="center">
  <a href="https://github.com/kshubhamm/TAGMEAI/">
   <img src="https://madewithlove.now.sh/in?heart=true&colorA=%23ff0000&colorB=%23050505&template=plastic" alt="Made with love">
    <img alt="GitHub" src="https://img.shields.io/github/license/merrcury/tagonizer?style=plastic">
    <img src="https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20by%20-TEAM JUST DO IT%20KK-red&template=plastic">
  </a>
</p>

<p align="center">
  <a href="https://github.com/kshubhamm/TAGMEAI/">
    <img src ="https://img.shields.io/github/issues-raw/merrcury/Tagonizer" alt = "Open Issues">
    <img src ="https://img.shields.io/github/issues-closed-raw/merrcury/Tagonizer" alt = "Closed Issues">
    <img src ="https://img.shields.io/github/issues-pr-raw/merrcury/Tagonizer" alt = "Open Pull Requests">
    <img src ="https://img.shields.io/github/issues-pr-closed/merrcury/Tagonizer" alt = "Closed Pull Requests">
  </a>
 </p>
    

## Problem Statement 
Customers write product reviews on ecommerce websites like Amazon, Flipkart and others. Amazon processes the reviews to generate commonly occurring tags. But, there exist multiple tags referring to the same thing. The Auto-generated Tags from customer Reviews are pointless and repeating like battery, battery life, battery performance etc. Reviews are not well classified as positive or negative, and same goes with tags/comments

## Solution 💡 

+ Useless or Meaningless Auto-Generated Tags 🏷️
+ Reviews not classified as positive👍 or negative 👎
+ Tags not classified as positive👍 or negative 👎
+ Repeated Tags 🏷️🤔
+ Paid Review Tags that don't reflect sentiments of Customers 😢
+ Misleading Images that don't match the actual product ❓
+ New Buyer or Potential customer had to go through hundreds of reviews, tags and images to judge the product properly 😳

## Demo Video 
Below is the Demo Video of our Solution located on Youtube.

[![DEMO Video](https://github.com/kshubhamm/TAGMEAI/blob/main/tagme.jpg)](https://youtu.be/c5izyZUOq5o)

## Technical Details/ Dependencies 🧰 
+ Python 🐍 
+ FastAPI 
+ Uvicorn 🌏 
+ Heroku 
+ Microsoft Azure ☁️
+ HTML5, CSS3 & JS 

For more Detail, see `requirements.txt`

## Running Tagonizer Locally 

### Frontend

1. Go to [Release](https://github.com/merrcury/Tagonizer/releases) & Download latest `Tagonizer.zip` file. 
2. Follow the below Given Illustration for setting up extension on Google Chrome running on MacOS. For other OS, it should be pretty similar. 

![Demo](demo.gif)

### Backend 

1. First Clone the repository. 
```bash
$ git clone https://github.com/merrcury/Tagonizer.git
```
2. Navigate into Cloned Repository. 
```bash 
$ cd Tagonizer
```
3. Create Virtual Environment and Activate it. 
```bash 
$ python -m venv venv/
$ source venv/bin/activate
```
4. Install Requirements
```bash 
$ pip install -r requirements.txt
```
5. [Create an Azure resource](https://docs.microsoft.com/en-us/azure/cognitive-services/text-analytics/how-tos/text-analytics-how-to-call-api) for Text Analytics. Afterwards, [get the key](https://docs.microsoft.com/en-us/azure/cognitive-services/text-analytics/how-tos/text-analytics-how-to-call-api) generated for you to authenticate your requests.
6. Set Environment Variable `KEY`, `ENDPOINT`, `LOCATION` with secret token/key, endpoint/base-url and location of resource respectively. 
7. [Create a Computer Vision resource](https://portal.azure.com/#create/Microsoft.CognitiveServicesComputerVision)  in the Azure portal to get your key and endpoint. After it deploys, click Go to resource.
  + You will need the key and endpoint from the resource you create to connect your application to the Computer Vision service. You'll paste your key and endpoint into the code below later in the quickstart.
  + You can use the free pricing tier (F0) to try the service, and upgrade later to a paid tier for production.
  + Save them in Environment as `VKEY` & `VENDPOINT` for both key and endpoint respectively.

8. Run the following command to start backend at `http://localhost:8000/`
```bash
$ uvicorn API.main:app --reload --host=0.0.0.0 --port=8000
```
9. Open `http://localhost:8000/` in browser of your choice. You will be greeted with Swagger UI and further details are present there. 



