# Use the official Python base image
FROM python:3.13

ADD . .

# Set the working directory inside the container
WORKDIR /bike_sharing_api


RUN pip install -r test_requirements.txt

#COPY /dist/bikeshare_model-0.0.1-py3-none-any.whl ./bike_sharing_api/bikeshare_model-0.0.1-py3-none-any.whl

EXPOSE 8001

CMD [ "python" , "app/main.py"]