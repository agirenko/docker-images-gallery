FROM python:3.10.6

WORKDIR /app

EXPOSE 5050

COPY Pipfile Pipfile.lock ./

RUN pip install flask
RUN pip install requests
RUN pip install python-dotenv
RUN pip install flask-cors
RUN pip install flask_cors

# RUN pip install pipenv
# RUN pip freeze > requirements.txt
# RUN pip install -r requirements.txt

COPY . ./

CMD ["python", "main.py"]
#CMD ["/bin/bash"]


