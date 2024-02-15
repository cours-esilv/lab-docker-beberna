FROM python:3.10

WORKDIR /app

COPY . /app

# Install the requirements
RUN pip install -r requirements.txt

RUN mkdir logs

EXPOSE 5000

#to have it work in the CMD line below
ENV FLASK_APP=app.py

# ysing the instruction given in the readme file
CMD ["flask", "run", "--host=0.0.0.0"] 
