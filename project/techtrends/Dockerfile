FROM python:3.8

# working directory for the container
WORKDIR /app

# Copy current directory contents into the container
COPY . /app

RUN pip install -r requirements.txt


#port 3111
EXPOSE 3111

# command to run on container start
CMD ["sh", "-c", "python init_db.py && python app.py"]
