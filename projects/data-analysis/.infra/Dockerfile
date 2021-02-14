FROM python:3

WORKDIR /usr/src/app

COPY .infra/jupyter-notebook /root/.jupyter

COPY app ./

RUN apt-get update

RUN pip install --no-cache-dir -r requirements.txt

CMD ["jupyter notebook --allow-root --no-browser"]
