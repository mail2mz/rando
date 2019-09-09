#development  step:
   Backend
	$ mkdir rando; cd rando
	$ npm init -y
	$ npm i -S express password-generator
	modify node.js, index.js
	$ npm start
			Open up your browser and go to http://localhost:5000/api/passwords
   Frontend
	$create-react-app client
	modify client/package.json, client/App.js
	$ cd client; 
	$ npm start;
			Go to http://localhost:3000 and the app should be working! 

#Deploying to Heroku:
	$ add "heroku-postbuild" script in top-level package.json
		"scripts": {
  				"start": "node index.js",
  				"heroku-postbuild": "cd client && npm && npm run build"
		}
	on top lovel:
	$ git add .
	$ git commit -m "Ready for awesome"
	$ heroku create
	$ git push heroku master

Orignal from https://daveceddia.com/deploy-react-express-app-heroku/
