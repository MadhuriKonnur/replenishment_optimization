This project is based on replenishment optimization for Covid Vaccination.

Tech stack: 
Model is trained and saved as pkl file under model folder. A simple html file with name main.html is under templates. Flask application is built which takes 
inputs from main.html, and feeds it to model and gives the output as predition.
Deployment:
- Close the repo 
- Make sure Docker file has EXPOSE port 80 and app.py expose port 5001. In case if these ports are used in your server, please make necessary changes
- Build the docker with command docker build -t my_app . 
- Once Build is successful you cna see the image by running the command docker images 
- Run the docker container with command docker run -p 80:5001 my_app . (please change port numbers accordingly)
- Open the browser and http://ip_address should bring up a UI to enter the details and once duly entered all the fields click on Submit Query will show the Predition
