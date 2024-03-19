FROM python:3.12.2

# create the working dir
RUN mkdir /data
COPY ./requirements.txt /data/requirements.txt

# Install requirements as defined in the file

RUN  pip install --upgrade pip && \
  pip install -r /data/requirements.txt && \
  rm /data/requirements.txt

WORKDIR /data
CMD ["jupyter", "notebook", "--no-browser", "--allow-root", "--port", "4242"]
