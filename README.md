# ♻️ Ecoleta-NLW
> ♻️ Ecoleta Project, built during Rocketseat online classes event - Next Level Week

This project has the objective to allow people to register Collect Points of many types of waste, which cannot (or is not recommended to) be discarded in the common way.

![](banner.png)

## :wrench: Run setup

### Dependencies Installation 

How to install all development dependencies:
```
cd ./web
npm install

cd ../server
npm install

cd ../mobile
npm install
```

## Running each environment

### :bulb: Backend / Server folder

After installing the dependencies, just run the following command:

```
npm run dev
```

#### Endpoints

Here we have four endpoints that are used by the Mobile App and Website:

##### http:<span></span>//localhost:3333/points

1. Method: POST
2. Description: Create a new waste collect point
3. Fields: name: string, email: string, whatsapp: string, latitude: number, longitude: number, city: string, uf: string, items: number[], image: File

##### http:<span></span>//localhost:3333/points/:id

1. Method: GET
2. Description: List a specific point based on point id

##### http:<span></span>//localhost:3333/points

1. Method: GET
2. Description: List all the points that fit with especified filter sent in query params
3. Query Params: City, UF, Items (Separated by Comma)

##### http:<span></span>//localhost:3333/items

1. Method: GET
2. Description: List all items registered


### :art: Frontend / Web folder

After installing the dependencies, just run the following command:
```
npm start
```

Make sure to have the backend running on background, otherwise you won't be able to make any http request to the backend.

### 📱 Mobile / Mobile Folder

After installing the dependencies, just run the following command:
```
npm start
```

A new window will open. This part was created with Expo, so you can use the QR Code to test the app using your own phone. Just make sure to have the Expo App installed, then scan the QR Code and you'll be ready to go. Don't forget to keep the backend running on background as well.
