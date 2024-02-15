FROM python:3.10

WORKDIR /app

COPY . /app

# Install the requirements
RUN pip install -r requirements.txt

# Delete logs folder if it exists (otherwise fileexsist error when launching the container)
RUN rm -rf logs

EXPOSE 5000

#to have it work in the CMD line below
ENV FLASK_APP=app.py

# using the instruction given in the readme file
CMD ["flask", "run", "--host=0.0.0.0"] 
