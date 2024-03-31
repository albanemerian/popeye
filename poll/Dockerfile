FROM python:3
WORKDIR /app
COPY . /app
RUN pip3 install -r requirements.txt
EXPOSE 80
COPY . . 
CMD ["flask", "run", "--host=0.0.0.0", "--port=80"]
