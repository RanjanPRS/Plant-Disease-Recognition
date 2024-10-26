FROM python:3.10-slim

COPY . /app

WORKDIR /app

RUN pip install -r requirements.txt

EXPOSE 80

RUN mkdir ~/.streamlit

COPY config.toml ~/.streamlit/config.toml

COPY credentials.toml ~/.streamlit/credentials.toml

ENTRYPOINT ["python", "-m", "streamlit", "run"]

CMD ["main.py"]
