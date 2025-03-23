# Use the official Python base image
FROM python:3.13-slim

ADD . .

# Set the working directory inside the container
WORKDIR /M6_MP1_bikeshare_project/bikeshare_project/bike_sharing_api

# Copy the current directory contents into the container at the working directory
COPY /M6_MP1_bikeshare_project/bikeshare_project/dist/bikeshare_model-0.0.1-py3-none-any.whl ./bikeshare_model-0.0.1-py3-none-any.whl
COPY /M6_MP1_bikeshare_project/bikeshare_project/bike_sharing_api/requirements.txt ./requirements.txt


RUN pip install -r ./requirements.txt

#COPY /dist/bikeshare_model-0.0.1-py3-none-any.whl ./bike_sharing_api/bikeshare_model-0.0.1-py3-none-any.whl

CMD [ "python", "app/main.py" ]




