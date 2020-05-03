# Base Image
FROM python:3

# create and set working directory
RUN mkdir /app
WORKDIR /app
COPY requirements.txt /app/
ADD . /app/
# Add current directory code to working directory
RUN /usr/local/bin/python -m pip install --upgrade pip
RUN pip install -r requirements.txt



# set default environment variables
ENV PYTHONUNBUFFERED 1

RUN ls -a

# set project environment variables
# grab these via Python's os.environ
# these are 100% optional here
ENV PORT=8000

EXPOSE 8000

CMD [ "python", "./manage.py", "runserver", "0.0.0.0:8000"]

