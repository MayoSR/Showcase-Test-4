FROM python:3.7-slim

ENV CONTAINER_HOME=/var/www

ADD . $CONTAINER_HOME
WORKDIR $CONTAINER_HOME

ENV APP_SETTINGS=config.DevelopmentConfig
ENV DATABASE_URL=postgresql://localhost/my_app_db 
RUN pip install -r $CONTAINER_HOME/requirements.txt