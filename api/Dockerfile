# Dockerfile !

# pull the parent image
FROM python:2.0-alpine

# set the working directory
WORKDIR /webapp

# install python dependencies
RUN pip install 

# copy the requirements.txt into the container
COPY requirements.txt .

# install dependencies in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# copy the rest of the application code into the container
COPY . .

# expose the application to port 7000
EXPOSE 7000

# start the application when the cotainer is running
CMD [ "python" , "manage.py" , "runserver" , "0.0.0.0:7000"]